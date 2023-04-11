### Resume section 26 Post Processor

Post Processor adalah bagian dari Test Plan yang merupakan sebuah aksi yang berjalan saat proses telah dilakukan. Proses yang dilakukan pada web processor ini umumnya adalah untuk mengekstrak value yang didapatkan dari hasil mengakses halaman pada web seperti data - data pada JSON, pada session, atau pada bagian respon yang lainnya. 

Berikut salah satu Post Processor di JMeter yang bisa kita gunakan adalah JSON Extractor.
#### JSON Extractor
Pada JSON Extractor kita dapat menggunakan JSON Path untuk mengambil nilai - nilai yang terdapat pada data JSON yang dihasilkan dari respon saat kita melakukan request. 

#### JSON Path
Terkait JSON Path, berikut adalah aturan - aturan yang dapat digunakan untuk mengekstraksi JSON :
-> $ = root element, artinya seluruh data JSON yang didapatkan adalah $ 
-> . = child operator (object), untuk mengoperasikan child operator object dapat menggunakan tanda titik.
->[] = child operator (array), untuk mengoperasikan child operator array dapat menggunakan kurang siku buka dan tutup.
