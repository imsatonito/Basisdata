# Tugas 1

## 1. Apa itu client-server programming? (Point : 6)

Client-server programming adalah model arsitektur yang menggunakan dua komponen utama:
- Client: Bertindak sebagai peminta layanan
- Server: Bertindak sebagai penyedia layanan

Dalam model ini, client mengirimkan permintaan ke server untuk melakukan tugas tertentu, dan server merespons permintaan tersebut. Pada konteks basis data, client biasanya berfungsi sebagai antarmuka pengguna, sementara server mengelola operasi pada database.

## 2. Apa perbedaan antara sistem berkas (file system) dan sistem basis data (database system)? (Point : 6)

Perbedaan utama antara sistem berkas dan sistem basis data meliputi:

1. Struktur data: 
   - Sistem berkas: Data disimpan sebagai file terpisah
   - Sistem basis data: Data disimpan dalam tabel yang saling terkait

2. Manajemen data:
   - Sistem berkas: Mengelola data sebagai file individu yang tidak terkait
   - Sistem basis data: Mengelola data sebagai bagian dari kesatuan yang lebih besar (database)

3. Integritas data:
   - Sistem berkas: Tidak menjamin integritas data
   - Sistem basis data: Menggunakan konsep seperti constraint dan transaksi untuk menjaga integritas data

4. Keamanan:
   - Sistem berkas: Keamanan data terbatas
   - Sistem basis data: Menyediakan fitur keamanan yang lebih baik seperti autentikasi dan otorisasi

5. Performa:
   - Sistem berkas: Performa lebih lambat untuk data yang kompleks
   - Sistem basis data: Memiliki fitur untuk mengoptimalkan akses data, sehingga performa lebih baik

## 3. Apa itu DBMS (Database Management System) dan mengapa penting dalam sistem basis data? (Point : 6)

DBMS (Database Management System) adalah perangkat lunak yang digunakan untuk mengelola dan memanipulasi data yang disimpan dalam database. DBMS penting karena:

1. Memungkinkan penyimpanan dan pengambilan data yang efisien
2. Menjaga integritas dan keamanan data
3. Mendukung akses bersamaan oleh banyak pengguna
4. Menyediakan mekanisme untuk backup dan pemulihan data
5. Memungkinkan optimisasi kinerja melalui indeksasi dan caching
6. Menyediakan antarmuka untuk interaksi dengan data menggunakan bahasa query

Contoh DBMS populer termasuk MySQL, Oracle Database, Microsoft SQL Server, dan PostgreSQL.

## 4. Apa itu basis data, dan mengapa basis data penting dalam pengembangan perangkat lunak? (Point : 6)

Basis data adalah kumpulan data yang diorganisasikan dan dikelola menggunakan sistem manajemen basis data (DBMS). Basis data penting dalam pengembangan perangkat lunak karena:

1. Memungkinkan penyimpanan data yang terstruktur dan efisien
2. Mendukung akses dan manipulasi data yang cepat
3. Menjaga integritas dan konsistensi data
4. Memungkinkan sharing data antar aplikasi dan pengguna
5. Menyediakan mekanisme keamanan untuk melindungi data sensitif
6. Mendukung skalabilitas untuk menangani pertumbuhan data
7. Memfasilitasi analisis data untuk pengambilan keputusan

## 5. Jelaskan perbedaan antara data dan informasi, dan bagaimana basis data berperan dalam mengubah data menjadi informasi yang bermakna? (Point : 6)

Data adalah kumpulan fakta mentah yang belum memiliki arti, sedangkan informasi adalah data yang telah diproses dan memiliki makna atau konteks.

Basis data berperan dalam mengubah data menjadi informasi yang bermakna dengan cara:

1. Organisasi: Menyusun data dalam struktur yang terorganisir (tabel, relasi)
2. Pemrosesan: Memungkinkan query dan analisis data
3. Agregasi: Menggabungkan data dari berbagai sumber
4. Kontekstualisasi: Menghubungkan data dengan metadata dan relasi
5. Presentasi: Menyajikan data dalam format yang mudah dipahami

Dengan fitur-fitur ini, basis data membantu mengubah data mentah menjadi informasi yang dapat digunakan untuk pengambilan keputusan dan wawasan bisnis.

## 6. Apa yang dimaksud dengan skema basis data, dan mengapa itu penting dalam perancangan basis data? (Point : 6)

