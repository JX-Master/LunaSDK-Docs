# Getting Started
Thanks for using Luna SDK. In this article, we will guide you to Luna SDK by creating a simple program that draws one textured 3D cube on the screen. At the end of this article, you will have a basic understanding of using Luna SDK to create a simple graphic program, and can start to explore more advanced features provided by Luna SDK.

## Prerequisites
In this article, we assume that you have the basic knowledge of C++ programming and graphics programming (like using D3D11, D3D12 or OpenGL). You should also correctly setup Luna SDK and developing environments using the instructions provided in `README.md` of the project.

## Creating the program
The first thing to do is to create an binary target for our demo program, so that XMake build system can correctly build our program. To create a new program, create a new folder in the `{LUNA_ROOT_DIR}/Programs` directory, and name it `DemoApp`. In this folder, create a new Lua script file called `xmake.lua`, and fill its content with the following text:

```lua
target("DemoApp")
    set_luna_program()
    add_files("**.cpp")
    add_deps("Runtime", "Window", "RHI", "ShaderCompiler", "Image")
target_end()
```

`target` and `target_end` enclose a *target scope*, where all target definitions are specified. `set_luna_program` tells XMake that we are defining one Luna SDK program, this will let XMake set the target kind to "binary" and import all SDK options for the program. `add_files("**.cpp")` tells XMake to add all CPP files in the current directory and all subdirectories to the this target. `add_deps` lists all libraries that this program links to, in our example, we need to link to the SDK runtime (`Runtime`), the window module (`Window`) , the Graphics API module (`RHI`), the shader compiler module (`ShaderCompiler`) and the image file module (`Image`). If you got unresolved external symbol errors when compiling, make sure you already link correct libraries.

Then we need to create source CPP files for our program. Since out demo program is simple, we only create one "main.cpp" file to host all source codes. After this, the `DemoApp` directory should looks like this:
```
DemoApp
|- xmake.lua
|- main.cpp
```
The last thing is to add one line in the end of `{LUNA_ROOT_DIR}/Programs/xmake.lua` to tell XMake to add our program in the solution:
```lua
includes("DemoApp")
```
Well done, now every is set up and we can start to program our first Luna SDK program!

## Program structure

Next, fills `main.cpp` with the following initial content. As we go further, we will add more properties and methods to our `DemoApp` structure, while remaining the rest part unchanged.
```c++
#include <Runtime/Runtime.hpp>
#include <Runtime/Module.hpp>
#include <Runtime/Debug.hpp>
using namespace Luna;
struct DemoApp
{
    RV init();
    RV update();
    bool is_closed();
};
DemoApp* g_app = nullptr;
RV DemoApp::init()
{
    return ok;
}
RV DemoApp::update()
{
    return ok;
}
bool DemoApp::is_closed()
{
    return false;
}
RV run_app()
{
    auto result = init_modules();
    if(failed(result)) return result;
    g_app = memnew<DemoApp>();
    result = g_app->init();
    if(failed(result)) return result;
    while(!g_app->is_closed())
    {
        result = g_app->update();
        if(failed(result)) return result;
    }
    return ok;
}
int main()
{
    bool initialized = Luna::init();
    if(!initialized) return -1;
    RV result = run_app();
    if(failed(result)) debug_printf(explain(result.errcode()));
    if(g_app) memdelete(g_app);
    Luna::close();
    return 0;
}
```
The first three lines includes the header files that we need to include to compile the program, which are:
* <Runtime/Runtime.hpp> for `Luna::init()` and `Luna::shutdown()`.

* <Runtime/Module.hpp> for `Luna::init_modules()`.

* <Runtime/Debug.hpp> for `Luna::debug_printf()`.

You can include any SDK interface header files using similar syntax: `#include <Module/File>`. We set `{LUNA_ROOT_DIR}/Engine` as the global include directory, the user may check it for available header files. In this example, all header files are from the `Runtime` module, which is the core module of Luna SDK that provides fundamental SDK features.

The next statement is `using namespace Luna`. In Luna SDK, all types, functions and variables are defined in `Luna` namespace, and every module will define its elements in nested namespace, such as `Luna::RHI`. So, we use this statement to prevent spelling the `Luna::` namespace prefix in our following code.

The program starts with the `main` function, just like any normal C/C++ program. In the main function, we firstly call `Luna::init` to initialize Luna SDK. This function should be called before any other Luna SDK function. `Luna::init` returns one Boolean value to indicate whether the SDK initialization is succeeded, if the return value is `false`, we then return `-1` and exit the program to indicate one runtime error. If `Luna::init` returns `true`, then one `Luna::close` call is need before the program exit to let the SDK clean up all internal resources.

We then wrap the real program logic in one `run_app` function. The return type of `run_app` is `RV`, which is a shortcut for `R<void>`, this is part of the error handling mechanism of Luna SDK. `R<T>` is a structure that encapsulates one return value with type `T` and one error code with type `ErrCode`, which is simply an alias of `usize` (or `std::size_t`). If the function succeeds, the returned value will be one `T`-typed value and one error code `0`; if the function fails, the returned value will be one non-zero error code, and the `T`-typed value will be uninitialized and inaccessible, you may call `errcode()` to fetch the error code from `R<T>`, and may call `explain` to get a brief description of the error. In our `main` function, we check whether our `run_app` function is failed by using `failed` helper function (there is also one `succeeded` helper function available), then we print the error description and exits the program if any error occurs.

In our `run_app` function, the first thing to do is calling `init_modules`, which will initialize all linked SDK modules for our program. We deliberately separate module initialization from `Luna::init` so that the user get a chance to set module initialization parameters before initializing modules, and modules can also indicate initialization failure by returning error codes (error handling system is available after `Luna::init`). Then, we allocate and initialize one new object of `DemoApp` type by calling `memnew` function. The following table shows memory allocation functions used in Luna SDK:

| Luna SDK functions                 | C++ functions/keywords |
| ---------------------------------- | ---------------------- |
| `memalloc(size, alignment)`        | `malloc(size)`         |
| `memfree(ptr, alignment)`          | `free(ptr)`            |
| `memrealloc(ptr, size, alignment)` | `realloc(ptr, size)`   |
| `memsize(size, alignment)`         | N/A                    |
| `memnew<T>(args...)`               | `new T (args...)`      |
| `memdelete(ptr)`                   | `delete ptr`           |

The user should uses allocation functions provided by Luna SDK instead of those provided by C++ std. `DemoApp` will contain all states and logics for our demo program. The created `DempApp` instance then will be assigned to a global variable `g_app`, and will be deleted by `memdelete` when the program exits.

`DemoApp` has three functions: `init`, `update` and `is_closed`. The `init` function initializes the program, and reports errors if the initialization is failed; the `update` function updates the program state and renders the image at every frame; the `is_exiting` function checks whether the program is exiting. We will implement these three methods in the following sections. 

The rest part of our `run_app` function simply checks whether the program is exiting by calling `is_exiting`, and updates the program when it is not exiting. 

After filling this content, execute `xmake build DemoApp` on terminal or click `build` button on your IDE, you should successfully build the `DemoApp` program.

## Window creation and event handling

Now that we have one basic program structure, we need to create a system window so that we can render images to it. We also need to implement window event handling so that the program can exit when the user clicks the close button of the window.

Window creation is fairly simple, we firstly need to introduce one new header:

```c++
#include <Window/Window.hpp>
```

then we add one new property to our `DemoApp` structure:

```c++
struct DemoApp
{
    Ref<Window::IWindow> window;

    RV init();
    RV update();
    bool is_exiting();
    RV resize(u32 width, u32 height);
};
```

The window object is provided by `Window::IWindow*` interface pointer in Luna SDK, which points to a *boxed object* which manages its lifetime using *reference counting*. `IWindow` interface may have different implementations on different platforms, by they all provide the same functionality required by this interface. `Ref<T>` is a smart pointer for boxed objects, it will manage the reference counter of the pointing object automatically when being constructed and destructed, so the user does not need to call `object_retain` and `object_release` manually. You may compare `Ref<T>` to `ComPtr` used in Microsoft's Component-Object Model (COM), or the *automatic reference counting* in Apple's Objective-C and Swift. The default constructor of `Ref<T>` initializes the pointer to `nullptr`, so we need to assign it with a valid object.

Then we need to create our window in `DemoApp::init`:

```c++
RV DemoApp::init()
{
    lutry
    {
        luset(window, Window::new_window("DemoApp", 0, 0, 0, 0, nullptr, 
            Window::WindowCreationFlag::default_size | Window::WindowCreationFlag::position_center |
            Window::WindowCreationFlag::minimizable | Window::WindowCreationFlag::maximizable |
            Window::WindowCreationFlag::resizable));
    }
    lucatch
    {
        return lures;
    }
    return ok;
}
```

