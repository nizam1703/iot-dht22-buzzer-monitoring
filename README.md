# ESP8266 DHT22 Buzzer Blynk

Projek ini merupakan sistem IoT sederhana berbasis **ESP8266** yang menggunakan sensor **DHT22** untuk membaca suhu dan kelembapan. Jika suhu melewati batas yang sudah ditentukan, maka **buzzer** akan menyala sebagai tanda peringatan. Data suhu, kelembapan, dan status buzzer dikirim ke dashboard **Blynk** agar dapat dipantau secara real-time.

## Deskripsi Projek

Sistem ini bekerja dengan cara membaca data suhu dan kelembapan dari sensor DHT22. Data suhu kemudian dibandingkan dengan batas suhu yang sudah ditentukan pada program. Jika suhu lebih dari atau sama dengan 30°C, maka buzzer akan menyala. Jika suhu masih di bawah 30°C, maka buzzer akan mati.

Projek ini cocok digunakan sebagai simulasi sistem monitoring suhu ruangan, alarm suhu tinggi, atau sistem peringatan kondisi lingkungan berbasis IoT.

## Komponen yang Digunakan

- ESP8266
- Sensor DHT22
- Buzzer
- Kabel jumper
- Breadboard
- Platform Blynk
- Wokwi sebagai simulasi

## Library yang Digunakan

```cpp
#include <ESP8266WiFi.h>
#include <BlynkSimpleEsp8266.h>
#include <DHT.h>
