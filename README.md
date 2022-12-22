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

**Raw Data**

Keluaran Serial Monitor


Keluaran Serial Plotter


Keluaran Serial Plotter (disentuh)


Analisa : Pada percobaan ini diambil data (Raw Data) dari serial monitor dan plotter dari rangkaian dan script yang dijalankan. Percobaan ini digunakan touch sensor. Jadi apabila kabel jumper yang terhubung ke pin touch sensor disentuh, maka pada serial monitor dapat dilihat nilai yang keluar akan semakin bertambah dan pada serial plotter pun grafik/sinyal akan berada pada ambang atas. Sedangkan jika kabel jumper touch sensor tidak disentuh, maka nilai akan semakin berkurang dan grafik/sinyal menunjukkan pada ambang bawah.

**Kemudian Buat Rangkaian Seperti di Bawah**


Keluaran


Analisa :Pada percobaan ini ditambahkan 1 LED. Pada keluaran didapatkan, apabila jumper touch sensor disentuh, maka LED akan menyala, dan LED akan mati jika jumper tidak disentuh. 

**Kemudian Tambahkan Rangkaian Menjadi 3 LED Agar Menyala Running**

Keluaran



**2) Mengakses Sensor DHT 11 (Single Wire/BUS)**

**Mengakses Sensor DHT 11**

Keluaran 


**Kondisi jika suhu 30 derajat, maka LED Merah menyala dan Buzzer berbunyi. Jika tidak, maka LED akan running**

Keluaran 



**3) Mengakses Sensor RFID (SPI Communication)**

**Mengakses Sensor RFID**

Keluaran 


**Kondisi apabila Tag RFID didekatkan pada Reader, maka LED Hijau akan menyala, servo akan bergerak ke kanan (lalu kembali ke posisi semula setelah 3 detik) dan di Serial Monitor akan tertampil pesan “Akses Diterima, Silahkan Masuk”. Apabila Tag RFID tidak dikenali, maka LED Merah akan menyala, servo tidak bergerak dan di Serial Monitor akan tertampil pesan “Akses Ditolak”**

Keluaran 