Besides the `new_window` function that creates the window, there are four new keywords in our code: `lutry`, `lucatch`, `luset` and `lures`. These four keywords are macros that enables us to write error handling using a simpler try-catch style, rather than fetching and checking error codes once and once again for every function call that may fail. `lutry` and `lucatch` must be used in pairs, next to each other. In the `lutry` block, the user may define multiple `lulet` , `luset` or `luexp` statements, `lulet` statement creates a new local variable to hold the  return value of the function, and jumps to `lucatch` if the function fails; `luset` assigns the return value to one existing variable, and jumps to `lucatch` if the function fails; `luexp` is used if the function does not return any value, it simply checks whether the function succeeds, and jumps to `lucatch` if not. The user may also call `luthrow` manually in `lutry` block to jump to `lucatch` directly.

In the `lucatch` block, `lures` is provided as the error code that causes the failure. You may use one `switch` statement on the `lures` to handle specific errors, or you can propagate the error directly to parent function by `return lures`. Since error propagating is so commonly used, we create another macro `lucatchret` to replace `lucatch { return lures; }`, so the code above can be written as:

```c++
RV DemoApp::init()
{
    lutry
    {
        luset(window, Window::new_window("DemoApp", 0, 0, 0, 0, nullptr, 
            Window::WindowCreationFlag::default_size | Window::WindowCreationFlag::position_center |
            Window::WindowCreationFlag::minimizable | Window::WindowCreationFlag::maximizable |
            Window::WindowCreationFlag::resizable));
    }
    lucatchret;
    return ok;
}
```

Since we use `goto` statement to implement `lutry` and `lucatch`, it you needs multiple lutry-lucatch pairs in one function, you should use a numbered version for every pair (like `lutry2`, `lucatch2`, `luset`2, `lures2`, etc.). In most cases, only one lutry-lucatch pair is sufficient.

Now let's get back to `Window::new_window` function that does the actual work. The function signature of this function is:

```c++
R<Ref<IWindow>> new_window(const c8* title, 
	i32 x, i32 y, i32 width, i32 height, 
	monitor_t monitor = nullptr,
	WindowCreationFlag flags = WindowCreationFlag::none)
```

Most parameters are self-explained, `monitor` is one handle to one system monitor, if you need to create a full-screen window, you need to specify the monitor to create window for, otherwise just leave it `nullptr`. `flags` are a combination of `WindowCreationFlag` enumeration class that lists flags for window creation process. If `WindowCreationFlag::position_center` is set, then `x` and `y` will be ignored and the window will be positioned on the center of the primary monitor; if `Window::WindowCreationFlag::default_size` is set, then `width` and `height` will be ignored and the window size will be set to a proper value based on the primary monitor's resolution.

After the window is created, we need to register window event callbacks so that we can handle window events properly. In this example, the events we need to handle is the close event (triggered when the close button of the window is pressed) and the framebuffer resize event (triggered when the window framebuffer size is changed). This can be done by the following statements:

```c++
window->get_close_event() += [](Window::IWindow* window) { window->close(); };
window->get_framebuffer_resize_event() += [](Window::IWindow* window, u32 width, u32 height) {
    lupanic_if_failed(g_app->resize(width, height));
};
```

`get_close_event` and `get_framebuffer_resize_event` are methods of `IWindow` that gets the close event and the framebuffer resize event object of the window. The event object is a collection of callback functions that once triggered, calls all the callback functions. We then register one callback function to the close event that closes the window immediately, and one callback function to the framebuffer resize event that calls the `resize` method of our `DempApp`. The `resize` method is currently empty, we will fill the content of this method when we create render textures later:

```c++
RV DemoApp::resize(u32 width, u32 height)
{
    return ok;
}
```

Window events are not polled automatically, we need to tell the window system to poll events at every frame by calling `Window::poll_events` in `update` function:

```c++
RV DemoApp::update()
{
    Window::poll_events();
    return ok;
}
```

This call polls events for all existing windows, so we don't need to provide specific window here. After we correctly handle the close event, we can complete the `is_closed` method of `DemoApp`:

```c++
bool DemoApp::is_exiting()
{
    return window->is_closed();
}
```

So far, the complete code for `main.cpp` is:

```c++
#include <Runtime/Runtime.hpp>
#include <Runtime/Module.hpp>
#include <Runtime/Debug.hpp>
#include <Window/Window.hpp>

using namespace Luna;

struct DemoApp
{
    Ref<Window::IWindow> window;

    RV init();
    RV update();
    bool is_exiting();
    RV resize(u32 width, u32 height);
};

DemoApp* g_app = nullptr;

RV DemoApp::init()
{
    lutry
    {
        luset(window, Window::new_window("DemoApp", 0, 0, 0, 0, nullptr, 
            Window::WindowCreationFlag::default_size | Window::WindowCreationFlag::position_center |
            Window::WindowCreationFlag::minimizable | Window::WindowCreationFlag::maximizable |
            Window::WindowCreationFlag::resizable));
        window->get_close_event() += [](Window::IWindow* window) { window->close(); };
        window->get_framebuffer_resize_event() += [](Window::IWindow* window, u32 width, u32 height) {
            lupanic_if_failed(g_app->resize(width, height));
        };
        
    }
    lucatchret;
    return ok;
}
RV DemoApp::update()
{
    Window::poll_events();
    return ok;
}
bool DemoApp::is_exiting()
{
    return window->is_closed();
}
RV DemoApp::resize(u32 width, u32 height)
{
    return ok;
}
RV run_app()
{
    auto result = init_modules();
    if(failed(result)) return result;
    g_app = memnew<DemoApp>();
    result = g_app->init();
    if(failed(result)) return result;
    while(!g_app->is_exiting())
    {
        result = g_app->update();
        if(failed(result)) return result;
    }
    return ok;
}
int main()
{
    bool initialized = Luna::init();
    if(!initialized) return -1;
    RV result = run_app();
    if(failed(result)) debug_printf(explain(result.errcode()));
    if(g_app) memdelete(g_app);
    Luna::close();
    return 0;
}
```

Build and run `DemoApp`, and you will see a blank window appears, and the program exits when you click the close button of the window.

![](getting_started/DemoApp-window.png)

## Fetching graphic device

After the window is created, we can start drawing our box. In Luna SDK, all graphic resources are related to one specific graphic device represented by `RHI::IDevice`, which is the virtual representation of the physical graphic device on the platform, so we need to add one property to `DemoApp` to hold this device:

```c++
Ref<RHI::IDevice> dev;
```

When `RHI` module initializes, it automatically chooses the most suitable physical device and creates one device for you, which can be fetched by `RHI::get_main_device()`. You may also create additional devices for special use, but in our `DemoApp`, we will stick to the default one  by adding the following line in the `lutry ` scope of `DemoApp::init`:

```c++
dev = RHI::get_main_device();
```

We can also import all RHI types and functions by `using namespace RHI;` so that we don't need to spell them all over the `init` function:

```c++
using namespace RHI;
```

The code of `DemoApp::init` should look similar to:

```c++
RV DemoApp::init()
{
    lutry
    {
    	luset(window, Window::new_window("DemoApp", 0, 0, 0, 0, nullptr, 
            Window::WindowCreationFlag::default_size | Window::WindowCreationFlag::position_center |
            Window::WindowCreationFlag::minimizable | Window::WindowCreationFlag::maximizable |
            Window::WindowCreationFlag::resizable));
        window->get_close_event() += [](Window::IWindow* window) { window->close(); };
        window->get_framebuffer_resize_event() += [](Window::IWindow* window, u32 width, u32 height) {
            lupanic_if_failed(g_app->resize(width, height));
        };

        dev = RHI::get_main_device();
        using namespace RHI;
        // New resource creation code goes here...
    }
    lucatchret;
    return ok;
}
```

Unless explicitly specified, all codes we need to add to `DemoApp::init` in the following sections are added to the end of `lutry` scope, not in the end of the function scope directly.

## Creating command queue and command buffer

Luna SDK employs *deferred execution model*, where render and compute calls are recorded as *commands* in *command buffers*, then submitted to GPU explicitly by submitting *command buffers* to *command queues*. The command buffer object manages memory allocated to store commands, it also tracks the execution state for commands in the buffer when the buffer is submitted for execution. The command queue object is a FIFO message buffer between CPU and GPU. CPU can push command buffers into the queue, and GPU will pop command buffers from the queue and execute commands in the buffer. Command buffers in the queue are guaranteed to execute one after another, the next command buffer will not being executed until the last command buffer is finished.

We need to add two new properties to `DemoApp` to hold the command queue and command buffer:

```c++
Ref<RHI::ICommandQueue> queue;
Ref<RHI::ICommandBuffer> cmdbuf;
```

Then we can create the objects by adding the following codes to `DemoApp::init`:

```c++
luset(queue, dev->new_command_queue(CommandQueueType::graphic));
luset(cmdbuf, queue->new_command_buffer());
```