Skema basis data adalah deskripsi logis dari struktur dan organisasi data dalam suatu basis data. Ini mencakup definisi tabel, kolom, relasi antar tabel, dan konstrain data.

Skema basis data penting dalam perancangan basis data karena:

1. Memberikan blueprint untuk struktur data
2. Mendefinisikan hubungan antar entitas data
3. Memastikan integritas data melalui konstrain
4. Memfasilitasi pemahaman struktur data bagi pengembang dan pengguna
5. Memungkinkan optimisasi kinerja basis data
6. Mendukung evolusi dan pemeliharaan basis data seiring waktu

## 7. Apa itu entitas dalam konteks basis data, dan bagaimana hubungannya dengan tabel dalam DBMS? (Point : 6)

Entitas dalam konteks basis data adalah objek atau konsep dunia nyata yang dapat diidentifikasi secara unik dan memiliki atribut. Contohnya bisa berupa pelanggan, produk, atau pesanan.

Hubungan entitas dengan tabel dalam DBMS:

1. Representasi: Setiap entitas biasanya direpresentasikan sebagai tabel dalam DBMS
2. Atribut: Atribut entitas menjadi kolom dalam tabel
3. Instance: Setiap baris dalam tabel merepresentasikan instance spesifik dari entitas
4. Kunci Primer: Atribut unik entitas menjadi kunci primer dalam tabel
5. Relasi: Hubungan antar entitas diimplementasikan melalui kunci asing dalam tabel

Dengan demikian, entitas dalam model konseptual diterjemahkan menjadi struktur tabel dalam implementasi DBMS.

## 8. Jelaskan perbedaan antara basis data relasional dan basis data non-relasional (NoSQL). (Point : 6)

Perbedaan utama antara basis data relasional dan non-relasional (NoSQL):

1. Struktur:
   - Relasional: Data disimpan dalam tabel dengan skema yang tetap
   - NoSQL: Fleksibel, bisa menggunakan berbagai model data (dokumen, key-value, kolom-lebar, graf)

2. Skema:
   - Relasional: Skema yang kaku, harus didefinisikan sebelum memasukkan data
   - NoSQL: Skema fleksibel, bisa berubah tanpa mengganggu aplikasi

3. Skalabilitas:
   - Relasional: Umumnya skalabilitas vertikal (meningkatkan kapasitas server)
   - NoSQL: Skalabilitas horizontal yang lebih mudah (menambah server)

4. Konsistensi:
   - Relasional: Menjamin konsistensi data yang kuat (ACID)
   - NoSQL: Beberapa sistem NoSQL mengadopsi konsistensi eventual untuk performa lebih baik

5. Query:
   - Relasional: Menggunakan SQL standar
   - NoSQL: Seringkali menggunakan API atau bahasa query khusus

6. Use Case:
   - Relasional: Cocok untuk aplikasi dengan struktur data yang jelas dan transaksi kompleks
   - NoSQL: Ideal untuk aplikasi dengan data yang cepat berubah, volume besar, atau struktur yang bervariasi

## 9. Apa fungsi utama DBMS dalam sebuah sistem basis data, dan sebutkan beberapa DBMS populer yang digunakan secara luas di industri perangkat lunak. (Point : 6)

Fungsi utama DBMS dalam sistem basis data:

1. Manajemen Data: Menyimpan, mengambil, dan memperbarui data
2. Keamanan: Mengontrol akses dan melindungi data
3. Integritas: Memastikan akurasi dan konsistensi data
4. Konkurensi: Mengelola akses bersamaan oleh banyak pengguna
5. Pemulihan: Menyediakan backup dan mekanisme pemulihan
6. Optimisasi: Meningkatkan kinerja query dan akses data
7. Abstraksi Data: Menyembunyikan kompleksitas penyimpanan dari pengguna

DBMS populer yang digunakan secara luas:

1. MySQL
2. Oracle Database
3. Microsoft SQL Server
4. PostgreSQL
5. MongoDB
6. SQLite
7. IBM Db2
8. MariaDB
9. Cassandra
10. Redis

## 10. Apa itu ERD (Entity Relationship Diagram) dalam konteks desain basis data, dan mengapa ERD penting? (Point : 6)

