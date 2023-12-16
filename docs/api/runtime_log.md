# Logging
## Alias types
* [using log_callback_t =  void(LogVerbosity verbosity, const c8* tag, usize tag_length, const c8* message, usize message_length)](group___runtime_log_1ga4f5add77207e2a4582c82b8a9c85e4e1.md)

    Called by the log system when one log is emitted. 

## Functions
* [void log(LogVerbosity verbosity, const c8 *tag, const c8 *format,...)](group___runtime_log_1ga4b5683a95a7118bcfc3203ddcde34d07.md)

    Logs one message. 

* [void logv(LogVerbosity verbosity, const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gae6c1798bbd5446a133100e8ebc283ca2.md)

    Logs one message. 

* [void log_verbose(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga38e60462c76c37f69f150f44704fe328.md)

    Outputs one log message with LogVerbosity::verbose verbosity. 

* [void logv_verbose(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gacadef67504280ec6bb3adb3347f493b3.md)

    Outputs one log message with LogVerbosity::verbose verbosity. 

* [void log_debug(const c8 *tag, const c8 *format,...)](group___runtime_log_1gadae5c40552d5fd5cd14f5d2f0cf1ef50.md)

    Outputs one log message with LogVerbosity::debug verbosity. 

* [void logv_debug(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gaa4eba0bfec55c87b90fac20154972ea7.md)

    Outputs one log message with LogVerbosity::debug verbosity. 

* [void log_info(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga8d79a7c1bad5288fbae2957a393571a8.md)

    Outputs one log message with LogVerbosity::info verbosity. 

* [void logv_info(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1ga1959851d7f6c95a7ff4a9f1299d8c320.md)

    Outputs one log message with LogVerbosity::info verbosity. 

* [void log_warning(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga879252fc6b5710591017dedcf8477ab6.md)

    Outputs one log message with LogVerbosity::warning verbosity. 

* [void logv_warning(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gaf09ca29af954d9c57fec7ecdddd965fa.md)

    Outputs one log message with LogVerbosity::warning verbosity. 

* [void log_error(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga5d0a6cff8f2359b2333c51cf0fe43fc2.md)

    Outputs one log message with LogVerbosity::error verbosity. 

* [void logv_error(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1ga54dd6e067a62bf7bd9ce394ce33af1a4.md)

    Outputs one log message with LogVerbosity::error verbosity. 

* [usize register_log_handler(const Function< log_callback_t > &handler)](group___runtime_log_1ga076012c7d4f86dbc45b773737f3a7048.md)

    Registers one custom log handler that will be called when a new log message is spawned. 

* [void unregister_log_handler(usize handler_id)](group___runtime_log_1ga35f89e378c4ca67c543136b5517a8276.md)

    Unregisters one registered log handler. 

* [void set_log_to_platform_enabled(bool enabled)](group___runtime_log_1ga6ce512bc6294c3f095431120d68f4c9d.md)

    Enables or disables outputting log messages to platform's default logging device. 

* [void set_log_to_platform_verbosity(LogVerbosity verbosity)](group___runtime_log_1gad74a8925848e1f43dca786eb32d8a151.md)

    Sets the maximum log verbosity level that will be outputted to platform's default logging device. 

* [void set_log_to_file_enabled(bool enabled)](group___runtime_log_1gad9e21a84299dda0f2f44d176e76d8132.md)

    Enables or disables outputting log messages to the log file. 

* [void set_log_file(const c8 *file)](group___runtime_log_1ga1d07b29664bc23bd9477ed5005c2b181.md)

    Sets the file path of the log file. 

* [void set_log_to_file_verbosity(LogVerbosity verbosity)](group___runtime_log_1ga988ebb856716ebcf6ce5538418cf2f1a.md)

    Sets the maximum log verbosity level that will be outputted to the log file. 

* [void flush_log_to_file()](group___runtime_log_1ga9e47467e3cae737a4160a169667a6399.md)

    Flushes the log-to-file cache and writes all cached logs to the log file. 