When creating command queues, we must specify the type of the queue. There are three different queue types: `graphic`, `compute` and `copy`. The copy queue only accepts copy commands, and is used for transferring data between different resources; the compute queue accepts copy and compute tasks, while the graphic queue accepts graphic, compute and copy commands. In our case, we need to create one graphic queue.

Note that command buffers are created from command queues, not from the graphic device directly. Once the command buffer is created, it is bound to the queue who created the buffer, and the binding can not be changed.

## Creating swap chain

The swap chain object contains resources that are used to present render results to our window. 

We need to add one new property to `DemoApp` to hold the command queue and command buffer:

```c++
Ref<RHI::ISwapChain> swap_chain;
```

In Luna SDK, the swap chain presentation is also a command that should be submitted using graphic command queues, so we need to specify the command queue we need to use when creating swap chains like so:

```c++
luset(swap_chain, new_swap_chain(queue, window, SwapChainDesc(0, 0, Format::rgba8_unorm, 2)));
```

The swap chain is described by one `SwapChainDesc` structure:

```c++
struct SwapChainDesc
{
	u32 width;
	u32 height;
	Format pixel_format;
	u32 buffer_count;
};
```

When used for creating swap chains, you may pass `0` for `width` and `height` property, which indicates the system to use the window framebuffer size as the size of the swap chain.

The swap chain needs to be resized when the window framebuffer size is changed. This can be done by filling `DemoApp::resize` method with the following codes:

```c++
RV DemoApp::resize(u32 width, u32 height)
{
    lutry
    {
        using namespace RHI;
        auto dev = get_main_device();
        luexp(swap_chain->resize_buffers(2, width, height, Format::rgba8_unorm));
    }
    lucatchret;
    return ok;
}
```

`ISwapChain::resize_buffers` will recreate the swap chain buffer according to the new window framebuffer size.

## Creating descriptor set layout and descriptor set

The *descriptor set* object stores descriptors that bind resources to graphic or compute pipeline. Descriptors have the following types:

1. Constant buffer view, which binds constant global data to shaders.
2. Shader resource view, which binds read-only textures and structured buffers to shaders.
3. Unordered access view, which binds writable resources to compute shaders.
4. Sampler, which stores sampling settings and exposes those settings for shaders.

Every pipeline may bind multiple descriptor sets, every descriptor set may contain all four kinds of descriptors listed above. The *descriptor set layout* object stores the layout of one descriptor set object, including the number of descriptors in the descriptor set and the property of each descriptor.

In order to create one descriptor set layout object, we need to fill one `DescriptorSetLayoutDesc` structure. Here is the definition of `DescriptorSetLayoutDesc` structure:

```c++
struct DescriptorSetLayoutDesc
{
	Vector<DescriptorSetLayoutBinding> bindings;
	DescriptorSetLayoutFlag flags = DescriptorSetLayoutFlag::none;
};
```

The descriptor set layout consists of multiple *bindings* specified by `DescriptorSetLayoutBinding`, each binding describes one range of the descriptor set:

```c++
struct DescriptorSetLayoutBinding
{
	DescriptorType type;
	u32 binding_slot;
	u32 num_descs;
	ShaderVisibility shader_visibility;
};
```

the `type` property describes the type of this binding. All descriptors in the same binding must be the same type:

```c++
enum class DescriptorType : u32
{
	srv,
	uav,
	cbv,
	sampler
};
```

`binding_slot` and `num_descs` describes the binding slot range of this binding, starting from `0`. All slots in `[binding_slot, binding_slot + num_descs)` will be occupied by this binding and cannot be used by other bindings. If `num_descs` is greater than `1`, then this binding will be interpreted as one descriptor array in the shader. `shader_visibility` specifies which shader may access descriptors in this binding, you may restrict the visibility of one binding to one specific shader to potentially improve performance.

We need to add two new properties to `DemoApp` to hold the descriptor set layout object and the descriptor set object:

```c++
Ref<RHI::IDescriptorSetLayout> dlayout;
Ref<RHI::IDescriptorSet> desc_set;
```

We need **1** descriptor set with **1** constant buffer view, **1** shader resource view and **1** sampler. So we can create our descriptor set layout object in `DemoApp::init` like so:

```c++
luset(dlayout, dev->new_descriptor_set_layout(DescriptorSetLayoutDesc({
    {DescriptorType::cbv, 0, 1, ShaderVisibility::vertex},
    {DescriptorType::srv, 1, 1, ShaderVisibility::pixel},
    {DescriptorType::sampler, 2, 1, ShaderVisibility::pixel}
})));
```

Then we can create one descriptor set using the descriptor set layout object:

```c++
luset(desc_set, dev->new_descriptor_set(DescriptorSetDesc(dlayout)));
```

We will fill descriptors in the set by calling `set_cbv`, `set_srv` and `set_sampler` later.

## Compiling shaders

The next thing to do is compiling shaders for the pipeline state object. Luna SDK uses HLSL as the source shader language, and uses `ShaderCompiler` module to compile HLSL to DXBC, DXIL, SPIR-V and other target shading languages. To compile shader, we need to include corresponding header files:

```c++
#include <ShaderCompiler/ShaderCompiler.hpp>
#include <RHI/ShaderCompileHelper.hpp>
```

`ShaderCompileHelper.hpp` includes `RHI::get_current_platform_shader_target_format()` function, which tell the shader compiler the native target target shader format for the current graphic API. Since our shader is rather simple, we declare our shader source code directly in the C++ source file, in `DemoApp::init` function:

```c++
const char vs_shader_code[] = R"(
cbuffer vertexBuffer : register(b0)
{
    float4x4 world_to_proj;
};
struct VS_INPUT
{
    float3 position : POSITION;
    float2 texcoord : TEXCOORD;
};
struct PS_INPUT
{
    float4 position : SV_POSITION;
    float2 texcoord : TEXCOORD;
};
PS_INPUT main(VS_INPUT input)
{
    PS_INPUT output;
    output.position = mul(world_to_proj, float4(input.position, 1.0f));
    output.texcoord = input.texcoord;
    return output;
})";

const char ps_shader_code[] = R"(
Texture2D tex : register(t1);
SamplerState tex_sampler : register(s2);
struct PS_INPUT
{
    float4 position : SV_POSITION;
    float2 texcoord : TEXCOORD;
};
float4 main(PS_INPUT input) : SV_Target
{
    return float4(tex.Sample(tex_sampler, input.texcoord));
})";
```

here we use C++ raw string syntax `R"()"` to declare multiline string without appending `\` for every string line. Note the register number specified in shader must match the binding slot specified in descriptor set layout we just created. Since we use the same slot numbering system for all descriptor types, the register number for `b`, `t`, `u` and `s` should not overlap.

Then we can compile shaders using `ShaderCompiler::ICompiler` object:

```c++
auto compiler = ShaderCompiler::new_compiler();
compiler->set_source({ vs_shader_code, strlen(vs_shader_code) });
compiler->set_source_name("DemoAppVS");
compiler->set_entry_point("main");
compiler->set_target_format(RHI::get_current_platform_shader_target_format());
compiler->set_shader_type(ShaderCompiler::ShaderType::vertex);
compiler->set_shader_model(5, 0);
compiler->set_optimization_level(ShaderCompiler::OptimizationLevel::full);
luexp(compiler->compile());
auto vs_data = compiler->get_output();
Blob vs(vs_data.data(), vs_data.size());

compiler->reset();
compiler->set_source({ ps_shader_code, strlen(ps_shader_code) });
compiler->set_source_name("DemoAppPS");
compiler->set_entry_point("main");
compiler->set_target_format(RHI::get_current_platform_shader_target_format());
compiler->set_shader_type(ShaderCompiler::ShaderType::pixel);
compiler->set_shader_model(5, 0);
compiler->set_optimization_level(ShaderCompiler::OptimizationLevel::full);
luexp(compiler->compile());
auto ps_data = compiler->get_output();
Blob ps(ps_data.data(), ps_data.size());
```

The shader compilation process is fairly simple, we just set source code, compilation settings, then triggers the compilation. The compilation result will be given by `get_output`, we use one `Blob` object , a container for binary data, to hold the compilation result. The compiled shader data will be used when creating pipeline state object later.



## Creating shader input layout and pipeline state

The graphic and compute pipeline state is described by two objects: shader input layout object and pipeline state object. Shader input layout object stores the shader binding layout information for all shader stages, while pipeline state object stores pipeline settings for all graphic stages. 

Shader input layout is described by the `ShaderInputLayoutDesc` structure, which is set by specifying layouts of descriptor sets that will be bound to this pipeline and flags that specifies shaders that are allowed to access shader inputs.

```c++
struct ShaderInputLayoutDesc
{
	Vector<IDescriptorSetLayout*> descriptor_set_layouts;
	ShaderInputLayoutFlag flags;
};
```

We need to add one new property to `DemoApp` to hold the shader input layout object:

```c++
Ref<RHI::IShaderInputLayout> slayout;
```

Then we can create shader input layout object using the following code:

```c++
luset(slayout, dev->new_shader_input_layout(ShaderInputLayoutDesc({dlayout}, 
    ShaderInputLayoutFlag::allow_input_assembler_input_layout |
    ShaderInputLayoutFlag::deny_hull_shader_access |
    ShaderInputLayoutFlag::deny_domain_shader_access |
    ShaderInputLayoutFlag::deny_geometry_shader_access)));
