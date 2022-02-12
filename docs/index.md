# Hardware for ESP IoT Framework

This repository contains the essential Gerber-files or CAD drawings which where utilized for creating a test application of the [ESP-IoT-Framework](https://github.com/ECE-IoT/esp-iot-framework) and the [AWS-IoT-Framework](https://github.com/ECE-IoT/aws-iot-framework)

## Motivation

### Overview

The networking of sensors and actuators via the internet is becoming increasingly important in industry, but also in the private sector. In this project work it will be shown how a processing chain from the sensor to the cloud service (AWS) can be realized practically. The project aims to provide a valuable overview of what is possible with embedded/connected IoT devices that can transmit data to the cloud. In addition, the projects goal was to provide a secure connection to AWS.

!!! attention

    Please be aware that this project is a feasibility study. It does not provide code which is ready for production, or similar. Further information about the future intentions of this project can be found here.

### OpenSource

This project can be accessed via the MIT License. Based upon this license the project team highly encourages people who are keen on getting in touch with embedded IoT applications to contribute to this project.

## PCB Design

The idea of the PCB was to make a simple connection from sensors to the ESP32. Three I2C and one OneWire interfaces were used for the PCB. Most of the sensors can communicate with I2C therefore  a connection with I2C is easy because everything is on a bus and speed is not that important in our case. Pull-up resistors were used for the data lines and Vcc. Male pin headers were used as connectors for the sensors.

![PCB Top](ESP32_PCB.png)
![PCB Bottom](back_ESP32_PCB.png)

## Case

The idea for the case of the PCB was to make a universal use for a realisation of any sensor combination for our application. Threaded inserts were used to mount the PCB/sensors to the housing. 

- M3 for the PCB
- M2.5 for VEML7700, LPS25 and DHT22
- M2 for SCD30

For the cover 2 variations were constructed. A closed one and one a opened one for the light sensor VEML7700. For the connection of cover and housing a simple snap connection was chosen. Grooves were added to the sides of the housing and to the cover to guarantee a sufficient air supply.

![Case](case.png)