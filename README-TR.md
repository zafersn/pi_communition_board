# Pi_CAR JOYSTICK KARTI
İçerik Listesi
=================

<!--ts-->
   * [1. Genel Bakış](#1-genel-bakış)
   * [2. Block Diyagram ve PCB'Lere Genel Bakış](#2-block-diyagram-ve-pcblere-genel-bakış)
      * [2.1 Transmitter Kit'e Genel Bakış](#21-transmitter-kite-genel-bakış)
        * [Üstten Görünüş](#Üstten-görünüş)
        * [Alttan Görünüş](#alttan-görünüş)
        * [3D Render Görünümler](#3d-render-görünümler)
      * [2.2 Receive Kit'e Genel Bakış](#22-receive-kite-genel-bakış)
        * [Üstten Görünüş](#Üstten-görünüş-1)
        * [Alttan Görünüş](#alttan-görünüş-1)
        * [3D Render Görünümler](#3d-render-görünümler-1)
   * [3. Örnek Uygulama Videoları](#3-Örnek-uygulama-videoları)
        * [Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)](#pi_car-joystick-board-with-ros-gazebocustom-joytick-board)
        * [Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board)](#3pi_car-joystick-board-with-ros-turtlesim-custom-joytick-board)
<!--te-->

# 1. Genel Bakış
 &emsp;Kullanıcıların, **``Bluetooth``**, **``WiFi``** ve **``RF``** haberleşme teknolojileri üzerine geliştirme yapmak, programlamayı eğlenceli kılmak aynı zamanda uygulamaya yönelik öğrenme becerilerini geliştirmek amacıyla **``alıcı``** ve **``verici``** devresi olarak tasarlanmış bir geliştirme kartıdır.<br>
Arduino IDE' nin geniş kütüphane, hızlı programlama ve sadeliği gibi birçok desteğini de arkasına alan, fiyat performans kalitesi olarak da öne çıkan ESP32 cipset ailesinin işlevselliğini değerlendirmelerine olanak sağlamaktadır. Bu kit ( Pi_CAR Haberleşme Kartı ), uygulama geliştiricilerinin fikirlerini ESP32 serisi donanımı etrafında (RC-CAR Araç kontrol Senaryosu üzerine kurularak) oluşturmasına yardımcı olan temel donanım ( BLE 4.2, WiFi, RF ) ve yazılım kaynaklarını sağlar. Pi_CAR Haberleşme Kartı yazılım geliştirme çerçevesi,**`` Wi-Fi``**, **``Bluetooth``**,**`` RF``**, güç yönetimi ve diğer bazı sistem özellikleri ile hızla gelişen **``İnternet Nesneleri (IoT) uygulamları``** ve **``Robotik (ROS (Robot Operating System)) uygulamaları``** geliştirmek için tasarlanmıştır.

![overview](https://github.com/zafersn/pi_communition_board/blob/master/img/Block%20Diagram4.png)

# 2. Block Diyagram ve PCB'Lere Genel Bakış


## 2.1 Transmitter Kit'e Genel Bakış

 &emsp;Pi_CAR Transmitter Kartımız 2 adet Thumb Joystick ya da 1 Adet Thumb joystick ve 4 adet Tact Switch Button şeklinde konfigure edilerek kullanılabilir. Tranmitter kartı, kullanıcı ile receive kartı arasında RF üzerinden yaklaşık 1KM 'ye yakın bağlantı kurulmasını,buna ek olarak Bluetooth ve WiFi bağlantısı ile kullanıcıya yakın çevre birimleri ile iletişim kurulmasını ve spesifik uygulamar geliştirilmesini amaçlanmaktadır (VR, Cloud, telefon, pc vb...). 
 
### Üstten Görünüş

![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board4.png)

### Alttan Görünüş

![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board_Bttm2.png)

### 3D Render Görünümler

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


## 2.2 Receive Kit'e Genel Bakış

### Üstten Görünüş

![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/Rx_BOARD.png)

### Alttan Görünüş

![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/Rx_BOARD_bottom.png)

### 3D Render Görünümler

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

# 3. Örnek Uygulama Videoları

## Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)

[![Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)](https://img.youtube.com/vi/L5YpyjPOgC0/0.jpg)](https://youtu.be/L5YpyjPOgC0)

## Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board)

[![Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board))](https://img.youtube.com/vi/Qxs-DMT6eOg/0.jpg)](https://youtu.be/Qxs-DMT6eOg)



