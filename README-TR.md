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
Arduino IDE' nin geniş kütüphane, hızlı programlama ve sadeliği gibi birçok desteğini de arkasına alan, fiyat performans kalitesi olarak da öne çıkan ESP32 cipset ailesinin işlevselliğini değerlendirmelerine olanak sağlamaktadır. Bu kit ( Pi_CAR Joystick Kartı ), uygulama geliştiricilerinin fikirlerini ESP32 serisi donanımı etrafında (RC-CAR Araç kontrol Senaryosu üzerine kurularak) oluşturmasına yardımcı olan temel donanım ( BLE 4.2, WiFi, RF ) ve yazılım kaynaklarını sağlar. Pi_CAR Joystick Kartı yazılım geliştirme çerçevesi,**`` Wi-Fi``**, **``Bluetooth``**,**`` RF``**, güç yönetimi ve diğer bazı sistem özellikleri ile hızla gelişen **``Nesnelerin İnterneti (IoT) uygulamları``** ve **``Robotik (ROS (Robot Operating System)) uygulamaları``** geliştirmek için tasarlanmıştır. 

## 1.1 Pi_CAR Joystick Kartı Amaçları
### 1.1.1 Temel Amaçlar ve Kazanılması Beklenen Tecrübeler

* 1. ESP32-WROOM-32'nin yapısı, fonsiyonu ve uygulamalarının geliştirilmesi
       * a. ESP32'nin ESP-IDF ile programlama ve kullanım. (Eclipse üzerinde)
       * b. ESP32'nin Arduino IDE ile programlama ve kullanım.
       * c. Wi-Fi, Bluetooth, Mesh Network, Peripherals (ADC, SPI, UART, TIMER, PWM, GPIO Vb...), Storage (MicroSD), System (FreeRTOS, Watchdogs, Over The Air Updates (OTA), High Resolution Timer Vb...) kullanımı.
       * d. Debugging ( GDB kullanılarak hata ayıklama )
* 2. Bluetooth, WiFi, RF Haberleşme Protokolleri öğrenme ve uygulamalar geliştirme 
       * a. Bluetooth, WiFi, RF Uygulamaları geliştirme
       * b. TCP, UDP Uygulamaları geliştirme
* 3. Nesnelerin İnterneti (IoT) uygulamları geliştirme
       * a. MQTT, HTTP haberleşme protokollerini öğrenme, IBM Watson IoT Platform ya da IVEN Bulut Platform kullanarak uygulama geliştirme

* 4. ROS (Robot Operating System) uygulamaları geliştirme. 
       * a. ROS(Robot Operating System) yapısı (Nodes, Topics, Messages, Publisher, Subscriber, Services vs...), kütüphaneleri, araçları kullanılması ve oluşturulması.
       * b. Gazebosim araçlarının kullanımı, modelleme, simülasyon ve ROS ile haberleştirilmesi.
       

![overview](https://github.com/zafersn/pi_communition_board/blob/master/img/Block%20Diagram4.png)

# 2. Block Diyagram ve PCB'Lere Genel Bakış


## 2.1 Transmitter Kit'e Genel Bakış

 &emsp;Pi_CAR Transmitter Kartımız 2 adet Thumb Joystick ya da 1 Adet Thumb joystick ve 4 adet Tact Switch Button şeklinde konfigure edilerek kullanılabilir. Tranmitter kartı, kullanıcı ile receive kartı arasında RF üzerinden yaklaşık 1KM 'ye yakın bağlantı kurulmasını,buna ek olarak Bluetooth ve WiFi bağlantısı ile kullanıcıya yakın çevre birimleri ile iletişim kurulmasını ve spesifik uygulamar geliştirilmesini amaçlanmaktadır (VR, Cloud, telefon, pc vb...). 
 
Üstten Görünüş
=================

![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board4.png)

Alttan Görünüş
=================

![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board_Bttm2.png)

3D Render Görünümler
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
1 |  Kart Boyutları  99 x 61 mm | RF SMA Anten Dahil Değil


## 2.2 Receive Kit'e Genel Bakış

Üstten Görünüş
=================

![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/Rx_BOARD.png)

Alttan Görünüş
=================

![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/Rx_BOARD_bottom.png)

3D Render Görünümler
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
1 |  Kart Boyutları 89 x 52 mm | RF SMA Anten Dahil Değil


# 3. Örnek Uygulama Videoları

## Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)

[![Pi_CAR Joystick Board with ROS GAZEBO(Custom Joytick Board)](https://img.youtube.com/vi/L5YpyjPOgC0/0.jpg)](https://youtu.be/L5YpyjPOgC0)

## Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board)

[![Pi_CAR Joystick Board with ROS Turtlesim (Custom Joytick Board))](https://img.youtube.com/vi/Qxs-DMT6eOg/0.jpg)](https://youtu.be/Qxs-DMT6eOg)