```

The pipeline object is described by the `GraphicPipelineStateDesc` structure or the `ComputePipelineStateDesc` structure. Since we are creating one graphic pipeline, we need to fill the `GraphicPipelineStateDesc`  structure, which is a complex structure that contains all pipeline settings for one graphic pipeline:

```c++
struct GraphicPipelineStateDesc
{
	InputLayoutDesc input_layout;
	IShaderInputLayout* shader_input_layout = nullptr;
	Span<const byte_t> vs;
	Span<const byte_t> ps;
	Span<const byte_t> ds;
	Span<const byte_t> hs;
	Span<const byte_t> gs;
	StreamOutputDesc stream_output;
	BlendDesc blend_state;
	RasterizerDesc rasterizer_state;
	DepthStencilDesc depth_stencil_state;
	IndexBufferStripCutValue ib_strip_cut_value = IndexBufferStripCutValue::disabled;
	PrimitiveTopologyType primitive_topology_type = PrimitiveTopologyType::triangle;
	u32 num_render_targets = 0;
	Format rtv_formats[8] = { Format::unknown };
	Format dsv_format = Format::unknown;
	u32 sample_count = 1;
	u32 sample_mask = 0xFFFFFFFF;
	u32 sample_quality = 0;
};
```

Most graphic settings are similar to those in D3D11, D3D12, OpenGL or Vulkan, we will not explain these settings, but only gives the code that correctly sets every setting of the pipeline. You can see docs for `RHI` module for detailed explanations of these settings.

We need to add one new property to `DemoApp` to hold the pipeline state object:

```c++
Ref<RHI::IPipelineState> pso;
```

Then we can create pipeline state object using the following code:

```c++
GraphicPipelineStateDesc ps_desc;
ps_desc.primitive_topology_type = PrimitiveTopologyType::triangle;
ps_desc.sample_mask = U32_MAX;
ps_desc.sample_quality = 0;
ps_desc.blend_state = BlendDesc(false, false, { RenderTargetBlendDesc(false, false, BlendFactor::src_alpha,
	BlendFactor::inv_src_alpha, BlendOp::add, BlendFactor::inv_src_alpha, BlendFactor::zero, BlendOp::add, LogicOp::noop, ColorWriteMask::all) });
ps_desc.rasterizer_state = RasterizerDesc(FillMode::solid, CullMode::back, 0, 0.0f, 0.0f, 0, false, true, false, false, false);
ps_desc.depth_stencil_state = DepthStencilDesc(true, true, ComparisonFunc::less_equal, false, 0x00, 0x00, DepthStencilOpDesc(), DepthStencilOpDesc());
ps_desc.ib_strip_cut_value = IndexBufferStripCutValue::disabled;
ps_desc.input_layout = InputLayoutDesc({
    {"POSITION", 0, Format::rgb32_float},
    {"TEXCOORD", 0, Format::rg32_float},
});
ps_desc.vs = vs.cspan();
ps_desc.ps = ps.cspan();
ps_desc.shader_input_layout = slayout;
ps_desc.num_render_targets = 1;
ps_desc.rtv_formats[0] = Format::rgba8_unorm;
ps_desc.dsv_format = Format::d32_float;
luset(pso, dev->new_graphic_pipeline_state(ps_desc));
```

## Creating render and depth textures

The next step is to create the render texture and depth texture that is used as render target and depth stencil target. We also need to create *render target view* object and *depth stencil view* object for our render texture and depth texture.

All graphic resources in Luna SDK, including buffers and textures, are described by `ResourceDesc` structure, and are represented by `IResource` interface. Here is the definition of the`ResourceDesc` structure:

```c++
struct ResourceDesc
{
	ResourceType type;
	ResourceHeapType heap_type;
	Format pixel_format;
	ResourceUsageFlag usages;
	u64 width_or_buffer_size;
	u32 height;
	u32 depth_or_array_size;
	u32 mip_levels;
	u32 sample_count;
	u32 sample_quality;
	ResourceFlag flags;
};
```

`type` specifies the type of the resource, like `buffer`, `texture_2d`, etc. `heap_type` specifies which memory heap to create the resource in, possible options include:

1. `local` - The resource can only be accessed by GPU, CPU access is disabled. This heap is suitable for GPU generated resources like temporary texture between render passes.
2. `shared` and `shared_upload` - The resource can be accessed by both GPU and CPU, but is optimized for maximum GPU bandwidth, CPU access is slow and limited. `shared_upload` only allows CPU-write, while `shared` allows both CPU read and write. This heap is suitable for CPU-write-once textures like static textures read from file.
3. `upload` - The resource can be written by CPU and read by GPU. This heap is suitable for resources that should be updated by CPU frequently. Textures cannot be created in this heap.
4. `readback` - The resource can be written by GPU and read by CPU. This heap is suitable for transferring data from GPU to CPU frequently. Textures cannot be created in this heap.

`pixel_format` specifies the pixel format of the resource if the resource is a texture, otherwise is ignored and will be set to `unknown`. `usages` specifies all possible roles of the resource when being bound to a pipeline. `width_or_buffer_size`, `height` and `depth_or_array_size`  specifies the size of the resource, if the resource is a buffer, only `width_or_buffer_size` is used, and specifies the size of the buffer in bytes, otherwise, based on the `type` of the resource, those three properties specifies the width, height, depth (for 3D textures) or array size (for 1D and 2D textures) of the resource. `mip_levels` specifies the number of mips that should be allocated for the resource, if this is `0`, the system allocates full mipmap chain for the resource. `sample_count` and `sample_quality` specifies the sampling configuration for MSAA textures. `flags` specifies additional flags for the texture, like whether this texture can be simultaneously accessed by multiple command queues.

To simplify the resource specification, we can use static methods provided by `ResourceDesc` to quickly construct `ResourceDesc` structure:

```c++
ResourceDesc ResourceDesc::buffer(ResourceHeapType heap_type, ResourceUsageFlag usages, u64 size, ResourceFlag flags = ResourceFlag::none);

ResourceDesc ResourceDesc::tex1d(ResourceHeapType heap_type, Format pixel_format, ResourceUsageFlag usages, u64 width, u32 array_size = 1, u32 mip_levels = 0, ResourceFlag flags = ResourceFlag::none);

ResourceDesc ResourceDesc::tex2d(ResourceHeapType heap_type, Format pixel_format, ResourceUsageFlag usages, u32 width, u32 height, u32 array_size = 1, u32 mip_levels = 0, u32 sample_count = 1, u32 sample_quality = 0, ResourceFlag flags = ResourceFlag::none);

ResourceDesc ResourceDesc::tex3d(ResourceHeapType heap_type, Format pixel_format, ResourceUsageFlag usages, u32 width, u32 height, u32 depth, u32 mip_levels = 0, ResourceFlag flags = ResourceFlag::none);
```

Back to our `DemoApp`, we need to add four new properties to `DemoApp` to hold the render texture, the depth texture, and two views:

```c++
Ref<RHI::IResource> rt_tex;
Ref<RHI::IRenderTargetView> rtv;
Ref<RHI::IResource> depth_tex;
Ref<RHI::IDepthStencilView> dsv;
```

Then we can create textures using the following code:

```c++
auto window_size = window->get_framebuffer_size();

luset(rt_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::rgba8_unorm, ResourceUsageFlag::shader_resource | ResourceUsageFlag::render_target, window_size.x, window_size.y, 1, 1)));

luset(depth_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::d32_float, ResourceUsageFlag::depth_stencil, window_size.x, window_size.y, 1, 1)));
```

Note that when retrieving window size for rendering, we need to call `IWindow::get_framebuffer_size` instead of `IWindow::get_size`, on some platforms the window size is not necessary measured in pixels, causing these two methods return different values.

We then need to create the render target view and depth stencil view for these two textures. Render target views and depth stencil views describes which portion of the texture will be bound to the graphic pipeline. Unlike other views, these two views are represented by dedicated objects: `IRenderTargetView` and `IDepthStencilView`, they can be created using the following code:

```c++
luset(rtv, dev->new_render_target_view(rt_tex));
luset(dsv, dev->new_depth_stencil_view(depth_tex));
```

these two methods accepts additional `RenderTargetViewDesc` and `DepthStencilViewDesc` structures when creating views, but since we are using the default settings, these two structures can be omitted.

Since we are using the window size as the render texture size, these textures should also be recreated when the window framebuffer is changed. This can be done by adding the following code to the `DemoApp::resize` method:

```c++
luset(rt_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::rgba8_unorm, 
    ResourceUsageFlag::shader_resource | ResourceUsageFlag::render_target, width, height, 1, 1)));
