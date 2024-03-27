# Luna::RHIError::device_removed

```c++
ErrCode device_removed()
```

The video card has been physically removed from the system, or a driver upgrade for the video card has occurred. The application should destroy and recreate the device. Sending badly formed commands to the device will also cause device being (virtually) removed from the application. 

