# Pi_CAR JOYSTICK BOARD

Table of contents
=================
<!--ts-->
   * [1. Overview](#1-overview)
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
<!--te-->

# 1. Overview
&emsp;  It is a development board(**``Pi_CAR JOYSTICK BOARD``**) designed as a receiver and transmitter circuit for users to develop themselves on **``Bluetooth``**, **``WiFi``** and **``RF``** communication technologies, to make programming fun, and to develop application-oriented learning skills.
  Arduino IDE's extensive library, fast programming and simplicity, such as support behind many, as the price performance quality of the prominent ESP32 chipset family allows you to evaluate the functionality. This kit (Pi_CAR Communication Card) provides basic hardware (BLE 4.2, WiFi, RF) and software resources that help application developers build their ideas around the ESP32 series hardware (based on the RC-CAR Vehicle control Scenario).The Pi_CAR Communication Card software development framework is designed to develop fast-growing  **``Internet of Things (IoT)``** applications and  **``Robotics (ROS (Robot Operating System))``** applications with  **``Wi-Fi``**,  **``Bluetooth``**,  **``RF``**, power management and some other system features.
  
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

Adet | Ürün Adı | Açıklama
------------|---------| -------------
1 | ESP32 Joystick Ana kartı | BLE + WiFi
2 | Thumb Joysticks | 2 Eksen Kontrol
4 | Momentary Pushbutton Switch | 12mm 
2 | NRF24L01 | ~1KM Menzil - Alıcı ve Verici
1 | MikroBUS | Standartlaştırılmış Genişletme Kartı Desteği  <p>[Bakınız: MicroBUS](https://www.mikroe.com/mikrobus)</p>
1 | Micro SD Socket| 
2 | RGB LED 
3 | FPV Güç I/O | Board ile İzole 
1 | Güç Girişi | 6V - 18V
1 | Micro USB | Programlama ve haberleşme için USB 'den seri bağlantı dönüştürücü
1 | JTAG Debugging | Programlama ve Debug için.

## 2.2 Receive Kit Overview
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


Adet | Ürün Adı | Açıklama
------------|---------| -------------
1 | ESP32 Joystick Ana kartı | BLE + WiFi
2 | NRF24L01 | ~1KM Menzil - Alıcı ve Verici
1 | MikroBUS | Standartlaştırılmış Genişletme Kartı Desteği  <p>[Bakınız: MicroBUS](https://www.mikroe.com/mikrobus)</p>
2 | RGB LED 
3 | FPV Güç I/O | Board ile İzole 
1 | Güç Girişi | 6V - 18V
1 | Micro USB | Programlama ve haberleşme için USB 'den seri bağlantı dönüştürücü
1 | JTAG Debugging | Programlama ve Debug için.
1 | FPV Camera Girişi |
40| Harici I/O | PWM/SPI/USART/I2C/GPIO

# 3. Sample Demo Videos

Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)
=================

Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board)
=================
