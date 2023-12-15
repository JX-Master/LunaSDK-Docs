# Logging
## Aliasing types
* [using log_callback_t =  void(LogVerbosity verbosity, const c8* tag, usize tag_length, const c8* message, usize message_length)](group___runtime_log_1ga4f5add77207e2a4582c82b8a9c85e4e1.md)

    Called by the log system when one log is emitted. 

## Functions
* [LUNA_RUNTIME_API void log(LogVerbosity verbosity, const c8 *tag, const c8 *format,...)](group___runtime_log_1ga350946e90121f9ef51e063e4c5bccc40.md)

    Logs one message. 

* [LUNA_RUNTIME_API void logv(LogVerbosity verbosity, const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gab307215773d74f6206e9f160b981e487.md)

    Logs one message. 

* [LUNA_RUNTIME_API void log_verbose(const c8 *tag, const c8 *format,...)](group___runtime_log_1gafab1bbad31b455c6319d599aff292861.md)

    Outputs one log message with LogVerbosity::verbose verbosity. 

* [LUNA_RUNTIME_API void logv_verbose(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gaa970d47c6a13e8a50336d50bb7718766.md)

    Outputs one log message with LogVerbosity::verbose verbosity. 

* [LUNA_RUNTIME_API void log_debug(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga8ac371f6e8d3004cfee11af8c4a9c792.md)

    Outputs one log message with LogVerbosity::debug verbosity. 

* [LUNA_RUNTIME_API void logv_debug(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1gaab0d7bef3078405ab630732e2a267514.md)

    Outputs one log message with LogVerbosity::debug verbosity. 

* [LUNA_RUNTIME_API void log_info(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga55a28bdf8fba8c2406f1e6c118c29145.md)

    Outputs one log message with LogVerbosity::info verbosity. 

* [LUNA_RUNTIME_API void logv_info(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1ga20e350eaf2b211c77ed8d0a154a68d32.md)

    Outputs one log message with LogVerbosity::info verbosity. 

* [LUNA_RUNTIME_API void log_warning(const c8 *tag, const c8 *format,...)](group___runtime_log_1ga2d44dc9ca61bd03809cbfa07e2536ae3.md)

    Outputs one log message with LogVerbosity::warning verbosity. 

* [LUNA_RUNTIME_API void logv_warning(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1ga7aeedeac2504e537c698bd6a68a9d40d.md)

    Outputs one log message with LogVerbosity::warning verbosity. 

* [LUNA_RUNTIME_API void log_error(const c8 *tag, const c8 *format,...)](group___runtime_log_1gad29d52073dc0b3f7ec0267c3ba03f360.md)

    Outputs one log message with LogVerbosity::error verbosity. 

* [LUNA_RUNTIME_API void logv_error(const c8 *tag, const c8 *format, VarList args)](group___runtime_log_1ga054dbc82fab4901356fbc8a3644de723.md)

    Outputs one log message with LogVerbosity::error verbosity. 

* [LUNA_RUNTIME_API usize register_log_handler(const Function< log_callback_t > &handler)](group___runtime_log_1gaf6e2aabe6a4e4f1a3146dc30146eacf4.md)

    Registers one custom log handler that will be called when a new log message is spawned. 

* [LUNA_RUNTIME_API void unregister_log_handler(usize handler_id)](group___runtime_log_1gaa223d91f158a47f11806bf2c915dc227.md)

    Unregisters one registered log handler. 

* [LUNA_RUNTIME_API void set_log_to_platform_enabled(bool enabled)](group___runtime_log_1ga8d51f2669af7117b5d2ef04818feb092.md)

    Enables or disables outputting log messages to platform's default logging device. 

* [LUNA_RUNTIME_API void set_log_to_platform_verbosity(LogVerbosity verbosity)](group___runtime_log_1ga9cba706488b218d214e0ef4b65c49134.md)

    Sets the maximum log verbosity level that will be outputted to platform's default logging device. 

* [LUNA_RUNTIME_API void set_log_to_file_enabled(bool enabled)](group___runtime_log_1ga5181d848131182ecd7dfe9ce22129712.md)

    Enables or disables outputting log messages to the log file. 

* [LUNA_RUNTIME_API void set_log_file(const c8 *file)](group___runtime_log_1ga26ac527152f3c2e10cb93223d37f00ec.md)

    Sets the file path of the log file. 

* [LUNA_RUNTIME_API void set_log_to_file_verbosity(LogVerbosity verbosity)](group___runtime_log_1ga89a711cfd618825a7139fed0cb10578f.md)

    Sets the maximum log verbosity level that will be outputted to the log file. 

* [LUNA_RUNTIME_API void flush_log_to_file()](group___runtime_log_1ga05f9c48f4ca84328d6ac59079d85b3c5.md)

    Flushes the log-to-file cache and writes all cached logs to the log file. 