luset(depth_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::d32_float, 
     ResourceUsageFlag::depth_stencil, width, height, 1, 1)));
luset(rtv, dev->new_render_target_view(rt_tex));
luset(dsv, dev->new_depth_stencil_view(depth_tex));
```

## Creating buffers

The next step is to create buffers used in our `DemoApp`, including:

1. The vertex buffer and index buffer for our box mesh.
2. The constant buffer for camera properties.

Firstly we need to define the vertex structure of our box. Adding the following code after the declaration of `DemoApp` structure:

```c++
struct Vertex
{
    Float3U position;
    Float2U texcoord;
};
```

`Float2U` and `Float3U` are vector types used in Luna SDK, which represent 2D and 3D vectors. In Luna SDK, we have 16-bytes aligned vector types `Float2`, `Float3`, `Float4`, and unaligned vector types `Float2U`, `Float3U` and `Float4U`. The aligned vector types are used for calculations, SIMD functions like `min`, `max`, `lerp`, `clamp` only accepts aligned types, while unaligned vector types are used for storing and transferring data, such as in this case. The size of aligned vector types are all 16 bytes, while the size of unaligned types are 8, 12 and 16 for `Float2U`, `Float3U` and `Float4U`.

We need to add three new properties to `DemoApp` to hold the these three buffers:

```c++
Ref<RHI::IResource> vb;
Ref<RHI::IResource> ib;
Ref<RHI::IResource> cb;
```

Then, we need to create the vertex buffer and index buffer for our box using the following code:

```c++
Vertex vertices[] = {
    {{+0.5, -0.5, -0.5}, {0.0, 1.0}}, {{+0.5, +0.5, -0.5}, {0.0, 0.0}},
    {{+0.5, +0.5, +0.5}, {1.0, 0.0}}, {{+0.5, -0.5, +0.5}, {1.0, 1.0}},
    {{+0.5, -0.5, +0.5}, {0.0, 1.0}}, {{+0.5, +0.5, +0.5}, {0.0, 0.0}},
    {{-0.5, +0.5, +0.5}, {1.0, 0.0}}, {{-0.5, -0.5, +0.5}, {1.0, 1.0}},
    {{-0.5, -0.5, +0.5}, {0.0, 1.0}}, {{-0.5, +0.5, +0.5}, {0.0, 0.0}},
    {{-0.5, +0.5, -0.5}, {1.0, 0.0}}, {{-0.5, -0.5, -0.5}, {1.0, 1.0}},
    {{-0.5, -0.5, -0.5}, {0.0, 1.0}}, {{-0.5, +0.5, -0.5}, {0.0, 0.0}},
    {{+0.5, +0.5, -0.5}, {1.0, 0.0}}, {{+0.5, -0.5, -0.5}, {1.0, 1.0}},
    {{-0.5, +0.5, -0.5}, {0.0, 1.0}}, {{-0.5, +0.5, +0.5}, {0.0, 0.0}},
    {{+0.5, +0.5, +0.5}, {1.0, 0.0}}, {{+0.5, +0.5, -0.5}, {1.0, 1.0}},
    {{+0.5, -0.5, -0.5}, {0.0, 1.0}}, {{+0.5, -0.5, +0.5}, {0.0, 0.0}},
    {{-0.5, -0.5, +0.5}, {1.0, 0.0}}, {{-0.5, -0.5, -0.5}, {1.0, 1.0}}
};
u32 indices[] = {
    0, 1, 2, 0, 2, 3, 
    4, 5, 6, 4, 6, 7, 
    8, 9, 10, 8, 10, 11,
    12, 13, 14, 12, 14, 15,
    16, 17, 18, 16, 18, 19,
    20, 21, 22, 20, 22, 23
};
luset(vb, dev->new_resource(ResourceDesc::buffer(ResourceHeapType::shared_upload, ResourceUsageFlag::vertex_buffer, sizeof(vertices))));
luset(ib, dev->new_resource(ResourceDesc::buffer(ResourceHeapType::shared_upload, ResourceUsageFlag::index_buffer, sizeof(indices))));
void* mapped = nullptr;
luexp(vb->map_subresource(0, false, &mapped));
memcpy(mapped, vertices, sizeof(vertices));
vb->unmap_subresource(0, true);
luexp(ib->map_subresource(0, false, &mapped));
memcpy(mapped, indices, sizeof(indices));
ib->unmap_subresource(0, true);
```

We firstly define vertex and index data for our box, then we create two buffer resources to hold the vertex and index data. Those two resources are created in `shared_upload` heap, so we can upload data to the resource, while still achieving maximum GPU bandwidth.  After the resource is created, we can map the resource to system memory by calling `IResource::map`, and retrieving one pointer to the memory, then we use `memcpy` to copy buffer data, and use `IResource::unmap` to release the memory mapping, and store the data to the resource.

We can use similar code to create the constant buffer for uploading camera properties, but there are two differences. First, the graphic device usually has alignment requirements for constant buffers, which can be fetched from `IDevice::get_constant_buffer_data_alignment()`, so we use `align_upper` helper function to adjust the size of our constant buffer resource to meet the alignment requirement. Second, since we need to update constant buffer data once every frame, we should choose `upload` heap instead of `shared_upload` for maximum CPU bandwidth.

In our `DemoApp`, the data of the constant buffer is the 4x4 world-to-project matrix of the camera. We need to add a new include file to use matrix types:

```c++
#include <Runtime/Math/Matrix.hpp>
```

then we can use the following code to create constant buffer:

```c++
auto cb_align = dev->get_constant_buffer_data_alignment();
luset(cb, dev->new_resource(ResourceDesc::buffer(ResourceHeapType::upload, ResourceUsageFlag::constant_buffer, align_upper(sizeof(Float4x4), cb_align))));
```

as you can see, `Float4x4` is the matrix type used in Luna SDK. We also have `Float3x3` for 2D affine transformations.

## Loading image from file

The next step is to load our Luna LOGO image that will be drawn on the box surface:

![](getting_started/luna.png)

Save the image file in the same directory as `main.cpp`, and naming it `luna.png`. You should have one file structure similar to this:

```c++
DemoApp
|- xmake.lua
|- main.cpp
|- luna.png
```

Then fills `xmake.lua` with the following code:

```
target("DemoApp")
    set_luna_program()
    add_headerfiles("**.hpp")
    add_files("**.cpp")
    add_deps("Runtime", "Window", "RHI", "ShaderCompiler", "Image")
    before_build(function(target)
        os.cp("$(scriptdir)/luna.png", target:targetdir() .. "/luna.png")
    end)
    after_install(function (target)
        os.cp(target:targetdir() .. "/luna.png", target:installdir() .. "/bin/luna.png")
    end)
target_end()
```

This script triggers registers custom functions before building the program and after installing the program, the custom function copies the image file to same the directory of our program binary file, so that our program can correctly find the image file.

We firstly need to add one new property to `DemoApp` to represent the loaded image:

```c++
Ref<RHI::IResource> file_tex;
```

To load the image in our program, we need to use one new module called `Image`, which parses image file data and gives row-majored image data in our desired format. We also need to use the file API provided by `Runtime` module, so we includes two new headers:

```c++
#include <Runtime/File.hpp>
#include <Image/Image.hpp>
```

The first thing to do is to load image file data from our `luna.png` file. In order to load file data, we need to use the `open_file` function provided by the `Runtime` module. This function returns one file handle represented by `IFile` if the file is correctly opened. Then, we loads the file data into one `Blob` object by calling `load_file_data`, this function creates one properly-sized blob object, and calls `IFile::read` to read all data of the file to the blob, then returns the blob:

```c++
lulet(image_file, open_file("Luna.png", FileOpenFlag::read, FileCreationMode::open_existing));
lulet(image_file_data, load_file_data(image_file));
```

Now that the file data has been stored in `image_file_data`, we need to call `Image::read_image_file` function to parse the file data and gives the real image data:

```c++
Image::ImageDesc image_desc;
lulet(image_data, Image::read_image_file(image_file_data.data(), image_file_data.size(), Image::ImagePixelFormat::rgba8_unorm, image_desc));
```

`Image::read_image_file` function outputs one `Image::ImageDesc` structure that describes the returned image data, including the width, height and pixel format of the image. The image data is arranged in a row-major manner and without and alignment padding. We then creates one new resource, and uploads the data to the resource:

```c++
luset(file_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::shared_upload, Format::rgba8_unorm, 
    ResourceUsageFlag::shader_resource, image_desc.width, image_desc.height, 1, 1)));
luexp(file_tex->map_subresource(0, false));
luexp(file_tex->write_subresource(0, image_data.data(), 
    image_desc.width * Image::pixel_size(image_desc.format), 
    image_desc.width * image_desc.height * Image::pixel_size(image_desc.format), BoxU(0, 0, 0, image_desc.width, image_desc.height, 1)));
