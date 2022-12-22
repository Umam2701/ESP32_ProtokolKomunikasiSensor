# PROTOKOL KOMUNIKASI & SENSOR

ESP32 adalah nama dari mikrokontroler yang dirancang oleh perusahaan yang berbasis di Shanghai, China yakni Espressif Systems. ESP32 menawarkan solusi jaringan WiFi dan BLE. ESP32 menggunakan prosesor dual core yang berjalan di instruksi Xtensa LX16. Selain itu, ESP32 telah mendukung protokol komunikasi seperti I2C, UART dan SPI.

**ALAT DAN BAHAN**
1) ESP32
2) Breadboard
3) Kabel jumper
4) Sensor DHT 11, RFID
5) LED (5) dan Push Button (3)
6) Servo
7) Resistor 330,1K, 10K Ohm (@ 3)


<br />

**HASIL PERCOBAAN** 

**A. ESP32 Capacitive Touch Sensor**

*- Raw Data*


https://user-images.githubusercontent.com/118170084/209159872-e67ccd2f-14e8-4663-987c-6e4a7329f1d3.mp4


Analisa : Dari output Raw Data di atas ESP32 dapat digunakan sebagai Touch Sensor dimana saat kabel jumper disentuh makan akan menghasilkan data pada serial plotter seperti pada video di atas. Jadi apabila kabel jumpernya disentuh, maka pada serial plotter grafik/sinyal akan berada pada ambang atas. Sedangkan jika kabel jumper tidak disentuh, maka grafik/sinyal menunjukkan pada ambang bawah. <br><br>

*- Lampu LED ON jika jumper disentuh dan OFF jika jumper tidak disentuh*

>_"Dokumentasi sama seperti pada RAW DATA. (perhatikan LED-nya)"_

Analisa : Pada percobaan ini ditambahkan 1 LED. Pada keluaran didapatkan, apabila jumper disentuh, maka LED akan menyala, dan LED akan mati jika jumper tidak disentuh. <br><br>

*- Lampu LED akan menyala Blink saat jumper disentuh*

https://user-images.githubusercontent.com/118170084/209167477-e175d139-3f04-46aa-98db-fc94061439e6.mp4

Analisa : Pada percobaan ini masih mengimplementasikan hasil serial plotter hanya saja pada programnya dapat diatur seingga ketika jumper disentuh maka LED akan menyala BLINK dan mati ketika jumper tidak disentuh. <br><br>

*- Ketika LED menyala Serial Monitor akan menampilkan angka yang bertambah tiap kali sensor disentuh*

https://user-images.githubusercontent.com/118170084/209169350-b40f29aa-c6e2-4591-9dd4-b2631b64ecd6.mp4

Analisa : Pada percobaan ini menghasilkan data berupa angka yang bertambah tiap kali kabel jumper yang menjadi sensor disentuh dan ditampilkan di serial monitor. <br><br>

*- LED akan menyala Running saat sensor disentuh*

https://user-images.githubusercontent.com/118170084/209171947-ab943c61-58fb-4348-bf10-4171f3222a7e.mp4

Analisa : Pada percobaan ini program diubah sehingga ketika sensor disentuh maka LED akan menyala running dari kiri ke kanan, kemudian kanan ke kiri secara kontinyu. <br><br>


**B. Mengakses Sensor DHT 11 (Single Wire/BUS)**

*- Mengakses Sensor DHT 11 (contoh)*



*- Kondisi jika suhu 30 derajat, maka LED Merah menyala dan Buzzer berbunyi. Jika tidak, maka LED akan running*

Uploading Output Sensor DHT11+Buzzer.mp4…

Uploading Output Sensor DHT11+Buzzer.mp4…


Uploading Output Sensor DHT11+Buzzer.mp4…




**C. Mengakses Sensor RFID (SPI Communication)**

*- Mengakses Sensor RFID*



*- Kondisi apabila Tag RFID didekatkan pada Reader, maka LED Hijau akan menyala, servo akan bergerak ke kanan (lalu kembali ke posisi semula setelah 3 detik) dan di Serial Monitor akan tertampil pesan “Akses Diterima, Silahkan Masuk”. Apabila Tag RFID tidak dikenali, maka LED Merah akan menyala, servo tidak bergerak dan di Serial Monitor akan tertampil pesan “Akses Ditolak”*

Keluaran 


