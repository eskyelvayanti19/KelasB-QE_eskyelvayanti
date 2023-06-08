### Resume section 28 Testing In CI/CD Pipeline 

### Pengertian CI
CI atau Continous Integration adalah praktik pengembangan software dimana developer berupa code serta melakukan match pada sebuah repository atau penyimpanan secara reguler dan terus menerus. Nnatinya jika ada branch atau commityang baru maka automated test dan build akan dijalankan sehingga hasilnya bisa langsung diketahui. Jadi, jika ada kesalahan dalam proses CI ini maka pihak development dapat langsung melakukan tindakan atau action. Syaratnya adlah dengan memperbarui code sehingga kualitasnya bisa snya bisa ditingkatkan sekaligus menghemat waktu ketika melakukan validate update.

CI sendiri merupakan solusi menyederhanakan tahapan pengembangan software sehingga isu bisa diperbaiki.

### Di dalam CI terdapat tiga stage yang harus dilatih seperti : build, unit tests, dan integration tests.

### Pengertian CD
CD atau Continous delivery/deployment yang mana memiliki makna yang berbeda-beda. Continous delivery adalah proses setelah continous integration, dimana developer sudah menjalankan build dan test, namun memilih untuk tidak melimpahkannya ke invirontment production. Continous deployment secara otomatis akan rilis ke production.

### Perbedaan Continous Delivery dan Deployment
- Delivery : 1. Butuh manual action untuk rilis ke production 
- Deployment : 1. Akan otomatis rilis ke production tanpa perlu approval dari developer

### Hal-hal untuk membuat cI/CD yang bagus :
*Ada 3 hal untuk membuat CI yang bagus :
1. Decoupled Stages, step-step yang berjalan di CI harus mengerjakan single task atau lebih fokus dalam task tersebut
2. Repeatable, step yang berulang-ulang bisa dipakai lagi atay konsisten, serta developer juga bisa memakai tools tersebut di local
3. Fail Fast, ketika aa error di line pertama stages tersebut harus langsung fail.

*Ada 3 hal untuk membuat CD yang bagus :
1. Design with system in mind, banyak bagian yang harus dicover atau dipikirkan dalam deployment, seperti aplikasi, infrastuktur, konfigurasi, dan data.
2. Pipelines, meningkatkan confidence untuk bisa lanjut ke production
3. Globally Unique version, mengetrti step-step di version kapan waktu serta bisa mendemokan antara current dengan future state.

### CI/CD
CI/CD adalah proses berkelanjutan serta terus-menerus dalam software deployment, mulai dari awal hingga software tersebut mencapai customers dan mendapatkan feedback, secara garis besar tahapan dari proses CI/CD  berikut ini, seperti :
1. Developer akan menulis sejumlah code untuk kemudian dieksekusi menggunakan versions control system
2. Commit
3. Build
4. Test
5. Deploy

### Manfaat CI dalam pengembangan perangkat lunak :
1. Dapat mendeteksi bug lebih cepat, CI/CD melakukan pengujian secara otomatis sehingga jika ada bug yang muncul pada aplikasi yang dikembangkan atau didevelopment maka langsung akan terdeteksi oleh CI itu. Developer juga dapat dengan menemukan dan memperbaiki bug tersebut
2. Reduce Bug Count, ketika menemukan bug secara otomatis juga akan mengurangi bug-bug yang muncul, ketika akan melakukan build atau deployment
3. Dapat mempercepat proses rilis, proses rilis dari suatu aplikasi dapat dipercepat. Hal itu disebabkan code yang terus digabungkan dan diterapkan ke dalam product sehingga apliaksi selalu dalam kondisi siap untuk dirilis kapanpun
4. Efisien

### Manfaat CD dalam pengembangan perangkat lunak :
1. Reduce the risk
2. Mengurangi dari sebuah deployment, jadi  biasanya deploymnet itu membutuhkan waktu yang sangat lama dan membutuhkan tenaga yang tidak sedikit
3. Mengurangi cost
4. Automated and Transparent Process
5. Merilis feature secara terus menerus

### Continuous Integration Costs :
Karena berjalan secara otomatis, kita harus menuliskan test secara automated dan harus menyiapkan untuk test tersebut, serta akan sering melakukan merge terhadap code-code yang baru.

### Continuous Delivery Costs :
Harus mengerti fondation dari suatu CI itu sendiri, membutuhkan kualitas test yang sangat tinggi, dan harus sering mengupdate dokumentasi-dokumentasi dari sebuah CI/CD ataur software tersebut.

### CI/CD tools :
1. Jenkins, adalah salah satu tools CI/CD yang paling sering digunakan oleh para developer yang mana merupakan open source automation server dan central build continous integration secara berlangsung, tools ini menggunakan bahasa pemrograman java dan bisa digunakan pada windows, macOS, dll (free, open source)
2. Bamboo
3. Circleci
4. Travis CI
5. AWS codeCuild
6. Azure Devops
7. CI/CD
8. GitHub Action
9. GitLab CI

### Pesriapan penggunaan CI/CD :
1. Install Java 1.8
2. Maven
3. Intellij IDEA
4. Git