file_tex->unmap_subresource(0, true);
```

 Note that for texture resources, we cannot fetch pointers to the mapped data and copy data directly using `memcpy` like those in buffer resources. Instead, we need to call `IResource::write_subresource` after `IResource::map_subresource` to let the system copy data to the resource memory. The resource is created in `shared_upload` heap, which is the common option for resources whose data will be loaded from file.

## Set up descriptor set

Once the constant buffer and file texture is set up, we can bind these two resources to the descriptor set that we need to bind to the pipeline state later. We also need to set the sampler in the descriptor set to be used by the pixel shader.

```c++
desc_set->set_cbv(0, cb, ConstantBufferViewDesc(0, align_upper(sizeof(Float4x4), cb_align)));
desc_set->set_srv(1, file_tex);
desc_set->set_sampler(2, SamplerDesc(FilterMode::min_mag_mip_linear, TextureAddressMode::clamp,
				TextureAddressMode::clamp, TextureAddressMode::clamp, 0.0f, 1, ComparisonFunc::always, 
                Float4U(0, 0, 0, 0), 0.0f, 0.0f));
```

This concludes the `DemoApp::init` function.

## Camera control

Now that we have created all resources required to draw the box, we need to fill the actual drawing code in `DemoApp::update`. To make our program more interesting, we can apply one simple animation that rotates the camera around the box. We firstly adds one new property to `DemoApp` that stores the rotation angle of the camera:

```c++
f32 camera_rotation = 0.0f;
```

We can increase the rotation angle of the camera by one at every frame by adding the following line to the end of `DemoApp:update`:

```c++
camera_rotation += 1.0f;
```

Since we are going to use many functions that may throw errors, it is better to declare one `lutry`-`lucatch` scope that wraps all succeeding codes in `DemoApp:update`:

```c++
RV DemoApp::update()
{
    Window::poll_events();
    if(window->is_closed()) return ok;
    lutry
    {
        camera_rotation += 1.0f;
        // More codes goes here...
    }
    lucatchret;
    return ok;
}
```

After we updates the camera rotation, we need to calculate the view-projection matrix for the camera. Fortunately, the math library of the `Runtime` module already includes implementations for many commonly used vector and matrix calculations, and here we are going to use two of them: `AffineMatrix3D::make_look_at` and `perspective_projection_fov`:

```c++
Float3 camera_pos(cosf(camera_rotation / 180.0f * PI) * 2.0f, 1.0f, sinf(camera_rotation / 180.0f * PI) * 2.0f);
Float4x4 camera_mat = AffineMatrix3D::make_look_at(camera_pos, Float3(0, 0, 0), Float3(0, 1, 0));
auto window_sz = window->get_framebuffer_size();
camera_mat = mul(camera_mat, perspective_projection_fov(PI / 3.0f, (f32)window_sz.x / (f32)window_sz.y, 0.001f, 100.0f));
```

The `AffineMatrix3D` namespace includes common functions for generating and decomposing 3D affine matrices. In our example, `AffineMatrix3D::make_look_at` generates one camera view matrix from the position of the camera and the position of the point to look at. `perspective_projection_fov` is another helper function that generates one projection matrix from the specified field-of-view and aspect ratio values. Those two matrices are multiplied by `mul` function to get the final view-projection matrix. Note that when performing matrix multiplications, use `mul` instead of operator `*`, the later one is used to multiply each element in the matrix separately.

After we get the matrix, we can upload the matrix data to our constant buffer using the syntax similar to those for vertex and index buffers:

```c++
void* camera_mapped;
luexp(cb->map_subresource(0, false, &camera_mapped));
memcpy(camera_mapped, &camera_mat, sizeof(Float4x4));
cb->unmap_subresource(0, true);
```

## Resource barriers

In Luna SDK, every graphic resource has one state that describes the current memory layout and pipeline access polity of the resource. Before we can issue draw calls, we need to transfer every resource we use to their correct states. Luna SDK requires the user to transfer the state explicitly by calling `ICommandBuffer::resource_barriers` with transition-typed resource barriers. In our example, we need to perform the following transitions:

```c++
cmdbuf->resource_barriers({
    ResourceBarrierDesc::as_transition(cb, ResourceState::vertex_and_constant_buffer),
    ResourceBarrierDesc::as_transition(vb, ResourceState::vertex_and_constant_buffer),
    ResourceBarrierDesc::as_transition(ib, ResourceState::index_buffer),
    ResourceBarrierDesc::as_transition(file_tex, ResourceState::shader_resource_pixel),
    ResourceBarrierDesc::as_transition(rt_tex, ResourceState::render_target),
    ResourceBarrierDesc::as_transition(depth_tex, ResourceState::depth_stencil_write)
});
```

Luna SDK internally manages the current state for all resources, so we only need to specify the state of the resource **after** the transition. Luna SDK also omits unnecessary transitions automatically if the before and after state of one resource is same or compatible.

## Drawing the box

Finally, we can issue the draw call that draws our box:

```c++
RenderPassDesc desc;
desc.rtvs[0] = rtv;
desc.rt_load_ops[0] = LoadOp::clear;
desc.rt_store_ops[0] = StoreOp::store;
desc.rt_clear_values[0] = {0, 0, 0, 0};
desc.dsv = dsv;
desc.depth_load_op = LoadOp::clear;
desc.depth_store_op = StoreOp::store;
desc.depth_clear_value = 1.0f;
desc.stencil_load_op = LoadOp::dont_care;
desc.stencil_store_op = StoreOp::dont_care;
cmdbuf->begin_render_pass(desc);
cmdbuf->set_graphic_shader_input_layout(slayout);
cmdbuf->set_pipeline_state(pso);
cmdbuf->set_graphic_descriptor_set(0, desc_set);
cmdbuf->set_primitive_topology(PrimitiveTopology::triangle_list);
auto sz = vb->get_desc().width_or_buffer_size;
cmdbuf->set_vertex_buffers(0, {VertexBufferViewDesc(vb, 0, sz, sizeof(Vertex))});
sz = ib->get_desc().width_or_buffer_size;
cmdbuf->set_index_buffer(ib, 0, sz, Format::r32_uint);
cmdbuf->set_scissor_rect(RectI(0, 0, (i32)window_sz.x, (i32)window_sz.y));
cmdbuf->set_viewport(Viewport(0.0f, 0.0f, (f32)window_sz.x, (f32)window_sz.y, 0.0f, 1.0f));
cmdbuf->draw_indexed(36, 0, 0);
cmdbuf->end_render_pass();
```

The first thing to do is to begin a *render pass* that attaches one set of render targets and/or the depth stencil target to the graphic pipeline, these render resources are bound to the pipeline during the current render pass and cannot be changed, while all other settings (like shader input layout object, pipeline state object, descriptor sets, etc) can be changed within the same render pass.

The render pass begins with `ICommandBuffer::begin_render_pass`. In the render pass, we set up all pipeline settings, and bind all resources required for the current draw call, then calls `ICommandBuffer::draw_indexed` to issue the draw call based on the current settings. Then we should close the render pass by calling `ICommandBuffer::end_render_pass`. We won't go detail about the pipeline setup for this draw call, they should be familiar to you if you have been using other graphics API before. For further explanations, please consult the documentations for the `RHI` module.

As we have said before, commands in the command buffer will not be executed immediately, they should be submitted to the command queue explicitly to get executed. So we do it here:

```c++
luexp(cmdbuf->submit());
```

This transfers the command buffer to the execution state, so we can no longer adding commands to the command buffer until we reset the command buffer using `ICommandBuffer::reset`.

## Presenting the render result

The last thing is to present our rendering result to the window (or precisely, the back buffer in the window swap chain), and this is done by calling `ISwapChain::presnet`:

```c++
luexp(swap_chain->present(rt_tex, 0, 1));
```

The first two parameters are the texture resource and subresource id to get displayed, and the system will blit the texture to the back buffer. For compatibility reasons, the user cannot fetch the back buffer directly like in other graphic APIs, this will bring one extra blit overhead on some platforms, but it won't be the bottleneck of your program for most cases.

In Luna SDK, the present call is not synchronous, it only pushes the present command into the bounding command queue and returns directly. We should explicitly wait for the present command to be finished by calling `ISwapChain::wait` before we can start the next frame:

```c++
swap_chain->wait();
```

Since we submitted the command buffer before the present call, when the present command is finished, the command buffer is guaranteed to be finished, so that we don't need to call `cmdbuf->wait()` explicitly and can reset the command buffer safely now:

```c++
luexp(cmdbuf->reset());
```

This concludes the `DemoApp::update` function. Build and run `DemoApp`, if everything goes correctly, you will see a textured rotating box in the screen:

![](getting_started/DemoApp-final.png)

The complete code for `main.cpp` is here for your reference:

```c++
#include <Runtime/Runtime.hpp>
#include <Runtime/Module.hpp>
#include <Runtime/Debug.hpp>
#include <Window/Window.hpp>
#include <RHI/RHI.hpp>
#include <ShaderCompiler/ShaderCompiler.hpp>
#include <RHI/ShaderCompileHelper.hpp>
#include <Runtime/Math/Matrix.hpp>
#include <Runtime/File.hpp>
#include <Image/Image.hpp>
#include <Runtime/Math/Transform.hpp>

