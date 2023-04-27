### Resume section 23 Fundamental Performance Testing

### Pengertian
Performance Testing adalah teknik non functional testing untuk menentukan parameter sistem dalam hal responsif dan stabilitas dibawah berbagai beban (load) kerja.
Performance testing mengukur kualitas atribut dari sistem seperti stabilitas, ketahanan (reliability), dan penggunaan sumber daya.

### Yang diukur dalan performance testing adalah :
- Performance suatu aplikasi sampai suatu batas tertentu
- Bukan merupakan functional-test
- Bisa dalam berbagai macam bentuk untuk memahami reliability, stability, dan availability pada environtment-nya.
Contoh :
.> Mengamati response time ketika menjalankan request dalam jumlah yang sangat banyak
.> Melihat suatu sistem berinteraksi dengan jumlah data yang cukup besar

Pada umumnya performance testing cukup mahal untuk diaplikasikan dan dijalankan, namun dapat dijadikan tolak ukur apakah sistem tersebut dapat mengakomodasikan traffic yang ada.
Hal ini disebabkan karena pengetesannya memerlukan persiapan yang dimana beberapa kasus harus membuat environment terpisah dari production agar tidak tercampurnya data test dengan data production.
Environment ini ada juga yang membuatnya di server load yang biayanya lebih besar dari environtment production.

Dalam melakukan performance test biasanya menjadi perhatian adalah throughput dan response data-nya.

### Contoh kasus performance test:
Sebuah sistem baru yang akan di launch ke production, namun sebelum masuk ke production perlu dilakukan performance test untuk mengetahui throughput dan response time dari sistem tersebut.
Untuk informasi endpoint yang akan ditest adalah:
1. /login
2. /beli_pulsa
3. /cek_out

Langkah yang harus dilakukan :
1. Membuat test plan
2. Membuat script test
3. Melakukan performance test
4. Menganalisa hasil performance test

### Metode Performance Test :

### Membuat test plan 
Kenali yang dibutuhkan : 
. Endpoint yang akan ditest:
  .> /login
  .> /beli_pulsa
  .> /cek_out
  
. Kebutuhan masing-masing endpoint :
  .> username dan password untuk endpoint/login
  .> produk, denom, dan nomor untuk pengetesan untuk endpoint /beli_pulsa
  .> metode pembayaran yang dipilih untuk endpoint /cek_out
  
### Menentukan Metode Test 
. Pilih berdasarkan kondisi sistem, apakah belum pernah dites atau sudah 
  - Selalu diawali dengan load test untuk tahu kondisi awal sistem
. Pilih berdasarkan situasi yang akan dihadapi

### Beberapa tipe Performance Test :
1. Load Test
2. Endurance Test
3. Stress Test
4. Peak Test

### Smoke Testing
Dilakukan untuk verify script yang sudah dibuat, apakah sistem tersebut dapat handle minimal load, tanpa masalah sama sekali. Biasanya hanya 1-2 VUs.

### Load Testing
Adalah pengujian paling sederhana yang dilakukan untuk memahami perilaku sistem dalam keadaan beban tertentu. Hasil dari load test digunakan untuk mengukur kepentingan saat transaksi yang kritis dengan memonitor dampak terhadap database, application server atau pendukung lainnya.
Sederhananya load testing menentukan kelakuan sistem pada saat kondisi normal dan puncak. Idealnya, kita mengetahui jumlah traffic yang ada di prod sebagai nilai di load test.

### Tabel Tier
Dijadikan patokan ideal suatu sistem baru yang belum pernah masuk ke production

### Stress Testing
Metode ini dilakukan untuk mengamati kemampuan dan kestabilan sistem pada saat kondisi ekstrem. Dilakukan bertahap menuju load normal, puncak, dan melebihinya, lalu turun untuk melihat proses recovery.

### Spike Testing
Seperti stress test, namun kenaikan langsung menuju melebihi puncak dilakukan dalam waktu singkat. Jika stress test memberikan waktu untuk scale-out, disini tidak.
Salah satu contoh adalah pada saat flash sale di suatu e-commerce, yang dimana banyaknya kunjungan pengguna yang langsung memuncak saat mengakses halaman flash sale.

### Soak Testing
Untuk mengetahui reliability ketika dalam tekanan di bawah puncak dalam jangka panjang (>=1 Jam). Dapat mengetahui apakah terdapat bug pada race condition, memory leaks, db connection dsb.
Tips : metode ini dilakukan berjam -jam sepi tidak ada transaksi pada sistem jika test dilakukan di production.

### Beberapa istilah penting dalam performance test :
1. System Under Test (SUT), sebutan untuk sistem yang sedang dilakukan test
2. Load Generator, sebutan untuk server yang digunakan untuk membuat request
3. Throughput, satuan kerja dalam satuan waktu. Misalnya Request Per Second (RPS) dan Request Per Minute (RPM)
4. Performance Threshold, target maksimal nilai yang diperbolehkan, misalnya response time 2 detik, max CPU usage 70% dan sebagainya
5. Saturation, kondisi dimana SUT atau Load Generator sudah dalam kondisi maksimum dalam merespon atau mengenerate
6. Virtual users, simulasi dari users yang melakukan pengujian, dapat melakukan satu atau lebih request dalam satu iterasi
7. Response time, lama waktu pengiriman request hingga menerima response.

### Note
- Volume test adalah salah satu non-functional test yang menguji ketahanan suatu sistem ketika diberi database yang banyak atau dikenal dengan istilah Flood Test
- Load test, menguji ketahanan secara umum, volume test berfokus pada sistem databasenya saja.



