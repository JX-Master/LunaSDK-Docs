# Times
## Functions
* [u64 get_ticks()](group___runtime_time_1ga442af85515e20d45ec4159a7049dab7e.md)

    Queries the ticks of the high-resolution counter of CPU. 

* [f64 get_ticks_per_second()](group___runtime_time_1ga7c8082023e9cd33705e691cf4f2fe55a.md)

    Queries the resolution of high-resolution counter of CPU represented by number of ticks per second. 

* [i64 get_utc_timestamp()](group___runtime_time_1ga8e9742ca3f0a329ad93f3c334490aad2.md)

    Gets the UTC timestamp of the current time. 

* [i64 get_local_timestamp()](group___runtime_time_1ga01462413ce251097096ec9499f644586.md)

    Gets the timestamp of the current time shiftted by the timezone setting of the current platform. 

* [i64 local_timestamp_to_utc_timestamp(i64 local_ts)](group___runtime_time_1ga84750fe01dda3c97a5536bc7eac6c199.md)

    Converts a local timestamp to a UTC timestamp based on the timezone setting of the current platform. 

* [i64 utc_timestamp_to_local_timestamp(i64 utc_ts)](group___runtime_time_1ga5910c042e3f0852cae95f1a83dddd3e2.md)

    Converts a UTC timestamp to a local timestamp based on the timezone setting of the current platform. 

* [DateTime timestamp_to_datetime(i64 timestamp)](group___runtime_time_1ga906130b196c01555fbfe34b989375886.md)

    Converts a timestamp to a calendar date time. 

* [i64 datetime_to_timestamp(const DateTime &datetime)](group___runtime_time_1gaed58ac1534ee8d386cf2ae0e41ba51ef.md)

    Converts a data time structure to a timestamp, without any timezone shift. 

