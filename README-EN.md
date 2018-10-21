# Pi_CAR JOYSTICK BOARD

Table of contents
=================
<!--ts-->
   * [1. Overview](#1-overview)
      * [1.1 Goals and Objectives](#11-goals-and-objectives)
   * [2. Block Diagram and PCBs Overview](#2-block-diagram-and-pcbs-overview)
      * [2.1 Transmitter Kit Overview](#21-transmitter-kit-overview)
        * [Top View](#top-view)
        * [Bottom View](#bottom-view)
        * [3D Render Views](#3d-render-views)
      * [2.2 Receive Kit Overview](#22-receive-kit-overview)
        * [Top View](#top-view-1)
        * [Bottom View](#bottom-view-1)
        * [3D Render Views](#3d-render-views-1)
   * [3. Sample Demo Videos](#3-sample-demo-videos)
        * [Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)](#pi_car-joystick-board-with-ros-gazebocustom-joytick-board)
        * [Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board)](#pi_car-joystick-board-with-ros-turtlesim-custom-joytick-board)
        * [Testing of Pi_CAR Joystick Board on Real RC-CAR](#testing-of-pi_car-joystick-board-on-real-rc-car)
<!--te-->

# 1. Overview
&emsp;  It is a development board(**Pi_CAR JOYSTICK BOARD**) designed as a receiver and transmitter circuit for users to develop themselves on **Bluetooth**, **WiFi** and **RF** communication technologies, to make programming fun, and to develop application-oriented learning skills. Arduino IDE's extensive library, fast programming and simplicity, such as support behind many, as the price performance quality of the prominent ESP32 chipset family allows you to evaluate the functionality. This kit (Pi_CAR Communication Card) provides basic hardware (BLE 4.2, WiFi, RF) and software resources that help application developers build their ideas around the ESP32 series hardware (based on the RC-CAR Vehicle control Scenario).The Pi_CAR Communication Card software development framework is designed to develop fast-growing  **Internet of Things (IoT)** applications and  **Robotics (ROS (Robot Operating System))** applications with  **Wi-Fi**,  **Bluetooth**,  **RF**, power management and some other system features.

## 1.1 Goals and Objectives

* Development of ESP32-WROOM-32's structure, function and applications
  * Programming and use of ESP32 with ESP-IDF. (On Eclipse)
  * Programming and use of ESP32 with Arduino IDE
  * Using of Wi-Fi, Bluetooth, Mesh Network, Peripherals (ADC, SPI, UART, TIMER, PWM, GPIO etc...), Storage (MicroSD), System (FreeRTOS, Watchdogs, Over The Air Updates (OTA), High Resolution Timer etc...) on ESP32.
  * Debugging  using GDB
* Learning Bluetooth, WiFi, RF Communication Protocols and Developing Applications
  * Developing Applications with Bluetooth, WiFi, RF
  * Developing TCP, UDP Applications
*  Developing Internet of Things (IoT) Applications
   * Learning MQTT, HTTP Communication Protocols
   * Developing Application with IBM Watson IoT Platform or IVEN Cloud Platform 

*  Developing ROS (Robot Operating System) Applications. 
   * Use and creation of ROS(Robot Operating System)'s structure (Nodes, Topics, Messages, Publisher, Subscriber, Services etc...), libraries, tools.
   * Using of Gazebosim tools, Modelling, simulation and Communication with ROS.<br><br>    
 

  ![overview](https://github.com/zafersn/pi_communition_board/blob/master/img/Block%20Diagram4.png)

# 2. Block Diagram and PCBs Overview

## 2.1 Transmitter Kit Overview
&emsp;Our Pi_CAR Transmitter Card can be used by configuring 2 Thumb Joysticks or 1 Thumb joystick and 4 Tact Switch Buttons.The Tranmitter card enables the connection between the user and the receive card to be approximately 1KM over RF. In addition, it enables the user to communicate with nearby peripherals and develop specific applications via Bluetooth and WiFi connection.(VR, Cloud, Phone App, pc etc...).

Top View
=================
![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board4.png)


Bottom View
=================
![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board_Bttm2.png)

3D Render Views
=================

![Top View render 1](https://github.com/zafersn/pi_communition_board/blob/master/img/1.PNG)

![Top View render 2](https://github.com/zafersn/pi_communition_board/blob/master/img/2.PNG)

![Bottom View render 1](https://github.com/zafersn/pi_communition_board/blob/master/img/2-5.PNG)

![Top View](https://github.com/zafersn/pi_communition_board/blob/master/img/12.png)

![Bottom View](https://github.com/zafersn/pi_communition_board/blob/master/img/10.png)

Piece | Product Name | Description
------------|---------| -------------
1 | ESP32 Joystick Main Board | BLE + WiFi
2 | Thumb Joysticks | 2 Axis Control
4 | Momentary Pushbutton Switch | 12mm 
2 | NRF24L01 | ~1KM Range - Receiver and Transmitter
1 | MikroBUS | Standardized Expansion Card Socket Support  <p>[See: MicroBUS](https://www.mikroe.com/mikrobus)</p>
1 | Micro SD Socket| 
2 | RGB LED 
3 | FPV Power I/O |Separated from the board power circuit.
1 | Power In  | 6V - 18V
1 | Micro USB | Serial to USB converter for programming and communication
1 | JTAG Debugging | for Programming and Debugging
1 |  Board size 99 x 61 mm | Without RF SMA Anten 

## 2.2 Receive Kit Overview
The main purpose of the Pi_CAR Receive card is to communicate with the Transmitter card via NRF24L01.

It is aimed to send the data(Sensors etc..) to the transmitter card from the system where the receiver card(RC-CAR, Drone etc.)  is connected and to perform the necessary operations on the robot by making sense of the data coming from the transmitter card.

Top View
=================
![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/Rx_BOARD.png)

Bottom View
=================
![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/Rx_BOARD_bottom.png)


3D Render Views
=================


![Top View render rx 1](https://github.com/zafersn/pi_communition_board/blob/master/img/4.PNG)

![Top View render rx 2](https://github.com/zafersn/pi_communition_board/blob/master/img/5.PNG)

![Top View](https://github.com/zafersn/pi_communition_board/blob/master/img/15.jpg)


Piece | Product Name | Description
------------|---------| -------------
1 | ESP32 Joystick Main Board | BLE + WiFi
2 | NRF24L01 | ~1KM Range - Receiver and Transmitter
1 | MikroBUS | Standardized Expansion Card Socket Support  <p>[See: MicroBUS](https://www.mikroe.com/mikrobus)</p>
2 | RGB LED 
3 | FPV Power I/O | Separated from the board power circuit.
1 | Power IN | 6V - 18V
1 | Micro USB | Serial to USB converter for programming and communication
1 | JTAG Debugging | For Programming and Debugging
1 | FPV Camera Input |
40| External I / O | PWM/SPI/USART/I2C/GPIO
1 |  Board size 89 x 52 mm | Without RF SMA Anten 
# 3. Sample Demo Videos

Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)
=================

[![Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)](https://img.youtube.com/vi/L5YpyjPOgC0/0.jpg)](https://youtu.be/L5YpyjPOgC0)

Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board)
=================
[![Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board))](https://img.youtube.com/vi/Qxs-DMT6eOg/0.jpg)](https://youtu.be/Qxs-DMT6eOg)

Testing of Pi_CAR Joystick Board on Real RC-CAR
=================
[![Testing of Pi_CAR Communication Board on Real RC-CAR](https://img.youtube.com/vi/O7l2V9Dhggc/0.jpg)](https://youtu.be/O7l2V9Dhggc)