ERD (Entity Relationship Diagram) adalah model visual yang menggambarkan entitas dalam sistem basis data dan hubungan antar entitas tersebut. ERD menggunakan simbol-simbol grafis untuk merepresentasikan entitas, atribut, dan relasi.

ERD penting karena:

1. Visualisasi Struktur: Memberikan gambaran visual yang jelas tentang struktur basis data
2. Komunikasi: Memudahkan komunikasi antara desainer, pengembang, dan stakeholder
3. Perencanaan: Membantu dalam perencanaan dan desain basis data sebelum implementasi
4. Dokumentasi: Berfungsi sebagai dokumentasi struktur basis data
5. Analisis: Membantu dalam mengidentifikasi redundansi dan inkonsistensi dalam desain
6. Normalisasi: Memfasilitasi proses normalisasi basis data
7. Evolusi: Memudahkan dalam merencanakan perubahan dan pengembangan basis data di masa depan

## 11. Apa itu atribut dalam konteks ERD, dan apa perbedaan antara atribut kunci dan atribut non-kunci? (Point : 8)

Atribut dalam konteks ERD adalah karakteristik atau properti yang menggambarkan suatu entitas. Atribut mewakili informasi spesifik yang disimpan untuk setiap instance dari entitas.

Perbedaan antara atribut kunci dan atribut non-kunci:

Atribut Kunci:
1. Berfungsi untuk mengidentifikasi secara unik setiap instance dari entitas
2. Biasanya menjadi primary key dalam implementasi tabel database
3. Tidak boleh memiliki nilai null atau duplikat
4. Digunakan untuk membentuk relasi antar entitas

Atribut Non-Kunci:
1. Menyimpan informasi deskriptif tentang entitas
2. Tidak digunakan untuk identifikasi unik instance entitas
3. Dapat memiliki nilai null (tergantung pada desain)
4. Dapat memiliki nilai yang sama untuk beberapa instance entitas

Contoh:
Untuk entitas "Mahasiswa", NIM bisa menjadi atribut kunci, sedangkan nama, alamat, dan tanggal lahir adalah atribut non-kunci.

## 12. Apa yang dimaksud dengan hubungan (relationship) dalam ERD, dan bagaimana hubungan dijelaskan dalam diagram ERD? (Point : 8)

Hubungan (relationship) dalam ERD adalah asosiasi atau koneksi logis antara dua atau lebih entitas. Hubungan menggambarkan bagaimana entitas berinteraksi atau terkait satu sama lain dalam sistem.

Hubungan dijelaskan dalam diagram ERD melalui:

1. Garis Penghubung: Menghubungkan entitas yang berelasi
2. Nama Hubungan: Label yang menjelaskan sifat hubungan
3. Kardinalitas: Menunjukkan jumlah instance entitas yang dapat terlibat dalam hubungan
4. Partisipasi: Menunjukkan apakah partisipasi entitas dalam hubungan wajib atau opsional

Contoh representasi hubungan dalam ERD:
- Garis dengan ujung berbentuk "crow's foot" untuk menunjukkan kardinalitas banyak
- Garis lurus untuk menunjukkan kardinalitas satu
- Lingkaran pada garis untuk menunjukkan partisipasi opsional
- Garis vertikal pada garis untuk menunjukkan partisipasi wajib

Misalnya, hubungan antara "Mahasiswa" dan "Kelas" bisa digambarkan dengan garis yang memiliki crow's foot di kedua ujungnya, menunjukkan hubungan banyak-ke-banyak.

## 13. Apa perbedaan antara hubungan satu-ke-banyak (one-to-many) dan hubungan banyak-ke-banyak (many-to-many) dalam ERD? (Point : 8)

Perbedaan antara hubungan satu-ke-banyak (one-to-many) dan banyak-ke-banyak (many-to-many) dalam ERD:

Hubungan Satu-ke-Banyak (One-to-Many):
1. Satu instance dari entitas A dapat berhubungan dengan banyak instance dari entitas B
2. Namun, satu instance dari entitas B hanya dapat berhubungan dengan satu instance dari entitas A
3. Direpresentasikan dengan crow's foot di sisi "banyak" dan garis lurus di sisi "satu"
4. Contoh: Satu departemen memiliki banyak karyawan

