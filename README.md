### Resume section 24 Introduction & Tutorial Record with JMeter
Ada beberapa tools yang dapat kita lakukan untuk melakukan pengujian ini :
- JMeter
- BlazeMeter
- Locust dll

Pada pengujian kali ini, kita menggunakan JMeter

### Pengertian
JMeter adalah software yang berlisensi Apache, yang merupakan perangkat lunak dengan sumber terbuka sehingga semua orang dapat ikut serta dalam menggunakan aplikasi JMeter ini.
JMeter juga terbuat dari aplikasi desktop berbasis java yang dirancang untuk menguji perilaku suatu website sehingga pengguna dapat melihat apakah website tersebut memiliki fungsionalitas dan kinerja yang sudah sesuai.
Apache JMeter semakin bertambah waktu semakin dikembangkan pula sehingga yang awalnya hanya untuk menguji website sekarang sudah berkembang pada fungsi-fungsi pengujian yang lainnya.

### Berikut Keuntungan Dalam Menggunakan JMeter :
- Open Source, sehingga kita dapat melihat code dari aplikasi JMeter ini. Jika ada masalah, kita dapat melihat sendiri permasalahan tersebut terjadi pada bagian mana
- JMeter dibuat dalam bentuk user inteface dan tanpa user interface, jika dengan user interface makan kita akan mendapatkan aplikasi yang berjalan seperti aplikasi desktop pada umumnya, terdapat tombol, form untuk input, dan tampilan-tampilan yang digunakan untuk interaksi lainnya. Jika kita menggunakan fitur non GUI dari JMeter ini maka kita dapat menggunakannya pada sistem berbasis YLIN atau command line interface. 

### Cara menginstallnya:
1. Install JDK (Java Development Kit) 
2. Download JMeter
3. Buka file dalam zip JMeter
4. Buka terminal dan buka jmeter
5. Install Plugin

### Komponen JMeter :
1. Test Plan
Rencana besar tes yang akan dilakukan (parent)
2. Thread Groups
Kumpulan thread yang menjalankan skenario yang sama
3. Samplers
Sebutan untuk request yang dikirim ke server
4. Config Element
Elemen yang digunakan untuk konfigurasi atau modifikasi sampler atau request yang dikirim ke server
5. Listener
Perekam data yang dihasilkan dari tes
6. Timers
Fitur ini akan jalan duluan sebelum semua fitur yang lain berjalan
7. Assertions
Seperti assert pada API/Web/Testing, merupakan kriteria tambahan apakah pass/tidak
8. Pre-post Processors
Fitur yang memproses response data sebelum/sesudah test


