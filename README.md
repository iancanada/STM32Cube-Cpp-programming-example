# STM32Cube-Cpp-programming-example

 * Copyright (C) Ian Jin
 * iancanada.mail@gmail.com
 * https://github.com/iancanada/
 * Twitter: @iancanadaTT

This example will show you how to program STM32 in C++ with STM32 HAL drivers and STM32CubeMX generated code frame.

It's true that STM32Cube can not generate C++ project so far. However, STM32 HAL drivers already have C++ support. So, it's still possible to create C++ code for STM32 based on STM32 HAL drivers and STM32CubeMX generated projects. 

It just needs a couple of steps:

1. Generate a STM32 MDK project normally by STM32CubeMX with most updated HAL drivers.
2. Open project in Keil ARM MDK, change project-option-C/C++ -MiscControls to --cpp
3. Create user C++ files in .hpp and .cpp

This example shows exactly how to do it.

Hardware platform: 

STM32 F4 Discovery board (STM32F407VGT6) 

Software platform:  

Keil ARM MDK V5.05

STM32CubeMX V4.9.0

Files: 

/MDK-ARM/: Keil ARM MDK project

STM32CubeCppExampleF4.ioc: STM32CubeMX project

/Src/LEDcpp.cpp, /Inc/LEDcpp.hpp : C++ LED class for STM32

If four LEDs on STM32 F4 Discovery board toggle respectively every 0.5,1,2,4 seconds, then we are done.

