# Pi HABERLEŞME KARTI

# 1. Genel Bakış
 &emsp;Kullanıcıların, **``Bluetooth``**, **``WiFi``** ve **``RF``** haberleşme teknolojileri üzerine geliştirme yapmak, programlamayı eğlenceli kılmak aynı zamanda uygulamaya yönelik öğrenme becerilerini geliştirmek amacıyla **``alıcı``** ve **``verici``** devresi olarak tasarlanmış bir geliştirme kartıdır.<br>
Arduino IDE' nin geniş kütüphane, hızlı programlama ve sadeliği gibi birçok desteğini de arkasına alan, fiyat performans kalitesi olarak da öne çıkan ESP32 cipset ailesinin işlevselliğini değerlendirmelerine olanak sağlamaktadır. Bu kit ( Pi_CAR Haberleşme Kartı ), uygulama geliştiricilerinin fikirlerini ESP32 serisi donanımı etrafında (RC-CAR Araç kontrol Senaryosu üzerine kurularak) oluşturmasına yardımcı olan temel donanım ( BLE 4.2, WiFi, RF ) ve yazılım kaynaklarını sağlar. Pi_CAR Haberleşme Kartı yazılım geliştirme çerçevesi,**`` Wi-Fi``**, **``Bluetooth``**,**`` RF``**, güç yönetimi ve diğer bazı sistem özellikleri ile hızla gelişen **``İnternet Nesneleri (IoT) uygulamları``** ve **``Robotik (ROS (Robot Operating System)) uygulamaları``** geliştirmek için tasarlanmıştır.

![overview](https://github.com/zafersn/pi_communition_board/blob/master/img/Block%20Diagram4.png)

# 2. Block Diyagram ve PCB'Lere Genel Bakış


## 2.1 Transmitter Kit'e Genel Bakış
![Top View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board4.png)
![Bottom View render block diagram](https://github.com/zafersn/pi_communition_board/blob/master/img/TX_Board_Bttm2.png)
![Top View render 1](https://github.com/zafersn/pi_communition_board/blob/master/img/1.PNG)

![Top View render 2](https://github.com/zafersn/pi_communition_board/blob/master/img/2.PNG)

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



