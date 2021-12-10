# ROS2 Interfaces for a generic PTU

## Actions

- SetPan: input: float32 pan --> output: bool return; feedback: float32 percentage_of_completing
- SetTilt: input: float32 tilt --> output: bool return; feedback: float32 percentage_of_completing
- SetPanTilt: input: float32 pan, float32 tilt --> output: bool return; feedback: float32 percentage_of_completing for pan and tilt

## Service

- SetPan: input: float32 pan --> output: bool return; 
- SetTilt: input: float32 tilt --> output: bool return; 
- SetPanTilt: input: float32 pan, float32 tilt --> output: bool return; 
- SetPanTiltSpeed: input: float32 pan_speed, float32 tilt_speed --> output: bool return; 
- GetLimits: input: None --> output: float32 pan_min, pan_max, tilt_min, tilt_max

## Messages

- PTU: 
	- Header
	- Pan
	- Tilt
	- PanSpeed
	- TiltSpeed