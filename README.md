### Resume section 27 Mobile Testing With Serenity 
Mobile testing adalah proses dimana aplikasi yang dikembangkan untuk perangkat mobile diuji untuk kegunaan dan konsistensinya. Ada 2 macam testing yang harus dilakukan pada aplikasi pada perangkat mobile, yaitu :
- Pengujian Hardware, testing hardware termasuk processor, memori internal, ukuran layar, resolusinya, besarnya RAM, kemampuan kamera, bluetooth, wifi dll akan menjadi komponen yang harus ditesting dalam proses pengujian hardware 
- Pengujian Sotware, dalam tahap ini aplikasi yang telah dikembangkan akan diuji secara detail dan teliti. Fungsi dan konsistensi sebuah aplikasi mobile akan diuji. 

seperti kita ketahui bahwa aplikasi mobile terbagi menjadi 3 macam, yaitu : Aplikasi mobile native, hybrid, dan web. Ketiganya memiliki perbedaaan dasar yang tentunya mempengaruhi proses pengujian. Pengujian aplikasi mobile jauh lebih kompleks dibandingkan pengujian aplikasi atau web desktop karena mobile meiliki banyak macam ukuran konfigurasi hardware seperti Qpad, virtual Qpad, kemudian bermacam-macam sistem informasi yang dipakai seperti android, windows, Ios dan semacamnya. 
Dan juga memiliki jenis jaringan mobile seperti xdme atau gsm.

### Ada beberapa macam testing yang selayaknya digunakan untuk mengatasi masalah - masalah mobile testing :
- Usability Testing, untuk memastikan bahwa aplikasi mobile mudah digunakan dan memberikan user experience untuk penggunanya 
- Compatibility Testing, pengujian aplikasi dengan perangkat mobile yang berbeda melalui browser dengan ukuran layar yang berbeda serta versi OS sesuai dengan kebutuhan.
- Interface Testing, pengujian pemilihan menu, tombol, kogma, history, pengaturan, dan navigasi dari aplikasi pengujian testing dalam keadaan online maupun offline.
- Low Level High Resource Testing, pengujian memory, auto delete file-file sementara, dan adanya database.
- Performance Testing, pengujian kinerja aplikasi dengan mengubah koneksi dari 2G ke Wifi atau 3G ke Wifi, kemampuan bebagi dokumen dan bagaimana kapasitas batreh yang dibutuhkan.
- Operational Testing, back up dan rencana recovery jika batreh melemah atau saat kehilangan data karena proses update dari toko.
- Installation Testing, validasi aplikasi dengan menginstall atau menguninstall perangkat mobile.
- Security, pengujian aplikasi untuk menvalidasi apakah data terlindungi di sistem informasi.

Untuk memastikan bahwa standaritas dan kinerja terpenuhi, maka adanya strategi untuk testing aplikasi mobile sangat dibutuhkan seperti pemilihan perangkat, analisis pasar, dan memilih perangkat yang banyak digunakan. Keputusan ini sebagian besar bergantung pada user atau pada development yang mempertimbangkan popularitas sebuah perangkat lunak tertentu.

Emulator, penggunaan emulator sangat membantu dalam tahap pengembangan awal. Emulator memungkinkan untuk melakukan pengecekan secara cepat dan efisien. Emulator sendiri merupakan sistem yang menjalankan software yang seolah-olah membawa kita pada sistem operasi lain.

### Mobile Automation Testing
Pada autimation kali ini akan menggunakan appium sebagai toolsnya.
Appium adalah mobile web, native, dan software application test automation tools dan juga open source artinya gratisan software automation tools, biasanya banyak digunakan untuk android dan IOS platform aplikasi. 
Appium dapat dijalankan di android appium simulator maupun di field device.

Keuntungan appium :
- Dapat regression alikasi mobile kita menjadi lebih mudah khususnya untuk apliksi mobile yang ngeshare updatenya dilakukan secara berkelanjutan dengan fitur dan fungsi yang terus diperbaharui.
- Appium mendukung multiple platform dan language serta bisa menggunakan testing framework apapun, seperti Android, IOS, Windows OO dll
- Appium mendukung abhasa pemrograman seperti java, bahasa c, javascript, python, ruby, php dll
- Appium tidak membutuhkan source code testing aplikasi dimana kita bisa testing langsung juga kita bisa membangun build in aplikasi seperti kamera, kalender, dsb di dalam tes script kita nanti

Keterbataan appium :
- Untuk versi android, appium tidak support untuk android level kurang dari 17 dan untuk eksekusi script sangat lambat di IOS platform serta gesture supportnya sangat terbatas 

### Appium Level High Architecture :
Client -> appium server -> XCUITest, UIAutomator2/Espreso, WinAppDriver

### Appium Components :
- Appium Server, merupakan komponen inti dari arsitektur appium, ditulis di node jd dan berjalan di mesin atau di cloud
- Appium Client, meminta untuk memulai session menggunakan perintah create session melalui protocol JSON While, menjalankan beberapa pengujian pada perangkat seluler dan menerima hasil dari server appium.

Library appium menjangkau beberapa bahasa, yaitu PHP, Java, Javascript, Python, Ruby dll

### Installation Appium :
Tools yang akan digunakan :
- Java JDK 8/11
- Install Android SDK Platform-tools & command-line tools
- Appium Desktop
- Node JS
- Appium-doctor