using namespace Luna;

struct DemoApp
{
    Ref<Window::IWindow> window;

    Ref<RHI::IDevice> dev;
    Ref<RHI::ICommandQueue> queue;
    Ref<RHI::ICommandBuffer> cmdbuf;
    Ref<RHI::ISwapChain> swap_chain;
    Ref<RHI::IDescriptorSetLayout> dlayout;
    Ref<RHI::IDescriptorSet> desc_set;
    Ref<RHI::IShaderInputLayout> slayout;
    Ref<RHI::IPipelineState> pso;
    Ref<RHI::IResource> rt_tex;
    Ref<RHI::IRenderTargetView> rtv;
    Ref<RHI::IResource> depth_tex;
    Ref<RHI::IDepthStencilView> dsv;
    Ref<RHI::IResource> vb;
    Ref<RHI::IResource> ib;
    Ref<RHI::IResource> cb;

    Ref<RHI::IResource> file_tex;

    f32 camera_rotation = 0.0f;

    RV init();
    RV update();
    bool is_exiting();
    RV resize(u32 width, u32 height);
};

DemoApp* g_app = nullptr;

struct Vertex
{
    Float3U position;
    Float2U texcoord;
};

RV DemoApp::init()
{
    lutry
    {
        luset(window, Window::new_window("DemoApp", 0, 0, 0, 0, nullptr, 
            Window::WindowCreationFlag::default_size | Window::WindowCreationFlag::position_center |
            Window::WindowCreationFlag::minimizable | Window::WindowCreationFlag::maximizable |
            Window::WindowCreationFlag::resizable));
        window->get_close_event() += [](Window::IWindow* window) { window->close(); };
        window->get_framebuffer_resize_event() += [](Window::IWindow* window, u32 width, u32 height) {
            lupanic_if_failed(g_app->resize(width, height));
        };

        dev = RHI::get_main_device();
        using namespace RHI;
        luset(queue, dev->new_command_queue(CommandQueueType::graphic));
        luset(cmdbuf, queue->new_command_buffer());
        luset(swap_chain, new_swap_chain(queue, window, SwapChainDesc(0, 0, Format::rgba8_unorm, 2)));

        luset(dlayout, dev->new_descriptor_set_layout(DescriptorSetLayoutDesc({
            {DescriptorType::cbv, 0, 1, ShaderVisibility::vertex},
            {DescriptorType::srv, 1, 1, ShaderVisibility::pixel},
            {DescriptorType::sampler, 2, 1, ShaderVisibility::pixel}
        })));
        luset(desc_set, dev->new_descriptor_set(DescriptorSetDesc(dlayout)));

        const char vs_shader_code[] = R"(
        cbuffer vertexBuffer : register(b0)
        {
            float4x4 world_to_proj;
        };
        struct VS_INPUT
        {
            float3 position : POSITION;
            float2 texcoord : TEXCOORD;
        };
        struct PS_INPUT
        {
            float4 position : SV_POSITION;
            float2 texcoord : TEXCOORD;
        };
        PS_INPUT main(VS_INPUT input)
        {
            PS_INPUT output;
            output.position = mul(world_to_proj, float4(input.position, 1.0f));
            output.texcoord = input.texcoord;
            return output;
        })";
        
        const char ps_shader_code[] = R"(
        Texture2D tex : register(t1);
        SamplerState tex_sampler : register(s2);
        struct PS_INPUT
        {
            float4 position : SV_POSITION;
            float2 texcoord : TEXCOORD;
        };
        float4 main(PS_INPUT input) : SV_Target
        {
            return float4(tex.Sample(tex_sampler, input.texcoord));
        })";
        auto compiler = ShaderCompiler::new_compiler();
		compiler->set_source({ vs_shader_code, strlen(vs_shader_code)});
		compiler->set_source_name("DemoAppVS");
		compiler->set_entry_point("main");
		compiler->set_target_format(RHI::get_current_platform_shader_target_format());
		compiler->set_shader_type(ShaderCompiler::ShaderType::vertex);
		compiler->set_shader_model(5, 0);
		compiler->set_optimization_level(ShaderCompiler::OptimizationLevel::full);
		luexp(compiler->compile());
		auto vs_data = compiler->get_output();
		Blob vs(vs_data.data(), vs_data.size());

        compiler->reset();
		compiler->set_source({ ps_shader_code, strlen(ps_shader_code)});
		compiler->set_source_name("DemoAppPS");
		compiler->set_entry_point("main");
		compiler->set_target_format(RHI::get_current_platform_shader_target_format());
		compiler->set_shader_type(ShaderCompiler::ShaderType::pixel);
		compiler->set_shader_model(5, 0);
		compiler->set_optimization_level(ShaderCompiler::OptimizationLevel::full);
		luexp(compiler->compile());
		auto ps_data = compiler->get_output();
		Blob ps(ps_data.data(), ps_data.size());

        luset(slayout, dev->new_shader_input_layout(ShaderInputLayoutDesc({dlayout}, 
            ShaderInputLayoutFlag::allow_input_assembler_input_layout |
            ShaderInputLayoutFlag::deny_hull_shader_access |
            ShaderInputLayoutFlag::deny_domain_shader_access |
            ShaderInputLayoutFlag::deny_geometry_shader_access)));
        GraphicPipelineStateDesc ps_desc;
		ps_desc.primitive_topology_type = PrimitiveTopologyType::triangle;
		ps_desc.sample_mask = U32_MAX;
		ps_desc.sample_quality = 0;
		ps_desc.blend_state = BlendDesc(false, false, { RenderTargetBlendDesc(false, false, BlendFactor::src_alpha,
			BlendFactor::inv_src_alpha, BlendOp::add, BlendFactor::inv_src_alpha, BlendFactor::zero, BlendOp::add, LogicOp::noop, ColorWriteMask::all) });
		ps_desc.rasterizer_state = RasterizerDesc(FillMode::solid, CullMode::back, 0, 0.0f, 0.0f, 0, false, true, false, false, false);
		ps_desc.depth_stencil_state = DepthStencilDesc(true, true, ComparisonFunc::less_equal, false, 0x00, 0x00, DepthStencilOpDesc(), DepthStencilOpDesc());
		ps_desc.ib_strip_cut_value = IndexBufferStripCutValue::disabled;
		ps_desc.input_layout = InputLayoutDesc({
            {"POSITION", 0, Format::rgb32_float},
            {"TEXCOORD", 0, Format::rg32_float},
        });
		ps_desc.vs = vs.cspan();
		ps_desc.ps = ps.cspan();
		ps_desc.shader_input_layout = slayout;
		ps_desc.num_render_targets = 1;
		ps_desc.rtv_formats[0] = Format::rgba8_unorm;
		ps_desc.dsv_format = Format::d32_float;
        luset(pso, dev->new_graphic_pipeline_state(ps_desc));
        
        auto window_size = window->get_framebuffer_size();
        luset(rt_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::rgba8_unorm, 
            ResourceUsageFlag::shader_resource | ResourceUsageFlag::render_target, window_size.x, window_size.y, 1, 1)));
        luset(depth_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::d32_float, 
            ResourceUsageFlag::depth_stencil, window_size.x, window_size.y, 1, 1)));
        luset(rtv, dev->new_render_target_view(rt_tex));
        luset(dsv, dev->new_depth_stencil_view(depth_tex));

        Vertex vertices[] = {
            {{+0.5, -0.5, -0.5}, {0.0, 1.0}}, {{+0.5, +0.5, -0.5}, {0.0, 0.0}},
            {{+0.5, +0.5, +0.5}, {1.0, 0.0}}, {{+0.5, -0.5, +0.5}, {1.0, 1.0}},

            {{+0.5, -0.5, +0.5}, {0.0, 1.0}}, {{+0.5, +0.5, +0.5}, {0.0, 0.0}},
            {{-0.5, +0.5, +0.5}, {1.0, 0.0}}, {{-0.5, -0.5, +0.5}, {1.0, 1.0}},

            {{-0.5, -0.5, +0.5}, {0.0, 1.0}}, {{-0.5, +0.5, +0.5}, {0.0, 0.0}},
            {{-0.5, +0.5, -0.5}, {1.0, 0.0}}, {{-0.5, -0.5, -0.5}, {1.0, 1.0}},

            {{-0.5, -0.5, -0.5}, {0.0, 1.0}}, {{-0.5, +0.5, -0.5}, {0.0, 0.0}},
            {{+0.5, +0.5, -0.5}, {1.0, 0.0}}, {{+0.5, -0.5, -0.5}, {1.0, 1.0}},

            {{-0.5, +0.5, -0.5}, {0.0, 1.0}}, {{-0.5, +0.5, +0.5}, {0.0, 0.0}},
            {{+0.5, +0.5, +0.5}, {1.0, 0.0}}, {{+0.5, +0.5, -0.5}, {1.0, 1.0}},

            {{+0.5, -0.5, -0.5}, {0.0, 1.0}}, {{+0.5, -0.5, +0.5}, {0.0, 0.0}},
            {{-0.5, -0.5, +0.5}, {1.0, 0.0}}, {{-0.5, -0.5, -0.5}, {1.0, 1.0}}
        };
        u32 indices[] = {
            0, 1, 2, 0, 2, 3, 
            4, 5, 6, 4, 6, 7, 
            8, 9, 10, 8, 10, 11,
            12, 13, 14, 12, 14, 15,
            16, 17, 18, 16, 18, 19,
            20, 21, 22, 20, 22, 23
        };
        luset(vb, dev->new_resource(ResourceDesc::buffer(ResourceHeapType::shared_upload, ResourceUsageFlag::vertex_buffer, sizeof(vertices))));
        luset(ib, dev->new_resource(ResourceDesc::buffer(ResourceHeapType::shared_upload, ResourceUsageFlag::index_buffer, sizeof(indices))));
        void* mapped = nullptr;
        luexp(vb->map_subresource(0, false, &mapped));
        memcpy(mapped, vertices, sizeof(vertices));
        vb->unmap_subresource(0, true);
        luexp(ib->map_subresource(0, false, &mapped));
        memcpy(mapped, indices, sizeof(indices));
        ib->unmap_subresource(0, true);
        auto cb_align = dev->get_constant_buffer_data_alignment();
        luset(cb, dev->new_resource(ResourceDesc::buffer(ResourceHeapType::upload, ResourceUsageFlag::constant_buffer, align_upper(sizeof(Float4x4), cb_align))));

        lulet(image_file, open_file("Luna.png", FileOpenFlag::read, FileCreationMode::open_existing));
        lulet(image_file_data, load_file_data(image_file));
        Image::ImageDesc image_desc;
        lulet(image_data, Image::read_image_file(image_file_data.data(), image_file_data.size(), Image::ImagePixelFormat::rgba8_unorm, image_desc));

        luset(file_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::shared_upload, Format::rgba8_unorm, 
            ResourceUsageFlag::shader_resource, image_desc.width, image_desc.height, 1, 1)));
        luexp(file_tex->map_subresource(0, false));
        luexp(file_tex->write_subresource(0, image_data.data(), 
            image_desc.width * Image::pixel_size(image_desc.format), 
            image_desc.width * image_desc.height * Image::pixel_size(image_desc.format), BoxU(0, 0, 0, image_desc.width, image_desc.height, 1)));
        file_tex->unmap_subresource(0, true);

        desc_set->set_cbv(0, cb, ConstantBufferViewDesc(0, align_upper(sizeof(Float4x4), cb_align)));
        desc_set->set_srv(1, file_tex);
        desc_set->set_sampler(2, SamplerDesc(FilterMode::min_mag_mip_linear, TextureAddressMode::clamp,
				TextureAddressMode::clamp, TextureAddressMode::clamp, 0.0f, 1, ComparisonFunc::always, 
                Float4U(0, 0, 0, 0), 0.0f, 0.0f));
        
    }
    lucatchret;
    return ok;
}
RV DemoApp::update()
{
    Window::poll_events();
    if(window->is_closed()) return ok;
    lutry
    {
        camera_rotation += 1.0f;
        Float3 camera_pos(cosf(camera_rotation / 180.0f * PI) * 2.0f, 1.0f, sinf(camera_rotation / 180.0f * PI) * 2.0f);
        Float4x4 camera_mat = AffineMatrix3D::make_look_at(camera_pos, Float3(0, 0, 0), Float3(0, 1, 0));
        auto window_sz = window->get_framebuffer_size();
        camera_mat = mul(camera_mat, perspective_projection_fov(PI / 3.0f, (f32)window_sz.x / (f32)window_sz.y, 0.001f, 100.0f));
        void* camera_mapped;
        luexp(cb->map_subresource(0, false, &camera_mapped));
        memcpy(camera_mapped, &camera_mat, sizeof(Float4x4));
        cb->unmap_subresource(0, true);

        using namespace RHI;

        cmdbuf->resource_barriers({
            ResourceBarrierDesc::as_transition(cb, ResourceState::vertex_and_constant_buffer),
            ResourceBarrierDesc::as_transition(vb, ResourceState::vertex_and_constant_buffer),
            ResourceBarrierDesc::as_transition(ib, ResourceState::index_buffer),
            ResourceBarrierDesc::as_transition(file_tex, ResourceState::shader_resource_pixel),
            ResourceBarrierDesc::as_transition(rt_tex, ResourceState::render_target),
            ResourceBarrierDesc::as_transition(depth_tex, ResourceState::depth_stencil_write)
        });

        RenderPassDesc desc;
        desc.rtvs[0] = rtv;
        desc.rt_load_ops[0] = LoadOp::clear;
        desc.rt_store_ops[0] = StoreOp::store;
        desc.rt_clear_values[0] = {0, 0, 0, 0};
        desc.dsv = dsv;
        desc.depth_load_op = LoadOp::clear;
        desc.depth_store_op = StoreOp::store;
        desc.depth_clear_value = 1.0f;
        desc.stencil_load_op = LoadOp::dont_care;
        desc.stencil_store_op = StoreOp::dont_care;
        cmdbuf->begin_render_pass(desc);
        cmdbuf->set_graphic_shader_input_layout(slayout);
        cmdbuf->set_pipeline_state(pso);
        cmdbuf->set_graphic_descriptor_set(0, desc_set);
        cmdbuf->set_primitive_topology(PrimitiveTopology::triangle_list);
        auto sz = vb->get_desc().width_or_buffer_size;
        cmdbuf->set_vertex_buffers(0, {VertexBufferViewDesc(vb, 0, sz, sizeof(Vertex))});
        sz = ib->get_desc().width_or_buffer_size;
        cmdbuf->set_index_buffer(ib, 0, sz, Format::r32_uint);
        cmdbuf->set_scissor_rect(RectI(0, 0, (i32)window_sz.x, (i32)window_sz.y));
        cmdbuf->set_viewport(Viewport(0.0f, 0.0f, (f32)window_sz.x, (f32)window_sz.y, 0.0f, 1.0f));
        cmdbuf->draw_indexed(36, 0, 0);
        cmdbuf->end_render_pass();

        luexp(cmdbuf->submit());
        luexp(swap_chain->present(rt_tex, 0, 1));
        swap_chain->wait();
        luexp(cmdbuf->reset());
    }
    lucatchret;
    return ok;
}
bool DemoApp::is_exiting()
{
    return window->is_closed();
}
RV DemoApp::resize(u32 width, u32 height)
{
    lutry
    {
        using namespace RHI;
        auto dev = get_main_device();
        luexp(swap_chain->resize_buffers(2, width, height, Format::rgba8_unorm));
        luset(rt_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::rgba8_unorm, 
            ResourceUsageFlag::shader_resource | ResourceUsageFlag::render_target, width, height, 1, 1)));
        luset(depth_tex, dev->new_resource(ResourceDesc::tex2d(ResourceHeapType::local, Format::d32_float, 
            ResourceUsageFlag::depth_stencil, width, height, 1, 1)));
        luset(rtv, dev->new_render_target_view(rt_tex));
        luset(dsv, dev->new_depth_stencil_view(depth_tex));
    }
    lucatchret;
    return ok;
}
RV run_app()
{
    auto result = init_modules();
    if(failed(result)) return result;
    g_app = memnew<DemoApp>();
    result = g_app->init();
    if(failed(result)) return result;
    while(!g_app->is_exiting())
    {
        result = g_app->update();
        if(failed(result)) return result;
    }
    return ok;
}
int main()
{
    bool initialized = Luna::init();
    if(!initialized) return -1;
    RV result = run_app();
    if(failed(result)) debug_printf(explain(result.errcode()));
    if(g_app) memdelete(g_app);
    Luna::close();
    return 0;
}
```

## Where should I go next?

Congratulations! If you have followed every step of this article, you should have a first impression of graphic programming using Luna SDK. If you have any question on the concepts and codes in this article, please leave comments below, so that we can improve this article to make it more clear for you.

To go deeper into Luna SDK, we suggest you to read the technical documentations for modules you are interested in (like `Runtime`, `RHI`, etc.), where we discusses not only the functionalities of the module, but also the design considerations of such functionalities. Since the documentation is still being constructed and may not be comprehensive, if you cannot find what you are looking for in the documentation, we also suggest you to check the header file of the module (files not in the `Source` folder of the module root directory), since most module interfaces are pretty well documented in the header files.

That's all of this article, thanks again for using Luna SDK.

 

