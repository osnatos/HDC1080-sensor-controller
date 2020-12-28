# HDC1080-sensor-controller
The sensor controller is designed to work with the [HDC1080 sensor](https://www.ti.com/lit/ds/symlink/hdc1080.pdf?ts=1609168968558&ref_url=https%253A%252F%252Fwww.google.com%252F), using the Sensor Controller Engine of CC2640R2F MCU. 
* Project name: HDC1080 sensor 
* Project file: hdc1080_sensor.scp 
* Operating system: TI-RTOS 
* Target chip: CC2640R2F, package QFN48 7x7 RGZ 
* I2C0_SCL - pin 11; I2C0_SDA - pin 10
# How to generate project files.
In order to generate all project files, you must:
* Launch “Sensor Controller Studio” (SCS) using the  hdc1080_sensor.scp project file.
* In the SCS program, click on the “Code Generator” button. SCS will create a scif_files folder (if it did not exist before) and generate all the necessary files in it (except for the readme file).
* The file “scif_hdc1080_how_to_use.html” contains information on using the controller.
# Software tools:
* Sensor Controller Studio v2.7.0.155
# Debugging:
* The project was debugged on the CC2640R2-LAUNCHXL debug board.
# Connection to CC2640R2-LAUNCHXL board:
* HDC1080 / pin1 - SDA / DIO5 + PULUP 10K
* HDC1080 / pin2 - GND
* HDC1080 / pin5 - 3.3V
* HDC1080 / pin6 - SCL / DIO4 + PULUP 10K
# Used in the project:
* The controller was used in the [Beacon_CC2640_with_SensorController_HDC1080](https://github.com/osnatos/Beacon_CC2640_with_SensorController_HDC1080).

