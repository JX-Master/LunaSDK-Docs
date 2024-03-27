# RHI Errors
## Functions
* [ErrCode device_hung()](group___r_h_i_error_1gaf6b718f84ca3c5b465498a6477b64560.md)

    The application's device failed due to badly formed commands sent by the application. This is an design-time issue that should be investigated and fixed. 

* [ErrCode device_reset()](group___r_h_i_error_1ga34693f298731b914347fa56745c4150b.md)

    The device failed due to a badly formed command. This is a run-time issue; The application should destroy and recreate the device. 

* [ErrCode device_removed()](group___r_h_i_error_1gafcd8fcbbe1e976e2d9a4ef205202180e.md)

    The video card has been physically removed from the system, or a driver upgrade for the video card has occurred. The application should destroy and recreate the device. Sending badly formed commands to the device will also cause device being (virtually) removed from the application. 

* [ErrCode driver_internal_error()](group___r_h_i_error_1gad6d7047edfd6265ad91591e193372a30.md)

    The driver encountered a problem and was put into the device removed state. 

* [ErrCode frame_statistics_disjoint()](group___r_h_i_error_1ga83f768c1b8643a04135fec220d1625a7.md)

    An event (for example, a power cycle) interrupted the gathering of presentation statistics. 

* [ErrCode swap_chain_out_of_date()](group___r_h_i_error_1ga35fdcbc18187e0c9cd75f8f38b96a30d.md)

    The swap chain is no longer compatible with the surface and should be reset. 

