# thor copter

Top level package for 'thor', running [rosflight](https://github.com/rosflight/rosflight), [roscopter](https://github.com/byu-magicc/roscopter), and [inertial sense](https://github.com/inertialsense/inertial_sense_ros).

`launch/` contains helpful launch files for different use cases you may be running.

`params/` contains thor-specific parameter files. Such as the firmware and vi_ekf parameters used for thor.

## Notes

- If you're using a uINS, make sure to turn on its baro (stream_barm param) and turn off the firmware baro: `rosservice call /param_set STRM_BARO 0`