Hubungan Banyak-ke-Banyak (Many-to-Many):
1. Satu instance dari entitas A dapat berhubungan dengan banyak instance dari entitas B
2. Satu instance dari entitas B juga dapat berhubungan dengan banyak instance dari entitas A
3. Direpresentasikan dengan crow's foot di kedua sisi hubungan
4. Dalam implementasi basis data relasional, hubungan ini biasanya memerlukan tabel junction
5. Contoh: Mahasiswa dapat mengambil banyak mata kuliah, dan satu mata kuliah dapat diambil oleh banyak mahasiswa

Implementasi:
- One-to-Many: Biasanya diimplementasikan dengan foreign key pada entitas "banyak"
- Many-to-Many: Memerlukan tabel tambahan (junction table) yang berisi foreign key dari kedua entitas

## 14. Apa yang dimaksud dengan kardinalitas dalam hubungan ERD, dan bagaimana kardinalitas dijelaskan dalam diagram ERD? (Point : 8)

Dalam diagram Entity-Relationship (ERD), kardinalitas mengacu pada jumlah maksimum entitas yang dapat dihubungkan ke satu entitas lain melalui sebuah relationship. Kardinalitas menentukan batasan partisipasi antara entitas yang terkait.
Berikut adalah penjelasan tentang bagaimana kardinalitas dijelaskan dalam diagram ERD:

- One-to-One (1:1)
Setiap entitas A terhubung dengan paling banyak satu entitas B, dan sebaliknya.
Digambarkan dengan garis tunggal yang menghubungkan kedua entitas.
Contoh: Satu karyawan memiliki satu ID karyawan yang unik.


- One-to-Many (1:N)
Satu entitas A dapat terhubung dengan banyak entitas B, tetapi setiap entitas B hanya dapat terhubung dengan satu entitas A.
Digambarkan dengan garis tunggal dari entitas A ke entitas B, dengan simbol kardinalitas (1 di sisi A dan N di sisi B).
Contoh: Satu departemen dapat memiliki banyak karyawan, tetapi setiap karyawan hanya terhubung ke satu departemen.


- Many-to-One (N:1)
Banyak entitas A dapat terhubung ke satu entitas B, tetapi setiap entitas A hanya dapat terhubung ke satu entitas B.
Digambarkan dengan garis tunggal dari entitas A ke entitas B, dengan simbol kardinalitas (N di sisi A dan 1 di sisi B).
Contoh: Banyak karyawan dapat terhubung ke satu manajer, tetapi setiap karyawan hanya memiliki satu manajer.


- Many-to-Many (M:N)
Banyak entitas A dapat terhubung dengan banyak entitas B, dan sebaliknya.
Digambarkan dengan dua garis yang menghubungkan kedua entitas, dengan simbol kardinalitas (M di satu sisi dan N di sisi lainnya).
Contoh: Seorang mahasiswa dapat mengambil banyak mata kuliah, dan setiap mata kuliah dapat diambil oleh banyak mahasiswa.

## 15. Bagaimana langkah-langkah dasar dalam merancang basis data yang efisien berdasarkan ERD? (Point : 8)
Langkah-langkah Dasar Merancang Basis Data yang Efisien Berdasarkan ERD

1. **Identifikasi entitas**: 
   Tentukan objek utama yang akan disimpan dalam database.

2. **Tentukan atribut**: 
   Identifikasi properti atau karakteristik dari setiap entitas.

3. **Identifikasi relasi**: 
   Tentukan hubungan antar entitas.

4. **Tentukan kardinalitas**: 
   Tetapkan batasan hubungan antar entitas.

5. **Normalisasi**: 
   Terapkan aturan normalisasi untuk menghindari redundansi data.

6. **Tentukan kunci utama dan kunci asing**: 
   Pilih atribut unik sebagai kunci utama dan tentukan kunci asing untuk menghubungkan tabel.

7. **Buat diagram ERD**: 
   Gambarkan entitas, atribut, dan relasi dalam bentuk diagram.

8. **Validasi dan revisi**: 
   Periksa kembali ERD untuk memastikan semua kebutuhan terpenuhi.

9. **Terjemahkan ERD ke skema basis data**: 
   Konversi ERD menjadi struktur tabel dalam sistem manajemen basis data.

10. **Implementasi**: 
    Buat tabel fisik dalam sistem basis data yang dipilih.

11. **Uji dan optimasi**: 
    Lakukan pengujian untuk memastikan basis data berfungsi sesuai kebutuhan dan optimalkan jika diperlukan.

