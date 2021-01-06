# MY3D-F1-SKR-1.4-Turbo
MY3D F1 + SKR 1.4 Turbo modification 

Display MKS_MINI_12864 (this default MY3D F1 display)

Stepper Drivers MC2209


I was able to adapt the native MKS 3d printer display for the skr1.4 turbo. I had to study the pinout of the display and motherboard. And also I managed to rewrite the marlin firmware from skr 1.4 turbo and MY3D F1. 

The one thing to look out for the most is the filament feed rate. I have a non-standard feeder. You will have to fix this for yourself Marlin / Configuration.h #define DEFAULT_AXIS_STEPS_PER_UNIT line 721 and #define DEFAULT_MAX_FEEDRATE line 728.

To be continued.....

![Alt MKS port](images_display/MKS_MINI_12864_port.png?raw=true "MKS MINI 12864 port")

![Alt SKR ports](images_display/SKR_ports.png?raw=true "SKR 1.4 Turbo ports")

![Alt Display](images_display/photo01.jpeg?raw=true "Display test")

![Alt Display](images_display/photo02.jpeg?raw=true "Display mount")



Thingiverse Author page https://www.thingiverse.com/freexmonster/designs.



## Building Marlin 2.0

Additional documentation can be found at the [Marlin Home Page](http://marlinfw.org/).
Please let us know if Marlin misbehaves in any way. Volunteers are standing by!

To build Marlin 2.0 you'll need [Arduino IDE 1.8.8 or newer](https://www.arduino.cc/en/main/software) or [PlatformIO](http://docs.platformio.org/en/latest/ide.html#platformio-ide). Detailed build and install instructions are posted at:

  - [Installing Marlin (Arduino)](http://marlinfw.org/docs/basics/install_arduino.html)
  - [Installing Marlin (VSCode)](http://marlinfw.org/docs/basics/install_platformio_vscode.html).
