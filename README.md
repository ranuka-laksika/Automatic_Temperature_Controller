# Automatic_Temperature_Controller

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Final_Product.jpg)

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#Project-Overview)
- [Key Features](#Key-Features)
- [Hardware Description:](#hardware-description)
- [Schematic Diagram](#schematic-diagram)
- [PCB Design](#pcb-design)
- [Enclosure Design](#enclosure-design)
- [Testing and Results](#testing-and-result)
- [Conclusion](#conclusion)

## Introduction

The Automatic Temperature Controller project is designed to provide a cost-effective and 
efficient solution for maintaining a comfortable environment by automatically controlling the air 
conditioning system. In modern times, with the increasing need for energy conservation and 
automation, this project offers a practical implementation using the ATmega328P microcontroller 
and the DHT22 temperature and humidity sensor.

## Project Overview

The primary objective of this project is to regulate room temperature within a specified user defined range. To achieve this, we employ the ATmega328P microcontroller, a versatile and 
widely used microcontroller known for its reliability and ease of programming. The DHT22 
sensor is utilized to measure real-time temperature and humidity levels, providing crucial data 
for the controller to make informed decisions.

## Key Features
The key features of the Automatic Temperature Controller project include:
- Temperature Control: The project allows users to set their desired temperature range, 
within which the air conditioning system will maintain the room temperature.
-Energy Efficiency: By automating the air conditioner based on real-time temperature 
data, the project significantly reduces energy waste, making it environmentally friendly 
and cost-effective.
- User-Friendly Interface: The user interface enables simple and intuitive input of 
temperature settings, ensuring ease of use for individuals of all technical backgrounds.
- Expandability: The modular design of the project allows for easy integration of additional 
features, such as remote control or data logging


## Hardware Description
### Product Specifications: 
- Input Voltage : 230V AC frequency: 50Hz 
- Operating Voltage : 5V 
- LCD display : 20 x 4 LCD display (Operating Voltage 5V) 
- Temperature Range : - 40°C to +80°C (DHT22) 
- Humidity Range :- (0 -100)%
- Accuracy of the Temperature sensor : ±0.5°C 
- Key Pad : A standard 4x3 matrix keypad 
- Enclosure Material : PLA 
- Product Dimensions : 160mm x 80mm x 80mm
### Hardware Specification:
#### Microcontroller ( Atmega328p ): 
This is the main control unit of the system, responsible for 
reading the temperature sensor data, controlling the fan through the relay module, and displaying 
the temperature value and the Humidity value on the LCD display. Here use a atmega328p 
microcontroller. 
#### Specifications:-
- Normal operating voltage – 5V
- Operating Temperature: -40°C to 85°C.
- Crystal Oscillator Frequency: Supports external crystal oscillators with 
frequencies from 32kHz to 20MHz; commonly used frequency is 
16MHz.
- Maximum Source/Sink Current: GPIO pins can source or sink up to 
20mA individually, with a total combined limit of 200mA in most cases.
<p align="center">
  <img src="https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Atmega328p_micrcontroller.png" alt="Small Image" width="500" height="500">
</p>

#### 20 x 4 LCD display: 
This display is used to show the current temperature and humidity and the 
user-set temperature range. It has a resolution of 20 x 4 characters. The display is connected to 
the microcontroller

  <p align="center">
  <img src="https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/LCD_Display.png" alt="Small Image" width="500" height="500">
</p>

#### Temperature sensor ( DHT22 ): 
The system uses a digital temperature sensor to measure the 
current room temperature. The temperature sensor should have a range of -40°C to +80°C and a 
temperature accuracy of ±0.5°C.And also this sensor can measure the humidity of the 
environment
 <p align="center">
  <img src="https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/DHT22.png" alt="Small Image" width="500" height="500">
</p>

#### Relay module ( SRD-05VDC-SL-C ): 
This module is used to switch the fan on or off based on 
the temperature readings. It consists of a relay, which can handle AC or DC load and a transistor 
driver circuit to interface with the microcontroller
<p align="center">
  <img src="https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Relay.png" alt="Small Image" width="500" height="500">
</p>

#### Keypad: 
The keypad is used to set the desired temperature value. A standard 4x3 matrix keypad 
can be used for this purpose
<p align="center">
  <img src="https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Keypad.png" alt="Small Image" width="500" height="500">
</p>

### Extra features
Smart Scheduling:
The system can be enhanced with a scheduling feature, which allows the user to set a 
different temperature for each day of the week or for specific time periods during the day. This 
feature can be useful in optimizing energy usage and reducing costs. The scheduling can be done 
through the keypad


## Schematic Diagram

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Schematic_Diagram.png)


### Schematic Diagram of the Power Supply Circuit

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Schematic_Diagram_Power_Supply_Circuit.png)

## PCB Design

### 2D View of the PCB

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/2D-View_of_PCB.png)



### 3D View of the PCB

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/3D-View_of_PCB.png)

## Enclosure Design

### Main part of the Enclosure

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Enclosure_Main_Part_1.png)

### Isometric View of the Enclosure 

![Project Image](https://github.com/ranuka-laksika/Automatic_Temperature_Controller/blob/main/Images/Isometric_View.png)


## Testing and Results

In order to evaluate the Automatic Temperature Controller project's performance, accuracy, and 
user interaction capabilities, thorough testing was conducted. The 3x4 keypad input technique 
was validated during testing, and the output shown on the 20x4 LCD screen was assessed.

#### Test Setup
The test setup remained consistent with the components used in the project:
- ATmega328P microcontroller board
- DHT22 temperature and humidity sensor
- 5V relay module
- Air conditioning unit
- 3x4 keypad for temperature input
- 20x4 LCD display for output

#### Input Testing: Using the 3x4 Keypad
Users were asked to enter the preferred temperature range using the 3x4 keypad during the input 
testing. An easy-to-use interface was provided by the keypad for entering the higher and lower 
temperature criteria. The goal of the test was to check that the system accurately read and 
interpreted the keypad input without any mistakes or discrepancies.
#### Output Testing: 20x4 LCD Display
The objective of the output testing was to confirm the veracity of the data displayed on the 20x4 
LCD panel. The LCD showed current temperature information, humidity readings.
#### Integrated Testing
The entire system was put through integrated testing after individual component testing. The 
system replied by managing the air conditioner and showing the results on the 20x4 LCD based 
on the temperature ranges that users entered using the 3x4 keypad. The goal was to make sure 
that the LCD display, input interface, microcontroller logic, sensor data, and relay control all 
worked together seamlessly.
#### Results

- Input Testing: Using the 3x4 Keypad

The input testing results were positive, showing that the 3x4 keypad was effective in accepting 
user input for defining the temperature range. Users could enter the desired upper and lower 
temperature values easily and accurately.

- Output Testing: 20x4 LCD Display
The output testing revealed that the 20x4 LCD accurately displayed real-time temperature and 
humidity data, as well as the status of the air conditioner. The LCD provided clear and consistent 
information, making it easy for users to monitor the room conditions and the system's response.

- Integrated Testing
The integrated testing demonstrated that the Automatic Temperature Controller operated 
seamlessly as a cohesive system. Users could input temperature values through the 3x4 keypad, 
and the system accurately controlled the air conditioner based on the defined temperature range. 
The 20x4 LCD effectively conveyed the system status and real-time data, ensuring a user friendly and informative experience.

## Conclusion

The Automatic Temperature Controller project is an intelligent solution for maintaining room 
temperature within a user-defined range. Utilizing an ATmega328P microcontroller and DHT22 
temperature and humidity sensor, the system achieves accurate temperature control, prompt 
responsiveness, and substantial energy savings. The 3x4 keypad for user input and 20x4 LCD for 
output display enhance the user experience. The project aims for energy conservation and user 
comfort, reducing energy waste and utility costs. The system's user-friendly interface and easy 
input of desired temperature ranges make it accessible to users of all technical backgrounds. The 
project's modular design allows for future enhancements, such as remote control or data logging 
features. Overall, the Automatic Temperature Controller project showcases the practical 
application of microcontrollers, sensors, and human-machine interfaces in creating a smart and 
eco-friendly temperature regulation system.

