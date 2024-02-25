---

banner: Screenshot 2023-09-07 144033.png

sticker: emoji//1f4bb

---

# Basis Data
Basis Data berasal dari 2 karakter yaitu basis dan data

Basis adalah tempat dimana data-data berkumpul. Contoh konkritnya yaitu lemari arsip yang menyimpan arsip data/dokumen dan objek data lainnya

Data adalah kumpulan informasi terkait sebuah objek yang berguna.

Jadi **Basis Data** adalah basecamp atau tempat menyimpan data-data untuk kepentingan web kita. Basis Data sendiri memiliki manfaat yaitu untuk menyimpan data-data atau menampung data-data yang masuk ke dalam website kita.

Contoh penerapannya misalnya, dalam website rumah makan database yang digunakan untuk menampung data-data yang berisi tentang informasi mengenai invetaris , menu makanan, harga, dan sebagainya. Intinya, database akan menampung hal-hal yang ada di dalam rumah makan tersebut, untuk kepentingan website nya.

Didalam database, terdapat lagi tabel-tabel yang berisi data-data yang sudah diampung tersebut. Strukturnya misalnya adalah sebagai berikut:

![[WhatsApp Image 2023-10-01 at 22.31.19.jpg]]
Tabel-tabel itu sendiri dibuat menggunakan sistem MySql.

# MySql

MySQL adalah sebuah sistem manajemen basis data (DBMS) relasional yang bersifat open source. Ini berarti MySQL adalah perangkat lunak yang digunakan untuk menyimpan, mengelola, dan mengakses data dalam bentuk tabel terstruktur dengan menggunakan bahasa query SQL (Structured Query Language). Tujuan utama dari MySQL adalah:

1. **Penyimpanan Data**: MySQL digunakan untuk menyimpan berbagai jenis data, seperti data pelanggan, produk, transaksi, dan banyak lagi, dalam tabel yang terorganisir.
2. **Manipulasi Data**: MySQL memungkinkan pengguna untuk menambah, mengubah, menghapus, dan mengambil data dari basis data dengan menggunakan perintah SQL.
3. **Keamanan Data**: MySQL memiliki fitur keamanan yang dapat mengatur hak akses pengguna, mencegah akses tidak sah, dan melindungi data dari kerusakan atau kehilangan.
4. **Kinerja Tinggi**: MySQL dirancang untuk menangani beban kerja tinggi dengan cepat dan efisien, sehingga cocok untuk aplikasi berkinerja tinggi.
5. **Skalabilitas**: MySQL dapat diatur dan diubah ukurannya sesuai dengan kebutuhan, sehingga bisa mengatasi pertumbuhan data yang besar.
6. **Dukungan Multiplatform**: MySQL dapat dijalankan pada berbagai platform, termasuk Linux, Windows, dan macOS.
7. **Open Source**: Sebagai perangkat lunak open source, MySQL dapat digunakan secara gratis dan memiliki komunitas pengguna yang aktif yang menyediakan dukungan dan pengembangan tambahan.
8. **Integrasi dengan Bahasa Pemrograman**: MySQL dapat digunakan dengan berbagai bahasa pemrograman, seperti PHP, Python, Java, dan lainnya, untuk mengembangkan aplikasi berbasis data.

Secara singkat, MySQL adalah sebuah sistem basis data yang digunakan untuk menyimpan, mengelola, dan mengakses data dengan tujuan untuk mendukung aplikasi berbasis data yang beragam.

struktur database MySql:

**Database --> Tabel --> Field dan Record --> Item  Data**

1. Tabel: Tabel adalah tempat menympan data dalam website kita. Didalam tabel, terdapat Field dan Record, dan item data.

2. Record: adalah kolom yang diisi nama atau data field sedangkan Field adalah judul dari data tersebut, yang membuatnya terbagi menjadi beberapa kelompok. Sedangkan item data adalah isi data yang yang dimasukan dalam website

![[WhatsApp Image 2023-10-01 at 21.54.11 1.jpg]]

Berikut cara mengaktifkan MySql untuk basis data:

1. Buka XAMPP

![[Screenshot 2023-09-07 141730 1.png]]

  

2. Klik Start di *MySql*.

![[Screenshot 2023-09-07 141925.png]]

  

3. Klik Shell

![[Screenshot 2023-09-07 141934 1.png]]


4. Masuk ke database dengan akun administrator dengan cara mengetik *mysl -u root -p*.`

```sql
#mysql -u root -p
```
**Analisis Query:**

Perintah `mysql -u root -p` digunakan untuk mengakses server MySQL melalui baris perintah dengan spesifikasi pengguna (user) yang akan digunakan dan meminta kata sandi (password) untuk autentikasi. Mari saya jelaskan setiap komponen dari perintah ini:

- `mysql`: Ini adalah perintah yang digunakan untuk memulai klien MySQL di baris perintah. Klien MySQL memungkinkan kita untuk berinteraksi dengan server MySQL.

- `-u root`: Bagian ini mengeset pengguna (user) yang akan digunakan saat terhubung ke server MySQL. Dalam contoh ini, pengguna yang digunakan adalah "root." Pengguna "root" biasanya memiliki hak akses penuh ke server MySQL dan dapat melakukan tindakan administratif.

- `-p`: Opsi ini digunakan untuk meminta kata sandi (password) setelah perintah dijalankan. Ini adalah langkah keamanan yang umum digunakan untuk memastikan hanya pengguna yang sah yang dapat mengakses server MySQL. Setelah kita menekan Enter setelah perintah ini, kita akan diminta memasukkan kata sandi untuk pengguna "root."

Jadi, secara keseluruhan, perintah `mysql -u root -p` digunakan untuk melakukan koneksi ke server MySQL dengan pengguna "root" dan meminta kata sandi pengguna tersebut untuk autentikasi. Setelah berhasil masuk, kita akan masuk ke prompt MySQL di mana kita dapat menjalankan perintah SQL untuk mengelola basis data, mengambil data, atau melakukan tugas-tugas lainnya terkait MySQL.

**Kesimpulan:**
Perintah  `mysql -u root -p` ini adalah perintah untuk memanggil mysql.

5. Setelah itu akan tampil *Enter Password:*. Pada bagian ini, dikosongkan saja dengan cara langsung mengklik enter.

```sql
# mysql -u root -p
Enter password:
```

Hasil:

![[Screenshot 2023-09-07 142118.png]]

**Analisis Query:**

Perintah "Enter password" di MySQL adalah pesan yang akan muncul setelah kita menjalankan perintah `mysql -u root -p` atau perintah serupa yang menggunakan opsi `-p` untuk autentikasi dengan pengguna dan meminta kata sandi. Pesan ini menunjukkan bahwa sistem meminta kita untuk memasukkan kata sandi pengguna yang telah kita tentukan dengan opsi `-u` (dalam contoh ini, pengguna "root").

Saat pesan "Enter password" muncul, kita harus mengetikkan kata sandi yang sesuai dengan pengguna yang kita gunakan. Biasanya, karakter yang kita ketikkan tidak akan ditampilkan di layar, sehingga ini merupakan langkah keamanan yang umum digunakan untuk melindungi kata sandi dari mata orang lain yang mungkin melihat layar kita. Namun untuk akun administrator, biasa akan dikosongkan saja.  

Setelah kita memasukkan kata sandi dengan benar dan menekan tombol Enter, MySQL akan memeriksa kata sandi yang kita berikan. Jika kata sandi yang dimasukkan sesuai dengan yang terdaftar dalam database MySQL, kita akan berhasil masuk ke prompt MySQL, di mana kita dapat menjalankan perintah SQL atau melakukan tindakan lainnya pada server MySQL. Jika kata sandi yang dimasukkan salah, kita akan diberi kesempatan untuk mencoba lagi atau perintah akan ditolak jika kita mencapai batas percobaan yang ditentukan oleh konfigurasi MySQL.

**Kesimpulan:**

Enter Password sama halnya dengan memasukan kata sandi email agar kita bisa memakai akun email tersebut. Namun untuk akun administrator biasanyaakan dikosongkan

6. Kemudian kita akan diarahkan ke MariaDB monitor

![[Screenshot 2023-09-07 142200.png]]

# Tipe Data

Tipe data dalam MySQL adalah aturan yang menentukan jenis nilai yang dapat disimpan dalam kolom tabel database. Ini memberikan struktur dan format data dalam database, memungkinkan pengguna untuk mengontrol jenis data yang dapat dimasukkan dan operasi yang dapat dilakukan pada data tersebut, seperti perhitungan matematika, perbandingan, dan pencarian. MySQL memiliki berbagai tipe data, termasuk tipe data angka, teks, tanggal, dan waktu, yang digunakan untuk menyimpan jenis data yang berbeda dalam tabel database.

Dalam MySQL, terdapat beberapa tipe data yang umum digunakan, di antaranya:

1. **Tipe Data Angka**:
    - `INT` (Integer): Digunakan untuk menyimpan bilangan bulat, seperti 1, 42, -10.

    - `DECIMAL` atau `NUMERIC`: Digunakan untuk menyimpan angka desimal dengan presisi tertentu, seperti 3.14, 123.456.
1. **Tipe Data Teks**:
    - `VARCHAR`: Digunakan untuk menyimpan teks dengan panjang variabel, seperti nama, alamat email.
    - `CHAR`: Digunakan untuk menyimpan teks dengan panjang tetap, seperti kode pos.
    - `TEXT`: Digunakan untuk teks panjang seperti deskripsi atau catatan.
3. **Tipe Data Tanggal dan Waktu**:
    - `DATE`: Digunakan untuk menyimpan tanggal, seperti "2023-10-01".
    - `TIME`: Digunakan untuk menyimpan waktu, seperti "15:30:00".
    - `DATETIME`: Digunakan untuk menyimpan tanggal dan waktu, seperti "2023-10-01 15:30:00".
4. **Tipe Data Boolean**:
    - `BOOLEAN` atau `BOOL`: Digunakan untuk menyimpan nilai benar (true) atau salah (false).
   
Contoh penggunaan tipe data ini dalam tabel MySQL

```mysql
CREATE TABLE Mahasiswa (

    id INT AUTO_INCREMENT PRIMARY KEY,

    nama VARCHAR(50),

    umur INT,

    tanggal_lahir DATE
);
```
Dalam contoh di atas, kita membuat tabel "Mahasiswa" dengan beberapa kolom menggunakan tipe data yang umum digunakan, seperti `INT`, `VARCHAR`, dan `DATE`.
# Perintah-Perintah Umum
Terdapat 4 perintah umum dalam menyusun tabel dalam database Mysql yaitu:
1. Primary Key

2. Unique Key

3. Null

4. Not

Primary Key berfungsi sebagai penentu atau patokan sebuah keakuratan data agar tidak terjadi duplikasi data. Misalnya pada database daftar guru, yang menjadi primary key nya adalah NIP nya, agar jika ada nama guru yang sama, datanya tidak akan terduplikasi karena bagian NIP nya tidak sama dan tentunya sudah diberikan Primary Key. Primary Key mengidentifikasi data yang unik perbaris dalam tabel untuk dijadikan acuan data.

Unique Key berfungsi untuk mengidentifikasi data yang unik perbaris dalam kolom dan 1 tabel dalam database dapat memiliki lebih dari 1 Unique key. Biasanya digunakan sebagai acuan kedua, jika data yang di berikan Primary Key tetap sama.

Null: Nilai yang menunjukan bahwa data dalam kolom tertentu tidak memiliki nilai. Contoh: pada database data guru, kolom *Keterangan* tidak perlu diisi, maka digunakanlah perintah Null oada kolom tersebut.

Not: Operator logika untuk membalikan kondisi logika dalam MySql. Ini digunakan untuk memeriksa ketia kondisi yang dinyatakan tidak terpenuhi. Contoh: Data guru, nama guru tidak dapat kosong maka diberikan keterangan NOT NULL pada kolom nama guru.
# Membuat Database

1. Untuk melihat database yang telah tersedia, ketik **SHOW DATABASES;**. Maka program akan menunjukkan tabel daftar data base.

**Struktur Query:**

```sql
SHOW DATABASES;
```
**Contoh Query**: 
```sql
SHOW DATABASES;
```
Hasil:
![[Screenshot 2023-09-07 142309.png]]

**Analisis conth Query:**
Perintah `SHOW DATABASES;` dalam SQL digunakan untuk menampilkan daftar semua basis data yang ada dalam sistem manajemen basis data (DBMS) yang sedang digunakan. Ini adalah perintah yang berguna untuk melihat daftar semua basis data yang tersedia, termasuk yang aktif dan yang sudah ada.

Hasilnya akan menampilkan daftar basis data yang dapat diakses oleh pengguna saat ini, yang biasanya termasuk basis data sistem dan basis data yang mungkin telah dibuat oleh pengguna. Perintah ini sering digunakan untuk menjelajahi struktur basis data yang tersedia dalam DBMS dan memilih basis data yang ingin digunakan untuk menjalankan perintah SQL selanjutnya.

**Kesimpulan:**

Perintah SHOW DATABASES digunakan untuk menampilkan daftar database yang sudah kita buat.
  
2. Untuk membuat database baru kita akan meggunakan perintah **CREATE DATABASES**

**Struktur Query:**
```sql
CREATE DATABASE nama_database;
```
**Contoh:**
```sql
CREATE DATABASE nama;
```
Hasil:

![[Screenshot 2023-10-01 224958.png]]

**Analisis Query:**

Perintah `CREATE DATABASE` dalam MySQL digunakan untuk membuat basis data baru dalam sistem manajemen basis data MySQL. Ini memungkinkan kita untuk membuat wadah atau tempat untuk menyimpan tabel, data, dan objek database lainnya.

**Kesimpulan:**
Create Database digunakan untuk membuat database baru

3. Untuk menghapus database, ketik **DROP DATABASE nama;**.

**Struktur Query:**
```sql
DROP DATABASE nama_databasenya;
```
**Contoh Query:**
```sql
DROP DATABASE nama;
```
Hasil:

![[Screenshot 2023-10-01 225316.png]]

**Analisis Query:**
Perintah `DROP DATABASE` dalam MySQL digunakan untuk menghapus sebuah basis data beserta semua tabel, indeks, dan objek lainnya yang ada di dalamnya secara permanen. Ini adalah perintah yang sangat kuat dan perlu digunakan dengan sangat hati-hati karena tidak ada cara untuk menampilkan data yang telah dihapus setelah perintah ini dijalankan. Berikut adalah sintaks umum perintah `DROP DATABASE`:
```sql
DROP DATABASE nama_database;
```
Di mana:

- `nama_database` adalah nama basis data yang ingin kita hapus.  

Perintah `DROP DATABASE` sebaiknya hanya digunakan jika kita benar-benar yakin bahwa kita tidak lagi memerlukan basis data tersebut dan kita telah melakukan semua tindakan perlindungan yang diperlukan terhadap data yang ada di dalamnya.

**Kesimpulan:**
Drop database digunakan untuk menghapus database yang sudah tidak diperlukan lagi.

4. Untuk menggunakan database yang sudah kita buat, kita akan menggunakan perintah **USE**.

**Analisis Query:**
```sql
USE nama_databasenya;
```
**Contoh Query:**
```sql
USE test;
```
Hasil:
![[Screenshot 2023-10-01 225802.png]]

 **Analisis Query:**

 Perintah `USE` dalam SQL digunakan untuk mengganti basis data aktif yang sedang digunakan oleh sesi SQL. Ketika kita menggunakan perintah `USE`, kita mengindikasikan kepada sistem bahwa semua perintah SQL selanjutnya akan berlaku untuk basis data yang ditentukan. Berikut adalah sintaks umum dari perintah `USE`:
```sql
USE nama_database;
```  
Di mana:
- `nama_database` adalah nama basis data yang ingin kita aktifkan.

Namun, perlu diingat bahwa perintah `USE` hanya mempengaruhi sesi SQL saat itu. Ketika sesi SQL ditutup atau jika kita memulai sesi SQL baru, kita harus menggunakan perintah `USE` lagi untuk mengaktifkan basis data yang sesuai untuk sesi tersebut.

**Kesimpulan:**
Use digunakan untuk menggunakan/mengaktifkan database yang akan digunakan, sehingga kita bisa mengatur aktifitas database yang digunakan

# Membuat tabel di database

Untuk membuat tabel kita perlu menggunakan salah satu database. Caranya yaitu menggunakan perintah Use tadi: 

1. Masuklah ke database yang sudah kita buat, dengan cara ketik **USE toko_condrado;**.
```sql
USE toko_condrado;
```
Hasil:
![[Screenshot 2023-09-07 142451.png]]

**Analisis Query:**
Jadi kita akan membuat tabel di dalam database toko_condrado, oleh karena itu kita akan menggunakan/mengaktifkan database tersebut dengan cara mengetikkan `USE toko_condrado`. Jika sudah ada perintah `MariaDB [toko_condrado]>` artinya database kita sudah berhasil diaktifkan.

**Kesimpulan:**
Jika kita ingin mengaktifkan database kita, maka gunakanlah perintah USE.

2. untuk mulai membuat tabel maka perintah yang digunakan adalah **create table**.

**Struktur Query:**
```sql
create table nama_tabel_yang_akan_dibuat
```
**Contoh Query:**
```sql
create table pelanggan
```
Hasil:
![[Screenshot 2023-09-07 143149.png]]

**Analisis Query:**
Kita akan membuat tabel bernama pelanggan di dalam database toko_condrado. Caranya yaitu menggunakan perintah create table diikuti oleh nama tabel yang mau dibuat. Contohnya yaitu: `create tabel pelanggan`. Dimana:
- `pelanggan` adalah nama dari tabel yang dibuat
- `create table` adalah perintah untuk membuat tabel.\

**Kesimpulan:**
Untuk membuat tabel, ketiklah perintah `create table` diikut dengan nama tabel yang akan dibuat.

3. Selanjutnya adalah membuat field yang ada dalam tabel:

**Struktur Query:**
```sql
create table nama_table (
    --> nama_field_1 tipe_data(MAX) Ket_Null Ket_primary key,
    --> nama_field_2 tipe_data(MAX) Ket_Null unique (opsional),
    --> nama_field_3 tipe_data(MAX) Ket_Null unique (opsional),
    --> nama_field_4 tipe_data(MAX) Ket_Null unique (opsional)
    -->);
)
```
**Contoh Query:**
```sql
create table pelanggan (
    --> id_pelanggan int(4) not null primary key,
    --> nama_depan varchar(25) not null,
    --> nama_belakang varchar(25) not null,
    --> no_telp char(12) unique
    -->);
)
```
Hasil:
![[Screenshot 2023-09-07 143952.png]]

**Analisis Query:**
jadi secara urutan adalah: nama field, tipe data(jumlah karakter) dan keterangan perintahnya.
terdapat 5 baris yang dimana baris 1 sampai 4 adalah daftar field yang akan dibuat pada tabel kita sedangkan yang ke 5 adalah penutup.
id pelanggan diberikan primary key, sedangkan no_telp diberikan unique key.
pada bagian no_telp diberikan juga tidak diberikan keterangan not null, sehingga isi data dari no_telp bisa dikosongkan
Jika sudah tekan Enter.

**Kesimpulan:**
Perintah-perintah yang dituliskan bertujuan untuk membuat filed dari tabel tersebut.

4. Kemudian adalah memeriksa atau melihat tabel yang telah dibuat menggunakan perintah **show tables;**.

```sql
show tables;
```
Hasil:
![[Screenshot 2023-09-07 144033.png]]

**Analisis Query:**
Pada database toko_condrado terdapat 1 tabel yaitu bernama table "pelanggan", yang tadi kita sudah buat. Sama halnya dengan melihat daftar database yang ada di akun administrator, kita juga akan melihat daftar tabel yang sudah kita buat dengan cara mengetikkan sintaks `show tables;`. Jika sudah muncul daftar tabel seperti pada gambar hasil, maka artinya tabel sudah berhasil kita buat.

**Kesimpulan:**
Perintah `show tables;` digunakan untuk melihat daftar tabel yang ada di database yang sedang diaktifkan.

8. Untuk mengecek atribut/field dari tabel tersebut caranya yaitu ketik **desc nama_table**. Contoh: desc pelanggan.
```sql
desc pelanggan;
```
Hasil:
![[Screenshot 2023-09-07 144116.png]]

**Analisis Query:**
Jadi setelah kita membuat tabel dan setelah kita cek ternyata sudah berhasil, maka selanjutnya adalah mengecek field yang sudah kita buat pula. Caranya yaitu dengan mengetikkan sintaks `desc pelanggan;`. dimana:
- `desc`: perintah untuk menampilkan filed tabel tersebut.
- `pelanggan`: nama tabel yang mau dicek des nya.

**Kesimpulan:**
Jadi perintah `desc pelanggan` adalah untuk melihat field atau atribut dari tabel pelanggan.

# INSERT

1. sekarang kita akan memanipulasi data yang ada dalam tabel akun. yang pertama adalah memasukan data. Caranya yaitu menggunakan perintah **INSERT INTO akun** lalu dienter.

**Analisis Query:**
```sql
INSERT INTO nama_table
   --> values(item_1,'item_2','item_3','item_3');
```
**Contoh Query:**
```sql
INSERT INTO akun
   --> values(1,'condrado','admin','123');
```
Hasil:
![[Screenshot 2023-09-21 150621 1.png]]

**Analisis Query:**
Perintah `INSERT INTO` dalam MySQL digunakan untuk menyisipkan (insert) data baru ke dalam sebuah tabel dalam basis data MySQL. Dengan perintah ini, kita dapat menambahkan baris-baris data baru ke dalam tabel yang telah kita tentukan. Pada praktek ini diketikkan `INSERT INTO akun` yang artinya masukan data pada tabel akun, dan `values (1,'1','condrado','admin','123');` berarti nilai yang dimasukan ke dalam tabel. Urutan datanya ialah sesuai filed yang dibuat secara berurutan.

**Kesimpulan:**
Untuk memasukan data gunakan perintah insert into diikuti dengan data-datanya.

2. Untuk menambahkan item data ke dalam tabel database, kita mengenal 2 cara, yaitu dengan menyebutkan nama kolomnya ataupun tidak. Pada praktek sebelumnya, kita mempraktekkan cara menambah item data namun tanpa menyebutkan kolomnya. Namun perlu untuk diingat, bahwasannya urutan item data harus sesuai dengan urutan kolomnya (perhatikan praktikum nomor 1). Kali ini kita akan menambahkan item data walaupun tidak berurutan. CAranya adalah sebagai berikut:

**Struktur Query:**
```sql
INSERT INTO Nama_Tabel 
 -->(Kolom1, Kolom2, Kolom3) 
 -->VALUES (Nilai1, Nilai2, Nilai3);

```
**Contoh Query:**
```sql
INSERT INTO akun
    -> (nama, username, id, password)
    -> VALUES ("Abri","owner",4,"222");
```
Hasil:
![[Screenshot 2023-10-11 220205.png]]

**Analisis Query:**
Pada praktek ini kita telah menambahkan item data yaitu:
- ID: 4
- nama: Abri
- username: owner
- password: 222

Pada sintaks setelah perintah `INSERT INTO akun` terdapat sintaks ``(nama, username, id, password)``. Sintaks inilah yang mengidentifikasi nama kolom yang mau ditambahkan. Ditekankan juga bahwa urutan kolom yang disebutkan tidak berurutan. Hal ini terjadi jika sekitainya kita kan menginput sebuah data yang urutan judul kolomnya tidak sesuai dengan urutan tabel di sql.

**Kesimpulan:**
Pada praktek ini kita telah menambahkan item data dengan menyebutkan nama kolomnya.

# SELEKSI

1. Untuk melihat data yang sudah dimasukan ketik **SELECT * FROM akun;**. Maka program akan menampilkan data yang sudah dimasukan tadi.

**Struktur  Query:**

```sql
SELECT * FROM nama_tabel;
```
**Contoh Query:**
```sql
SELECT * FROM akun;
```
Hasil:
![[Screenshot 2023-09-21 150621.png]]

**Analsis Query:**
jadi kita telah memasukan data sebanyak 3 item ke dalam tabel database kita. Sekarang kita akan melihat apakah data data tersebut telah masuk kedalam tabel database kita. Caranya yaitu mengetikkan sintaks `SELECT*FROM akun;` dimana:
- `SELECT * FROM` adalah perintah untuk melihat item tabel
- `akun` adalah nama tabel yang datanya mau dilihat.

**Kesimpulan:**
Untuk melihat item tabel, maka digunakanlah perintah `SELECT * FROM`.

2. Tadi kita sudah melakukan praktikum yaitu untuk melihat item data pada tabel. Namun item data yang ditampilkan secara keseluruhan, yaitu dimulai dari id,nama username dan password. Nah bagaimana jika kita hanya ingin menampilkan item data "nama" saja? Berikut caranya:

**Struktur Query:**
```sql
SELECT field
    --> FROM nama_akun;
```
**Contoh Query:**
```sql
SELECT nama
    --> FROM akun;
```
Hasil:
![[Screenshot 2023-10-12 075508.png]]

**Analisis Query:**
Jadi pada praktikum sebelumnya kita telah menampilkan item data pada tabel akun. Namun pada praktek kali ini kita hanya akan menampilkan data nama saja. caranya yaitu menggunakan perintah `SELECT` kemudian diikuti oleh judul kolom yang ingin ditampilkan, yaitu 'nama'. Kemudian kita melanjutkannya dengan mengetik perintah `FROM` dan diikuti dengan nama tabel. Dengan cara seperti ini kita telah menampilkan item data pada kolom "nama" pada tabel "akun".

**Kesimpulan:**
jika kita ingin menampilkan itemdata pada kolom tertentu saja, maka gunakan perintah `SELECT`, diikuti oleh `FROM`, dimana select diisi nama kolom yang mau ditampilkan, dan from diisi oleh tabel tempat kita akan mengambil datanya.

# PERBAHARIUI DATA
Sekarang, kita akan mengubah sebuah item data pada tabel. Caranya yaitu kita menggunakan perintah "UPDATE". Berikut cara penggunaannya:

**Struktur Query:**
```sql
UPDATE nama_table
  -> SET field = "Item_data_baru"
  -> WHERE field identifikasi = item_data_identifikasi;
```
**Contoh Query:**
```sql
UPDATE akun
  -> SET nama= "Abri"
  -> WHERE id = 2;
```
Table sebelumnya:
![[Screenshot 2023-10-11 222705.png]]

Hasil:
![[Screenshot 2023-10-11 222711.png]]

**Analisis Query:**

Di sini, penjelasan singkat mengenai setiap bagian perintah UPDATE:

1. `UPDATE`: Ini adalah kata kunci yang menkitakan bahwa kita ingin melakukan operasi pembaruan data.
2. `akun`: Ini adalah nama tabel yang akan kita perbarui.
3. `SET`: Ini adalah kata kunci yang mengikuti nama tabel dan menunjukkan kolom mana yang akan diperbarui dan nilai baru yang akan diatur.
4. `nama= "Abri"`: Ini adalah daftar kolom dan nilai baru yang akan kita atur, yaitu di kolom "nama", dengan nilai baru yaitu "Abri".
5. `WHERE id = 2`: ini adalah sintaks yang digunakan untuk mengidentifikasi letak data yang akan diganti tersebut.

**Kesimpulan:**
Jadi perintah-perintah diatas digunakan untuk mengubah data yang sudah ada di tabel.

# MENGHAPUS DATA
Selanjutnya kita akan mempelajari cara menghapus sebuah data yang telah ada di dalam tabel. Caranya adalah sebagai berikut:
**Struktur Query:**
```sql
DELETE from nama_tabel
   -> WHERE field = item_data_identifikasi;
```
**Contoh Query:**
```sql
DELETE from akun
   -> WHERE id = 4;
```
Tabel sebelumnya:

![[Screenshot 2023-10-11 220205.png]]

Hasil:
![[Screenshot 2023-10-11 221402.png]]

**Analisis Query:**
Jadi kita akan mengahapus item data abri, caranya yaitu mengetikkan terlebih dahulu sintaks `DELETE FROM akun;` . Hal ini dilakukan untuk mengidentifikasi di tabel mana kita akan menghapus item data tertentu.Rupanya yaitu di tabel "akun". Nah di bagian mana datanya mau dihapus? Kita kemudian mengidentifikas nya (biasanya dengan data primary), yaitu mengetikan `WHERE ID= 4`, yang berarti hapus item yang ada di ID 4.

**Kesimpulan:**
Untuk menghapus item data, gunakan perintah `DELETE FROM nama_tabel`, diikut oleh `WHERE kondisi = value`, sebagai perintah untuk mengidentifikasi letak data yang mau dihapus.

# TANTANGAN LOGIN
Pada praktek sebelumnya kita telah menampilkan data nama, namun di praktik ini muncul banyak sekali item data sesuai dengan jumlah item data di nama. Bagaimana jika kita hanya ingin menampilkan 1 data nama saja sesuai id atau identifikasi tertentu? berikut caranya:

**Struktur Query:**
```sql
SELECT field
   --> FROM nama_tabel
   --> where data_identifikasi;
```
**Contoh Query:**
```sql
SELECT nama
   --> FROM akun
   --> where username='admin'&& password=123;
```
Tabel:
![[Screenshot 2023-10-12 081156.png]]

Hasil:
![[Screenshot 2023-10-12 075153.png]]

**Analisis Query:**
Jadi pada praktek ini kita akan menampilkan data nama yang memiliki username 'admin', dan passwordnya = 123. Caranya yaitu menggunakan perintah `SELECT` nama, untuk mengidentifkasi kolom yang mau ditampilkan namanya, kemudian `FROM` akun untuk mengidentifikasi tabel yang mau digunakan, kemudian `WHERE` untuk mengidentifasi letak item data nama tersebut yang mau ditampilkan.

**Kesimpulan:**
Perintah-perintah diatas berfungsi untuk menampilkan 1 data saja dalam sebuah tabel dengan mengidentifikasi letak datanya.
# SELECT LANJUTAN
## Tantangan 2

Sekarang, didalam database rental_mobil_condradp kita akan membuat tabel

**Struktur Query**
```sql
CREATE TABLE nama_tabel(
	nama_kolom1 tipe data(ukuran) [tipe_constraint],
	nama_kolom1 tipe data(ukuran) [tipe_constraint],
);
```
**Contoh Query**
```sql
create table mobil (
	id_mobil int(2) not null PRIMARY KEY,
	no_plat varchar(10) not null UNIQUE,
	no_mesin varchar(10) not null UNIQUE,
	warna varchar(10) not null,
	pemilik varchar(25) not null,
	peminjam varchar(25) not null,
	harga_rental int(10) null
)
```
**Hasil:**
![[Screenshot 2023-10-25 214414.png]]

**Analisis Query:**

1. `create table mobil (`: perintah untuk membuat sebuah tabel yang dinamai "mobil".
2. `id_mobil int(2) not null PRIMARY KEY,`: kolom pertama dalam tabel "mobil". Tipe data kolom ini adalah `int` (bilangan bulat) dengan panjang maksimum 2 digit angka. Perintah `not null` menunjukkan bahwa kolom ini tidak boleh memiliki nilai kosong (NULL), Perintah `PRIMARY KEY` menunjukkan bahwa kolom ini adalah yang menjadi patokan data (primary key.
3. `no_plat varchar(10) not null UNIQUE,`: kolom kedua dengan nama "no_plat". Tipe data kolom ini adalah `varchar` (tipe data karakter panjang) dengan panjang maksimum 10 karakter. perintah `not null` menunjukkan bahwa kolom ini tidak boleh memiliki nilai kosong, dan perintah `UNIQUE` menunjukkan bahwa setiap nilai dalam kolom bersifat unik.
4. `no_mesin varchar(10) not null UNIQUE,`: Ini adalah kolom ketiga dengan nama "no_mesin". Seperti "no_plat", ini juga merupakan kolom `varchar` dengan panjang maksimum 10 karakter. Sama seperti sebelumnya, perintah `not null` dan `UNIQUE` digunakan untuk memastikan bahwa kolom ini tidak boleh kosong dan setiap nilai harus unik.
5. `warna varchar(10) not null,`: Ini adalah kolom keempat dengan nama "warna". Tipe data kolom ini adalah `varchar` dengan panjang maksimum 10 karakter, dan perintahi `not null` menunjukkan bahwa kolom ini tidak boleh kosong.
6. `pemilik varchar(25) not null,`: Ini adalah kolom kelima dengan nama "pemilik". Tipe data kolom ini adalah `varchar` dengan panjang maksimum 25 karakter, dan perintah `not null` menunjukkan bahwa kolom ini tidak boleh kosong.
7. `peminjam varchar(25) not null,`: Ini adalah kolom keenam dengan nama "peminjam". Tipe data kolomini ialah  `varchar` dengan panjang maksimum 25 karakter, dan perintah `not null` digunakan untuk memastikan bahwa kolom ini tidak boleh kosong.
    
8. `harga_rental int(10) null`: Ini adalah kolom terakhir dengan nama "harga_rental". Tipe data kolom ini adalah `int` dengan panjang maksimum 10 digit. Perintah `null` menunjukkan bahwa kolom ini dapat memiliki nilai NULL, yang berarti tidak wajib memiliki nilai (bisa kosong)

**Kesimpulan:**
Kesimpulan: Perintah "create table mobil" digunakan untuk membuat sebuah tabel dengan nama "mobil."
## Tantangan 3

**Kode Query**:
```sql
INSERT INTO MOBIL
VALUE
	(1,"DD 2650 XY", "ACX3560", "HITAM", "Ibrahim", "Afdal", 50000 ),
	(2, "DD 2440 AX", "BCS1120", "MERAH", "Ibrahim", "Elia", 100000),
	(3, "DD 1611 QC", "LSQ1112", "SILVER", "Baim", "Anty", 50000);
```
**Hasil:**
![[Screenshot 2023-10-26 032313.png]]

**Lanjutan Kode Query:**
```sql
INSERT INTO mobil
	(id_mobil, no_plat, no_mesin, warna, pemilik, harga_rental)
	VALUES
	(4, "DD 2901 JK", "UL1029", "HITAM", "Ibhe", 150000),
	(5, "DD 2210 LS", "CJH1011", "HITAM", "Ibhe", 100000);
```
**Hasil:**
![[Screenshot 2023-10-26 031409.png]]

**Analisis Query:**
1. `INSERT INTO MOBIL`: perintah untuk memasukkan data ke dalam tabel "MOBIL."
2. `VALUES`: perintah yang digunakan untuk memasukan nilai ke dalam tabel.
3. `(1, "DD 2650 XY", "ACX3560", "HITAM", "Ibrahim", "Afdal", 50000)`: data pertama yang akan dimasukkan ke dalam tabel "MOBIL." Setiap nilai di dalam tanda kurung merupakan nilai untuk kolom-kolom dalam tabel sesuai urutan ini:
   - Kolom pertama: 1 (nilai ID)
   - Kolom kedua: "DD 2650 XY" (Nomor Plat)
   - Kolom ketiga: "ACX3560" (Nomor Mesin)
   - Kolom keempat: "HITAM" (Warna)
   - Kolom kelima: "Ibrahim" (Pemilik Pertama)
   - Kolom keenam: "Afdal" (Pemilik Sekarang)
   - Kolom ketujuh: 50000 (Harga)
4. `(2, "DD 2440 AX", "BCS1120", "MERAH", "Ibrahim", "Elia", 100000)`: Ini adalah baris kedua dengan data yang serupa dengan baris pertama, tetapi isi datanya berbeda.
5. `(3, "DD 1611 QC", "LSQ1112", "SILVER", "Baim", "Anty", 50000)`: Ini adalah baris ketiga, juga dengan data yang mirip dengan baris pertama, tetapi dengan nilai yang berbeda.
6. pada query yang kedua, akan disi data namun dengan format yang berbeda
7. Query yang kedua ini ditentukan kolom mana yang akan diisi dengan data baru. Kolom yang diisi adalah "id_mobil," "no_plat," "no_mesin," "warna," "pemilik," dan "harga_rental." Ini memungkinkan pengguna untuk mengontrol kolom yang diisi dengan nilai tertentu.
8. Data yang Dimasukkan: Terdapat dua baris data yang dimasukkan. Data ini mewakili dua entri mobil yang berbeda dalam tabel "mobil."

   - Baris Pertama: 
     - id_mobil: 4
     - no_plat: "DD 2901 JK"
     - no_mesin: "UL1029"
     - warna: "HITAM"
     - pemilik: "Ibhe"
     - harga_rental: 150,000

   - Baris Kedua: 
     - id_mobil: 5
     - no_plat: "DD 2210 LS"
     - no_mesin: "CJH1011"
     - warna: "HITAM"
     - pemilik: "Ibhe"
     - harga_rental: 100,000
9. Data yang dimasukkan memiliki nilai yang berbeda untuk setiap kolom, sehingga setiap entri mobil memiliki isi data yang berbeda yang berbeda.

Perbedaan Query 1 dan 2:
1. Format penulisan kolom dan nilai berbeda: Query pertama hanya memberikan nilai untuk beberapa kolom seperti "Id_mobil," "nomor_plat," "nomor _mesin," "warna," "Pemilik," "peminjam," dan "Harga." Sementara query kedua menentukan kolom-kolom yang akan diisi dan nilai yang sesuai untuk setiap kolom.
2. Query pertama menggunakan gaya singkat dengan hanya memberikan nilai untuk kolom yang relevan, sementara query kedua ditentukan kolom mana yang akan diisi dengan nilai dan memberikan judul kolom terlebih dahulu seperti "id_mobil," "no_plat," "no_mesin," "warna," "pemilik," dan "harga_rental."
3. Jumlah baris data yang dimasukkan berbeda: Query pertama memasukkan 3 baris data, sementara query kedua hanya memasukkan 2 baris data.

**Kesimpulan:**
Dengan demikian, meskipun kedua query ini digunakan untuk tujuan yang sama, yaitu memasukkan data ke dalam tabel "MOBIL," mereka memiliki perbedaan dalam format dan data yang dimasukkan.


## SELECT (AND)

Select (and) adalah perintah yang digunakan untuk menampilkan 2 data secara bersamaan

**Struktur Query:**
```sql
SELECT * FROM nama_tabel
WHERE kondisi1 AND kondisi2;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
WHERE warna = "HITAM" AND pemilik = "Ibhe";
```
**Hasil:**
![[Screenshot 2023-10-26 040227.png]]
**Analisis Query:**
1. `SELECT *`: Ini adalah perintah untuk menampilkan data dari tabel "mobil." Dengan menggunakan tanda `*`, query akan mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menentukan tabel sumber data yang akan digunakan untuk mengambil data, yaitu tabel "mobil."
3. `WHERE warna = "HITAM" AND pemilik = "Ibhe"`: Perintah`WHERE` digunakan untuk menentukan kondisi atau kriteria yang harus dipenuhi untuk ditampilkan ke dalam hasil query. Dalam kasus ini, terdapat dua kondisi yang digunakan bersamaan dengan operator "AND":
   - Kondisi pertama adalah "warna = 'HITAM'," yang akan memfilter data mobil dengan warna "HITAM."
   - Kondisi kedua adalah "pemilik = 'Ibhe'," yang akan memfilter data mobil yang dimiliki oleh "Ibhe."

**Kesimpulan:**
Dengan menggabungkan kedua kondisi dengan "AND," query ini akan menampilkan data mobil dari tabel "mobil" yang memenuhi kedua kondisi tersebut, yaitu mobil dengan warna "HITAM" yang dimiliki oleh "Ibhe."
Hasil query ini akan menghasilkan daftar mobil dengan warna hitam yang dimiliki oleh "Ibhe" dari tabel "mobil."

## Select (OR)
pernyataan `SELECT` dengan operator "OR" digunakan untuk mengambil data dari tabel yang memenuhi salah satu dari beberapa kondisi yang diberikan dalam perintah `WHERE`. 

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE kondisi1 OR kondisi2 OR kondisi3 OR ...
```
**Contoh Query:**
```sql
SELECT FROM mobil
WHERE pemilik = "Ibrahim" OR warna= "HITAM";
```
**Hasil:**
![[Screenshot 2023-10-26 040959.png]]

**Analisis Query:**
1. `SELECT *`: perintah untuk menampilkan semua data (field) dari tabel "mobil." Dengan menggunakan tanda `*`, query akan mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menentukan tabel sumber data yang akan digunakan untuk mengambil informasi, yaitu tabel "mobil."
3. `WHERE pemilik = "Ibrahim" OR warna= "HITAM"`:`WHERE` yang digunakan untuk menyaring data dengan menggabungkan dua kondisi menggunakan "OR." Dalam query ini, terdapat dua kondisi yang digunakan bersamaan dengan operator "OR":
    - Kondisi pertama adalah "pemilik = 'Ibrahim'," yang akan memasukkan data mobil yang dimiliki oleh "Ibrahim."
    - Kondisi kedua adalah "warna = 'HITAM'," yang akan memasukkan data mobil dengan warna "HITAM."
    
**Kesimpulan:**
Jadi, "OR" digunakan dalam perintah `WHERE` untuk menampilkan 2  kondisi jika setidaknya salah satu dari kondisi tersebut benar.

## Select (Between) & (AND)
Select (Between) dan (AND) digunakan untuk mengambil data yang berada dalam rentang (range) tertentu dari tabel.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE kolom X BETWEEN nilai_awal AND nilai_akhir;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
WHERE harga_rental BETWEEN 50000 AND 100000;
```
**Hasil:**
![[Screenshot 2023-10-26 041840.png]]

**Analisis Query:**
1. `SELECT *`: perintah untuk menampilkan semua kolom (field) dari tabel "mobil." Dengan menggunakan tanda `*`, query akan mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menentukan tabel sumber data yang akan digunakan untuk mengambil informasi, yaitu tabel "mobil."
3. `WHERE harga_rental BETWEEN 50000 AND 100000`: Ini adalah perintah `WHERE` yang digunakan untuk menyaring data. Dalam kasus ini, digunakan perintah `BETWEEN` dengan `AND`:
    - `harga_rental BETWEEN 50000 AND 100000` akan menampilkan data mobil yang memiliki nilai dalam kolom "harga_rental" di antara 50,000 dan 100,000.
    - perintah `BETWEEN` digunakan untuk menentukan rentang harga rental yang diinginkan.
    - Operator `AND` digunakan untuk menghubungkan kedua nilai, yaitu 50,000 (nilai awal) dan 100,000 (nilai akhir) dalam perintah `BETWEEN`

**Kesimpulan:**
Hasil query ini adalah daftar mobil yang memiliki harga rental di antara 50,000 dan 100,000. Dengan kata lain, query ini akan menampilkan mobil yang memenuhi kriteria harga rental tertentu

## Select (NOT BETWEEN) & (AND)
Select (NOT BETWEEN) & (AND) untuk mengambil data yang berada di luar rentang tertentu.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE kolomX NOT BETWEEN nilai_awal AND nilai_akhir;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
WHERE harga_rental NOT BETWEEN 50000 AND 100000;
```
**Hasil:**
![[Screenshot 2023-10-26 042539.png]]

**Analisis Query:**
1. `SELECT *`: perintah untuk menampilkan semua kolom (field) dari tabel "mobil." Dengan menggunakan tanda `*`, query akan mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menentukan tabel sumber data yang akan digunakan untuk mengambil informasi, yaitu tabel "mobil."
3. `WHERE harga_rental NOT BETWEEN 50000 AND 100000`: Ini adalah perintah `WHERE` yang digunakan untuk menyaring data. Dalam kasus ini, digunakan perintah `NOT BETWEEN` dengan `AND`:
	- `harga_rental NOT BETWEEN 50000 AND 100000` akan memasukkan data mobil yang memiliki harga rental di luar rentang 50,000 hingga 100,000.
	- Perintah `NOT BETWEEN` digunakan untuk menentukan bahwa data yang diambil tidak boleh berada dalam rentang tersebut.
	- Operator `AND` digunakan untuk menghubungkan kedua nilai, yaitu 50,000 (nilai awal) dan 100,000 (nilai akhir) dalam Perintah `NOT BETWEEN`.

**Kesimpulan:**
Hasil query ini adalah daftar mobil yang memiliki harga rental di luar rentang 50,000 hingga 100,000, yaitu 150000 Dengan kata lain, query ini akan menampilkan mobil yang memenuhi kriteria harga rental yang berada di luar rentang tersebut.

## Select (<>)
Dalam SQL, operator `< >` (tidak sama dengan) digunakan untuk membandingkan apakah dua nilai atau ekspresi tidak sama. Ini adalah operator perbandingan yang menampilkan hasil `TRUE` jika kedua nilai yang dibandingkan tidak sama, dan `FALSE` jika sama. Operator `< >` dapat digunakan dalam pernyataan `SELECT` untuk mengambil data yang memenuhi kondisi di mana dua nilai tidak sama.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE kolomX <> nilai_tidak_diinginkan;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
WHERE warna <> "HITAM";
```
**Hasil:**
![[Screenshot 2023-10-26 043245.png]]

**Analisis Query:**
1. `SELECT *`: perintah untuk menampilkan data (field) dari tabel "mobil." Dengan menggunakan tanda `*`, query akan mengambil data semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menentukan tabel sumber data yang akan digunakan untuk menampilkan data, yaitu tabel "mobil."
3. `WHERE warna <> "HITAM"`: Ini adalah perintah `WHERE` yang digunakan untuk menyaring data. Dalam kasus ini, operator `<>` digunakan untuk memeriksa apakah nilai dalam kolom "warna" tidak sama dengan "HITAM."

**Kesimpulan:**
Hasil query ini adalah daftar mobil yang memiliki warna yang tidak sama dengan "HITAM." Dengan kata lain, query ini akan menampilkan mobil-mobil yang memiliki warna berbeda, seperti mobil dengan warna merah, biru, hijau, dan sebagainya.

## Select (!=)
Operator `!=` memiliki arti yang sama dengan operator `<>`, yang juga digunakan untuk menunjukkan ketidakkesamaan. Ini adalah operator perbandingan yang menampilkan hasil `TRUE` jika kedua nilai yang dibandingkan tidak sama, dan `FALSE` jika sama.

**Struktur Query:**
```sql
SELECT [kolom1, kolom2, ...]
FROM nama_tabel
WHERE kolomX != nilai_tidak_diinginkan;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
WHERE pemilik != "Ibrahim";
```
**Hasil:**
![[Screenshot 2023-10-26 044214.png]]

**Analisis Query:**

1. `SELECT *`: Ini adalah perintah untuk mengambil semua kolom (field) dari tabel "mobil." Dengan menggunakan tanda `*`, query akan mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menentukan tabel sumber data yang akan digunakan untuk mengambil informasi, yaitu tabel "mobil."
3. `WHERE pemilik != "Ibrahim"`: Ini adalah perintah `WHERE` yang digunakan untuk menyaring data. Dalam kasus ini, operator `!=` digunakan untuk memeriksa apakah nilai dalam kolom "pemilik" tidak sama dengan "Ibrahim."

**Kesimpulan:**
Hasil query ini adalah daftar mobil yang memiliki pemilik yang tidak sama dengan "Ibrahim." Dengan kata lain, query ini akan menampilkan mobil yang dimiliki oleh orang lain selain "Ibrahim."

## Select (<=)
Select (<=) sigunakan untuk menyaring data yang tidak lebih besar dari nilai yang ditentukan

**Struktur Query:**
```sql
SELECT [kolom1, kolom2, ...]
FROM nama_tabel
WHERE kolomX <= nilai_tidak_melebihi;
```
**Contoh Query:**
```sql
SELECT*FROM mobil 
WHERE harga_rental <= 100000;
```
**Hasil:**
![[Screenshot 2023-10-26 045348.png]]

**Analisis Query:**

1. `SELECT *`: Ini adalah perintah untuk memilih semua kolom dari tabel "mobil". tanda asterisk (*) digunakan sebagai wildcard untuk mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menunjukkan bahwa kita ingin mengambil data dari tabel yang disebut "mobil". Ini adalah bagian dari perintah `FROM`.
3. `WHERE harga_rental <= 100000`: Ini adalah perintah "WHERE" yang digunakan untuk memberikan syarat atau filter pada data yang akan diambil. Dalam hal ini, kita ingin mengambil hanya baris-baris di mana nilai dalam kolom "harga_rental" kurang dari atau sama dengan 100,000.

**Kesimpulan:**
Jadi, hasil dari query ini akan menjadi daftar semua mobil dalam tabel "mobil" yang memiliki harga rental kurang dari atau sama dengan 100,000.
## Select (>=)
untuk mengambil data dari tabel, sedangkan operator `(>=)` digunakan untuk membandingkan dua nilai numerik untuk melihat apakah nilai di sebelah kiri lebih besar atau sama dengan nilai di sebelah kanan.

**Struktur Query:**
```sql
SELECT column1, column2
FROM table_name
WHERE column_name >= value;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
	WHERE harga_rental >= 100000;
```
**Hasil:**
![[Screenshot 2023-10-26 082539.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah perintah untuk memilih semua kolom dari tabel "mobil". tanda asterisk (*) digunakan sebagai wildcard untuk mengambil semua kolom yang ada dalam tabel.
2. `FROM mobil`: Ini menunjukkan bahwa kita ingin mengambil data dari tabel yang disebut "mobil". Ini adalah bagian dari perintah `FROM`.
3. `WHERE harga_rental >= 100000`: Ini adalah perintah "WHERE" yang digunakan untuk memberikan syarat atau filter pada data yang akan diambil. Dalam hal ini, kita ingin mengambil hanya baris-baris di mana nilai dalam kolom "harga_rental" lebih dari atau sama dengan 100,000.
**Kesimpulan:**
hasil dari query ini adalah menampilkan isi tabel yang mencakup semua mobil yang dapat disewa dengan harga setidaknya 100,000 atau lebih.
# IN
## IN
**Pengertian In**: Perintah In digunakan untuk membandingkan nilai dalam sebuah kolom dengan satu atau lebih nilai dalam daftar. Jika nilai dalam kolom sama dengan salah satu nilai dalam daftar, baris data tersebut akan dimasukkan dalam hasil query.

**Struktur Query dengan In**: 
```sql
SELECT column1, column2
FROM table_name
WHERE column_name IN (value1, value2, ...);
```
**Contoh Query:**
```sql
SELECT*FROM mobil
    WHERE warna IN ("Merah", "Silver");
```
**Hasil:**
![[Screenshot 2023-10-26 095333.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE warna IN ("Merah", "Silver")`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana kolom "warna" memiliki nilai yang sama dengan "Merah" atau "Silver". Dengan kata lain, query ini akan mengambil semua baris dari tabel "mobil" di mana warna mobil adalah Merah atau Silver.

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi kondisi tersebut.
## IN + AND
`IN` dan `AND` adalah dua operator penting dalam SQL yang digunakan untuk menggabungkan kondisi dalam pernyataan SQL.

**Struktur Query:**
```sql
SELECT kolom
FROM tabel
WHERE kondisi_1 AND kondisi_2 AND ... kondisi_n
```
**Contoh querry:**
```sql
SELECT*FROM mobil
    WHERE pemilik = "Ibrahim" AND warna="HITAM";
```
**Hasil:**
![[Screenshot 2023-10-26 101231.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE pemilik = "Ibrahim" AND warna = "HITAM"`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana dua kondisi berikut ini harus terpenuhi:
    - Kolom "pemilik" harus memiliki nilai "Ibrahim."
    - Kolom "warna" harus memiliki nilai "HITAM."

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi kedua kondisi tersebut.
## IN + OR
`IN` dan `OR` adalah dua operator yang digunakan untuk menggabungkan kondisi dalam pernyataan SQL. Mereka digunakan untuk memfilter data dari tabel berdasarkan beberapa kriteria.

**Struktur Query:**
```sql
SELECT kolom
FROM tabel
WHERE (kondisi_1 OR kondisi_2 OR ... kondisi_n) AND (kondisi_a OR kondisi_b OR ... kondisi_z)
```
**Contoh Query:**
```sql
SELECT*FROM mobil
    WHERE peminjam = "Afdal" OR warna = "HITAM";
```
**Hasil:**
![[Screenshot 2023-10-26 102242.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
    
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
    
3. `WHERE peminjam = "Afdal" OR warna = "HITAM"`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana salah satu dari dua kondisi berikut ini harus terpenuhi:
    
    - Kolom "peminjam" memiliki nilai "Afdal."
    - Kolom "warna" memiliki nilai "HITAM."

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi setidaknya satu dari dua kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang entah dipinjam oleh "Afdal" atau berwarna "HITAM" dalam tabel "mobil."
## IN + AND + OPERATOR PEMBANDING (< dan >)
Kombinasi operator `IN`, `AND`, dan operator pembanding seperti `<` dan `>` dapat digunakan untuk membuat pernyataan SQL yang lebih kompleks dan spesifik untuk pemfilteran data dari tabel.

**Struktur Query:**
```sql
SELECT*FROM tabel
WHERE kolom1 IN (nilai1, nilai2, ...) AND kolom2 operator_pembanding nilai
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE warna IN ("HITAM","SILVER") AND harga_rental > 50000;
```
**Hasil:**
![[Screenshot 2023-10-26 102807 1.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE warna IN ("HITAM", "SILVER") AND harga_rental > 50000`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana dua kondisi berikut ini harus terpenuhi:
    - Kolom "warna" harus memiliki nilai "HITAM" atau "SILVER."
    - Kolom "harga_rental" harus memiliki nilai lebih besar dari 50000.

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi kedua kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang berwarna "HITAM" atau "SILVER" dan memiliki harga rental lebih dari 50000 dalam tabel "mobil."

# LIKE
## Awalan (Ib%)
Awalan `ib%` dalam SQL adalah pola pencarian yang menggunakan wildcard atau karakter joker `%` untuk mencari nilai di mana awalan (prefix) dari nilai tersebut adalah "ib". Wildcard `%` digunakan untuk mencocokkan sejumlah karakter apa pun yang mungkin mengikuti awalan "ib" dalam nilai yang dicari.

**Struktur Query:**
```sql
SELECT * FROM tabel WHERE nama LIKE 'ib%';
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE pemilik LIKE 'Ib%';
```
**Hasil:**
![[Screenshot 2023-10-26 103603.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE pemilik LIKE 'Ib%'`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana kolom "pemilik" dimulai dengan "Ib."

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang memiliki pemilik dengan nama yang dimulai dengan "Ib" dalam tabel "mobil."
## Akhiran (%m)
Akhiran `'%m'` dalam SQL adalah penggunaan karakter wildcard `%` untuk mencari data di mana nilai dalam suatu kolom berakhir dengan "m." Karakter wildcard `%` digunakan untuk menggantikan satu atau beberapa karakter sebelum karakter "m."

**Struktur Query:**
```sql
SELECT*FROM tabel
WHERE kolom_text LIKE '%m';
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE warna LIKE '%m';
```
**Hasil:**
![[Screenshot 2023-10-26 104134.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil." Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE warna LIKE '%m'`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana nilai dalam kolom "warna" berakhir dengan huruf "m."

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang berwarna dengan akhiran huruf "m."
## Awalan + Akhiran (b%m)
Gabungan awalan dan akhiran dalam SQL, seperti `b%m`, digunakan untuk mencari data yang memiliki pola tertentu pada kolom teks. Pencarian ini akan menghasilkan data yang memenuhi dua kondisi: yang dimulai dengan "b" dan berakhir dengan "m,"

**Struktur Query:**
```sql
SELECT*FROM tabel
WHERE kolom_teks LIKE 'b%' AND kolom_teks LIKE '%m';
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE pemilik LIKE 'b%' AND pemilik LIKE '%m';
```
**Hasil:**
![[Screenshot 2023-10-26 104628.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE pemilik LIKE 'b%' AND pemilik LIKE '%m'`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana kolom "pemilik" memenuhi dua kondisi berikut:
    - Kolom "pemilik" dimulai dengan "b" (awalan).
    - Kolom "pemilik" berakhir dengan "m" (akhiran).

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi kedua kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang dimiliki oleh pemilik yang namanya dimulai dengan "b" dan berakhir dengan "m" dalam tabel "mobil."
## Jumlah Karakter (i_+__ )

Untuk mencari data dalam SQL dengan jumlah karakter yang ditentukan dan pola karakter tertentu, kita dapat menggunakan karakter wildcard `_`, yang mewakili satu karakter tunggal, dan `LIKE`.

**Struktur Query:**
```sql
SELECT * FROM tabel
WHERE kolom_text LIKE '_SS';
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE pemilik LIKE '_b%';
```
**Hasil:**
![[Screenshot 2023-10-26 111153.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."

3. `WHERE pemilik LIKE '_b%'`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana kolom "pemilik" memenuhi tiga kondisi berikut:    
    - Karakter pertama dalam "pemilik" bisa menjadi karakter apa pun (diwakili oleh `_`).
    - Karakter kedua harus adalah "b."
    - Karakter selanjutnya (dilambangkan oleh `%`) bisa menjadi karakter apa pun lagi.

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi ketiga kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang pemiliknya memiliki nama yang dimulai dengan karakter apa pun (kecuali "b") dan diikuti oleh karakter "b" dalam tabel "mobil."
## Kombinasi ( _dan %)
`%` (Karakter Wildcard): tanda `%` digunakan sebagai karakter wildcard dalam SQL. Ini digunakan untuk mencocokkan nol atau lebih karakter.

**Struktur Query:**
```sql
SELECT*FROM tabel
WHERE kolom_teks LIKE 'dan%';
```
**Contoh Query:**
```sql
SELECT*FROM mobil
	 WHERE pemilik LIKE '__r%'
    ;
```
**Hasil:**
![[Screenshot 2023-10-26 111832.png]]

**Analisis Query:**
1. `SELECT *`: Ini adalah pernyataan yang digunakan untuk memilih semua kolom dari tabel "mobil". Artinya, hasil query akan mencakup semua kolom yang ada di tabel tersebut.
2. `FROM mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data. Dalam hal ini, tabel yang digunakan adalah "mobil."
3. `WHERE pemilik LIKE '__r%'`: Ini adalah perintah WHERE yang digunakan untuk memfilter data. Query akan mengambil baris-baris di mana kolom "pemilik" memenuhi tiga kondisi berikut:
    - Dua karakter pertama dalam "pemilik" dapat menjadi karakter apa pun (diwakili oleh `__`).
    - Karakter ketiga harus adalah "r."
    - Karakter selanjutnya (dilambangkan oleh `%`) bisa menjadi karakter apa pun lagi.

**Kesimpulan:**
Hasil dari query ini akan berisi semua kolom dari baris-baris yang memenuhi ketiga kondisi tersebut. Jadi, hasilnya akan menjadi daftar semua mobil yang pemiliknya memiliki nama yang memiliki dua karakter pertama yang dapat berupa karakter apa pun, diikuti oleh "r," dan kemudian diikuti oleh karakter apa pun lagi dalam tabel "mobil."


## Not Like
perintah "NOT LIKE" digunakan untuk mencari data yang tidak cocok dengan suatu pola dalam kolom teks. Pola ini ditentukan menggunakan ekspresi berbasis teks atau karakter tertentu. Misalnya, kita dapat menggunakan "NOT LIKE" untuk mencari data yang tidak mengandung kata tertentu, karakter tertentu, atau pola tertentu.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE kolom_teks NOT LIKE 'pola'
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE peminjam NOT LIKE 'A%';
    ```
**Hasil:**
![[Pasted image 20231026143403.png]]

**Analisis Query:**

1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil semua kolom (ditandai dengan tanda "*") dari tabel "mobil". Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
    
2. `WHERE peminjam NOT LIKE 'A%'`: Ini adalah perintah "WHERE" yang digunakan untuk memfilter data. perintah ini menentukan bahwa hanya data yang tidak memenuhi syarat tertentu yang akan diambil. Dalam hal ini, kita mencari data di mana kolom "peminjam" tidak dimulai dengan huruf 'A'. Jadi, ini akan mengambil semua data di mana nilai kolom "peminjam" tidak diawali dengan 'A'.

**Kesimpulan:**
adi, hasil query ini akan menampilkan semua catatan dari tabel "mobil" di mana peminjamnya bukanlah orang-orang yang nama mereka dimulai dengan huruf 'A'.
# MENCARI DATA NULL/NOT NULL
## NULL
perintah "IS NULL" digunakan untuk mencari data di mana kolom memiliki nilai NULL. Data dengan nilai NULL adalah data yang tidak memiliki nilai atau nilai yang tidak terdefinisi dalam kolom tersebut.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE nama_kolom IS NULL;

```
**Contoh Query:**
```sql
SELECT*FROM mobil
    WHERE peminjam IS NULL;
```
**Hasil:**
![[Pasted image 20231026143051.png]]

**Analisis Query:**
1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil seluruh kolom (ditandai dengan tanda "*") dari tabel "mobil". Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
2. `WHERE peminjam IS NULL`: Ini adalah perintah "WHERE" yang digunakan untuk memfilter data. perintah ini menentukan bahwa hanya data di mana kolom "peminjam" memiliki nilai NULL yang akan diambil. Ini berarti kita mencari mobil yang saat ini tidak dipinjam oleh siapa pun, atau di mana informasi peminjamnya tidak ada atau belum diisi.

**Kesimpulan:**
Query ini bermanfaat untuk menemukan mobil yang tersedia atau belum dipinjam, berdasarkan nilai NULL dalam kolom "peminjam".
## NOT NULL
perintah "NOT NULL" digunakan untuk memeriksa dan mengambil data dari kolom yang tidak mengizinkan nilai NULL. Ini digunakan untuk memastikan bahwa data yang kita ambil atau proses harus memiliki nilai yang valid dalam kolom tertentu.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
WHERE nama_kolom IS NOT NULL;
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    WHERE peminjam IS NOT NULL;
```
**Hasil:**
![[Pasted image 20231026143159.png]] 

**Analisis Query:**
1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil semua kolom (ditandai dengan tanda "*") dari tabel "mobil". Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
2. `WHERE peminjam IS NOT NULL`: Ini adalah perintah "WHERE" yang digunakan untuk memfilter data. perintah ini menentukan bahwa hanya data yang memenuhi syarat tertentu yang akan diambil. Dalam hal ini, kita mencari data di mana kolom "peminjam" tidak NULL. Artinya, kita hanya akan mengambil baris-baris di mana ada entri valid (tidak kosong) dalam kolom "peminjam."

**Kesimpulan:**
Hasil dari query ini akan berisi semua catatan dari tabel "mobil" di mana kolom "peminjam" tidak NULL, yang berarti hanya kolom yang memiliki nama peminjam yang valid akan ditampilkan dalam hasil query.

# ORDER/PENGURUTAN
## ASC (Ascending)
"ASC" adalah singkatan dari "Ascending" yang digunakan untuk mengurutkan hasil query dalam urutan naik, artinya dari nilai terkecil ke nilai terbesar atau sesuai urutan yang diatur berdasarkan kolom tertentu.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
ORDER BY nama_kolom ASC;
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    ORDER BY pemilik ASC;
```
**Hasil:**
![[Pasted image 20231026144429.png]]

**Analisis Query:**
1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil semua kolom (ditandai dengan tanda "*") dari tabel "mobil." Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
2. `ORDER BY pemilik ASC`: Ini adalah perintah "ORDER BY" yang digunakan untuk mengurutkan data berdasarkan kolom "pemilik" dalam urutan naik (ascending order). Dengan kata lain, query ini akan menghasilkan daftar mobil dan akan mengurutkannya berdasarkan pemiliknya dalam urutan abjad naik (dari A ke Z).

**Kesimpulan:**
Hasil dari query ini akan menampilkan seluruh data dari tabel "mobil," tetapi data tersebut akan diurutkan berdasarkan kolom "pemilik" dalam urutan naik.
## DESC (Descending)
"DESC" digunakan untuk mengurutkan hasil query dalam urutan menurun. Ini sering digunakan ketika kita ingin melihat data dari yang terbesar ke yang terkecil, seperti mengurutkan data numerik dari yang paling tinggi hingga yang paling rendah atau mengurutkan data teks secara terbalik, mulai dari huruf Z ke huruf A.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
ORDER BY nama_kolom DESC;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
    ORDER BY peminjam DESC;
```
**Hasil:**
![[Pasted image 20231026144608.png]]

**Analisis Query:**
1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil semua kolom (ditandai dengan tanda "*") dari tabel "mobil". Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
2. `ORDER BY peminjam DESC`: Ini adalah perintah "ORDER BY" yang digunakan untuk mengurutkan hasil query. perintah ini menentukan bahwa data akan diurutkan berdasarkan kolom "peminjam" dalam urutan menurun ("DESC"). Dengan demikian, data akan diurutkan dari yang terbesar ke yang terkecil berdasarkan nilai dalam kolom "peminjam."

**Kesimpulan:**
Hasil dari query ini akan berisi seluruh data dari tabel "mobil," diurutkan dalam urutan menurun berdasarkan kolom "peminjam," sesuai dengan nilai dalam kolom tersebut.
# DISTINCT
## Distinct
Dalam SQL, kata kunci "DISTINCT" digunakan untuk mengambil nilai unik atau menghilangkan duplikasi dari hasil query. Ini berguna ketika kita ingin mendapatkan daftar nilai yang berbeda dalam satu atau beberapa kolom tertentu dari tabel kita.

**Struktur Query:**`
```sql
SELECT DISTINCT kolom1, kolom2, ...
FROM nama_tabel;
```
**Contoh Query:**

**Tabel Pemilik:**
![[Pasted image 20231026150029.png]]

**Penggunaan Distinct:**
```sql
 SELECT DISTINCT(pemilik)
    FROM mobil;
```
**Hasil:**
![[Pasted image 20231026150104.png]]

**Analisis Query:**
1. `SELECT DISTINCT(pemilik)`: Ini adalah pernyataan yang mengambil daftar nilai yang berbeda dalam kolom "pemilik" dari tabel "mobil." Penggunaan "DISTINCT" sebelum kolom "pemilik" menunjukkan bahwa kita ingin hanya nilai unik dari kolom ini. Dengan kata lain, query ini akan mengambil satu nilai pemilik jika ada beberapa baris dengan pemilik yang sama, sehingga kita tidak akan mendapatkan pemilik yang berulang.
2. `FROM mobil`: Ini adalah bagian dari query yang menunjukkan tabel dari mana kita ingin mengambil data, yaitu tabel "mobil."

**Kesimpulan:**
Hasil dari query ini akan berisi daftar nama pemilik mobil yang berbeda dalam tabel "mobil," sehingga kita akan mendapatkan informasi tentang semua pemilik mobil yang terdaftar dalam tabel tersebut, tanpa duplikasi.
## Distinct + Order By
"DISTINCT" dan "ORDER BY" adalah dua perintah yang berbeda dalam SQL, dan keduanya digunakan untuk tujuan yang berbeda. Namun, kita dapat menggabungkan keduanya dalam satu query untuk menampilkan daftar nilai unik dan mengurutkannya sesuai kebutuhan.

**Struktur Query:**
```sql
SELECT DISTINCT column1, column2, ...
FROM table_name
ORDER BY column_to_sort;
```
**Contoh Query:**
```sql
SELECT DISTINCT(harga_rental)
    FROM mobil
    ORDER BY harga_rental DESC;
```
**Hasil:**
![[Pasted image 20231026151048.png]]

**Analisis Query:**
1. `SELECT DISTINCT(harga_rental)`: Ini adalah pernyataan yang mengambil daftar nilai harga rental yang berbeda dari kolom "harga_rental" dalam tabel "mobil." Penggunaan "DISTINCT" sebelum kolom "harga_rental" menunjukkan bahwa kita hanya ingin nilai unik dari kolom ini. Jika ada beberapa baris dengan harga rental yang sama, query ini hanya akan mengambil satu dari nilai-nilai tersebut dan menghilangkan duplikasi.
2. `FROM mobil`: Ini adalah bagian dari query yang menunjukkan tabel "mobil" dari mana kita ingin mengambil data.
3. `ORDER BY harga_rental DESC`: Ini adalah perintah "ORDER BY" yang digunakan untuk mengurutkan hasil query. Dalam hal ini, kita mengurutkan hasil berdasarkan kolom "harga_rental" dalam urutan menurun ("DESC"). Dengan kata lain, harga rental akan diurutkan dari yang tertinggi ke yang terendah.

**Kesimpulan:**
Hasil dari query ini akan berisi daftar harga rental yang berbeda dari tabel "mobil," tanpa duplikasi, dan diurutkan dalam urutan menurun berdasarkan harga rental. kita akan mendapatkan daftar harga rental yang paling tinggi di bagian atas hasil query, diikuti oleh harga rental yang lebih rendah.
# ORDER (HAL 215)
## ASC (Ascending)
"ASC" adalah singkatan dari "Ascending" yang digunakan untuk mengurutkan hasil query dalam urutan naik, artinya dari nilai terkecil ke nilai terbesar atau sesuai urutan yang diatur berdasarkan kolom tertentu.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
ORDER BY nama_kolom ASC;
```
**Contoh Query:**
```sql
 SELECT*FROM mobil
    ORDER BY pemilik ASC;
```
**Hasil:**
![[Pasted image 20231026144429.png]]

**Analisis Query:**
1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil semua kolom (ditandai dengan tanda "*") dari tabel "mobil." Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
2. `ORDER BY pemilik ASC`: Ini adalah perintah "ORDER BY" yang digunakan untuk mengurutkan data berdasarkan kolom "pemilik" dalam urutan naik (ascending order). Dengan kata lain, query ini akan menghasilkan daftar mobil dan akan mengurutkannya berdasarkan pemiliknya dalam urutan abjad naik (dari A ke Z).

**Kesimpulan:**
Hasil dari query ini akan menampilkan seluruh data dari tabel "mobil," tetapi data tersebut akan diurutkan berdasarkan kolom "pemilik" dalam urutan naik.
## DESC (Descending)
"DESC" digunakan untuk mengurutkan hasil query dalam urutan menurun. Ini sering digunakan ketika kita ingin melihat data dari yang terbesar ke yang terkecil, seperti mengurutkan data numerik dari yang paling tinggi hingga yang paling rendah atau mengurutkan data teks secara terbalik, mulai dari huruf Z ke huruf A.

**Struktur Query:**
```sql
SELECT kolom1, kolom2, ...
FROM nama_tabel
ORDER BY nama_kolom DESC;
```
**Contoh Query:**
```sql
SELECT*FROM mobil
    ORDER BY peminjam DESC;
```
**Hasil:**
![[Pasted image 20231026144608.png]]

**Analisis Query:**
1. `SELECT * FROM mobil`: Ini adalah pernyataan untuk mengambil semua kolom (ditandai dengan tanda "*") dari tabel "mobil". Ini berarti kita akan mendapatkan seluruh data dari tabel ini.
2. `ORDER BY peminjam DESC`: Ini adalah perintah "ORDER BY" yang digunakan untuk mengurutkan hasil query. perintah ini menentukan bahwa data akan diurutkan berdasarkan kolom "peminjam" dalam urutan menurun ("DESC"). Dengan demikian, data akan diurutkan dari yang terbesar ke yang terkecil berdasarkan nilai dalam kolom "peminjam."

**Kesimpulan:**
Hasil dari query ini akan berisi seluruh data dari tabel "mobil," diurutkan dalam urutan menurun berdasarkan kolom "peminjam," sesuai dengan nilai dalam kolom tersebut.
# DISTINCT (HAL 203) 
## Distinct
Dalam SQL, kata kunci "DISTINCT" digunakan untuk mengambil nilai unik atau menghilangkan duplikasi dari hasil query. Ini berguna ketika kita ingin mendapatkan daftar nilai yang berbeda dalam satu atau beberapa kolom tertentu dari tabel kita.

**Struktur Query:**`
```sql
SELECT DISTINCT kolom1, kolom2, ...
FROM nama_tabel;
```
**Contoh Query:**

**Tabel Pemilik:**
![[Pasted image 20231026150029.png]]

**Penggunaan Distinct:**
```sql
 SELECT DISTINCT(pemilik)
    FROM mobil;
```
**Hasil:**
![[Pasted image 20231026150104.png]]

**Analisis Query:**
1. `SELECT DISTINCT(pemilik)`: Ini adalah pernyataan yang mengambil daftar nilai yang berbeda dalam kolom "pemilik" dari tabel "mobil." Penggunaan "DISTINCT" sebelum kolom "pemilik" menunjukkan bahwa kita ingin hanya nilai unik dari kolom ini. Dengan kata lain, query ini akan mengambil satu nilai pemilik jika ada beberapa baris dengan pemilik yang sama, sehingga kita tidak akan mendapatkan pemilik yang berulang.
2. `FROM mobil`: Ini adalah bagian dari query yang menunjukkan tabel dari mana kita ingin mengambil data, yaitu tabel "mobil."

**Kesimpulan:**
Hasil dari query ini akan berisi daftar nama pemilik mobil yang berbeda dalam tabel "mobil," sehingga kita akan mendapatkan informasi tentang semua pemilik mobil yang terdaftar dalam tabel tersebut, tanpa duplikasi.
## Distinct + Order By
"DISTINCT" dan "ORDER BY" adalah dua perintah yang berbeda dalam SQL, dan keduanya digunakan untuk tujuan yang berbeda. Namun, kita dapat menggabungkan keduanya dalam satu query untuk menampilkan daftar nilai unik dan mengurutkannya sesuai kebutuhan.
**Struktur Query:**

```sql
SELECT DISTINCT column1, column2, ...
FROM table_name
ORDER BY column_to_sort;
```

**Contoh Query:**
```sql
SELECT DISTINCT(harga_rental)
    FROM mobil
    ORDER BY harga_rental DESC;
```
**Hasil:**
![[Pasted image 20231026151048.png]]

**Analisis Query:**
1. `SELECT DISTINCT(harga_rental)`: Ini adalah pernyataan yang mengambil daftar nilai harga rental yang berbeda dari kolom "harga_rental" dalam tabel "mobil." Penggunaan "DISTINCT" sebelum kolom "harga_rental" menunjukkan bahwa kita hanya ingin nilai unik dari kolom ini. Jika ada beberapa baris dengan harga rental yang sama, query ini hanya akan mengambil satu dari nilai-nilai tersebut dan menghilangkan duplikasi.
2. `FROM mobil`: Ini adalah bagian dari query yang menunjukkan tabel "mobil" dari mana kita ingin mengambil data.
3. `ORDER BY harga_rental DESC`: Ini adalah perintah "ORDER BY" yang digunakan untuk mengurutkan hasil query. Dalam hal ini, kita mengurutkan hasil berdasarkan kolom "harga_rental" dalam urutan menurun ("DESC"). Dengan kata lain, harga rental akan diurutkan dari yang tertinggi ke yang terendah.

**Kesimpulan:**
Hasil dari query ini akan berisi daftar harga rental yang berbeda dari tabel "mobil," tanpa duplikasi, dan diurutkan dalam urutan menurun berdasarkan harga rental. kita akan mendapatkan daftar harga rental yang paling tinggi di bagian atas hasil query, diikuti oleh harga rental yang lebih rendah.
# CONCAT (HAL 204) 
## CONCAT
Concatenation (concat) adalah proses penggabungan dua atau lebih string menjadi satu string tunggal dalam SQL. Dalam SQL, Anda dapat menggunakan berbagai fungsi atau operator untuk menggabungkan (concatenate) nilai-nilai string.

**Struktur Query:**
```sql
SELECT CONCAT(kolom-1,"Penghubung",kolom-2)
	FROM nama_tabel;
```
**Contoh Query:**
```sql
 SELECT CONCAT(pemilik,"_",warna)
    FROM mobil;
```
**Hasil:**
![[Pasted image 20231026152012.png]]

**Analisis Query:**
1. `SELECT`: Ini adalah pernyataan yang digunakan untuk mengambil data dari tabel. Dalam query ini, kita memilih data yang akan dihasilkan dalam hasil query.
2. `CONCAT(pemilik,"_",warna)`: Ini adalah fungsi yang digunakan untuk menggabungkan atau menggabungkan nilai dari kolom `pemilik` dan `warna`. Fungsi `CONCAT()` akan mengambil nilai dari kolom `pemilik`, menambahkan tanda underscore (`"_"`), dan kemudian menambahkan nilai dari kolom `warna`. Hasilnya adalah satu string yang berisi kedua nilai tersebut dengan underscore sebagai pemisah.
3. `FROM mobil`: Ini menentukan tabel yang digunakan dalam query. Dalam hal ini, kita mengambil data dari tabel yang disebut `mobil`.

**Kesimpulan:**
Hasil dari query ini akan menghasilkan satu kolom baru yang berisi hasil konkatenasi dari kolom `pemilik` dan `warna`, dengan underscore di antara keduanya, untuk setiap baris dalam tabel `mobil`.

## CONCAT_WS
Perintah `CONCAT_WS` (Concatenate With Separator) adalah perintah yang digunakan dalam SQL untuk menggabungkan beberapa nilai string dengan pemisah yang ditentukan.

**Struktur Query:**
```sql
CONCAT_WS(penghubung, string1, string2, ..., stringN)
	FROM nama_table;
```
**Contoh Query**
```sql
 SELECT CONCAT_WS(" - ", no_plat, no_mesin, "id_mobil")
    FROM mobil;
```
**Hasil:**
![[Pasted image 20231026153409.png]]

**Analisis Query:**
- `CONCAT_WS`: Ini adalah fungsi SQL yang digunakan untuk menggabungkan sejumlah nilai dengan separator tertentu. Fungsi ini mengambil dua argumen: separator (dalam hal ini, " - ") dan daftar nilai atau kolom yang ingin digabungkan.
- `" - "`: Ini adalah separator yang akan digunakan untuk menggabungkan nilai-nilai dalam daftar. Dalam contoh ini, " - " adalah tanda hubung dengan spasi di antara tanda "-" yang akan memisahkan nilai-nilai yang digabungkan.
- `no_plat`, `no_mesin`, `"id_mobil"`: Ini adalah kolom atau nilai yang akan digabungkan. Dalam query ini, `no_plat` dan `no_mesin` adalah kolom yang diambil dari tabel `mobil`, dan "id_mobil" adalah string konstan.

**Kesimpulannya:**
Hasil dari query ini adalah satu kolom yang berisi hasil penggabungan kolom `no_plat`, `no_mesin`, dan string konstan "id_mobil" dengan tanda hubung (separator) " - " di antara mereka.
# AS
## AS
Perintah `AS` dalam SQL digunakan untuk memberi alias (nama lain) pada kolom atau tabel dalam hasil query. Alias digunakan untuk memberi nama atau label yang lebih deskriptif atau singkat pada hasil query.

**Struktur Query:**
```sql
SELECT column_name AS alias_name
FROM table_name;

```
**Contoh Query:**
```sql
 SELECT harga_rental, harga_rental*0.1
    AS diskon FROM mobil;
```
**Hasil:**
![[Pasted image 20231026154221.png]]

**Analisis Query:**
- `SELECT harga_rental`: Ini bagian pertama dari pernyataan SELECT yang mengambil nilai dari kolom `harga_rental` dari tabel `mobil`.
- `harga_rental * 0.1`: Ini adalah perhitungan yang dilakukan dalam query. Perhitungan ini mengambil nilai dari kolom `harga_rental` dan mengalikannya dengan 0.1, yang setara dengan menghitung 10% dari harga rental.
- `AS diskon`: Ini adalah bagian yang memberi alias pada hasil perhitungan. Hasil perhitungan, yaitu 10% dari harga rental, diberi alias "diskon". Dengan kata lain, kolom hasil perhitungan akan memiliki nama "diskon" dalam hasil query.

**Kesimpulan:**
Dengan hasil ini, kita memiliki harga rental asli dalam kolom `harga_rental` dan juga diskon sebesar 10% dari harga rental dalam kolom `diskon`.
## AS + CONCAT_WS
Dalam SQL, kita dapat menggunakan `AS` untuk memberikan alias pada kolom atau tabel, dan kita juga dapat menggunakan `CONCAT_WS` untuk menggabungkan nilai-nilai dengan separator tertentu.

**Struktur Query:**
```sql
SELECT CONCAT_WS(" - ", column1, column2) AS alias_name
FROM table_name;
```
**Contoh Query:**
```sql
SELECT CONCAT_WS(" + ", pemilik,peminjam) AS COLLAB
    FROM mobil;
```
**Hasil:**
![[Pasted image 20231026154323.png]]

**Analisis Query:**
- `CONCAT_WS(" + ", pemilik, peminjam)`: Ini adalah bagian dari query yang melakukan penggabungan (concatenation) dari nilai kolom `pemilik` dan `peminjam` dengan tanda "+" sebagai separator. `CONCAT_WS` digunakan di sini untuk menggabungkan kedua nilai dengan separator yang ditentukan.
- `AS COLLAB`: Ini adalah bagian yang memberikan alias pada kolom hasil perhitungan. Hasil dari penggabungan tersebut diberi nama alias "COLLAB".

**Kesimpulan:**
Kolom "COLLAB": Berisi hasil penggabungan antara nilai dari kolom `pemilik` dan
`peminjam` dalam tabel `mobil`, dengan tanda "+" sebagai pemisah.



# ALTER
## Menambahkan Kolom
Perintah SQL "ALTER TABLE" digunakan untuk mengubah struktur tabel, dan "ADD COLUMN" digunakan untuk menambahkan kolom baru ke tabel. Ini adalah cara umum untuk menambahkan kolom ke tabel yang sudah ada.

**Struktur Query:**

```sql
ALTER TABLE mobil
		field tipe_data(jumlah_karakter) constrain;
```
**Contoh Query:**

Sebelum:
![[Pasted image 20231102135044.png]]

```sql
ALTER TABLE mobil
	 ADD batas_waktu_pinjam varchar(10);
```
**Hasil**
![[Pasted image 20231102135525.png]]

**Analisis Query:**
1. `ALTER TABLE mobil`: Ini adalah bagian yang menyatakan bahwa kita ingin mengubah struktur tabel "mobil".
2. `ADD batas_waktu_pinjam VARCHAR(10)`: Bagian ini adalah instruksi untuk menambahkan kolom baru ke tabel "mobil". Kolom baru tersebut diberi nama "batas_waktu_pinjam" dan memiliki tipe data VARCHAR dengan panjang maksimum 10 karakter.

**Kesimpulan**
	Dengan demikian, setelah menjalankan perintah ini, Kita akan memiliki kolom "batas_waktu_pinjam" yang memungkinkan Kita untuk menyimpan informasi terkait batas waktu peminjaman mobil dalam bentuk string dengan panjang maksimum 10 karakter. Ini memungkinkan Kita untuk mengatur dan melacak informasi seperti tanggal atau waktu terkait dengan peminjaman mobil.
## Mengubah Kolom & Tipe Data

### Menggunakan Change
Perintah "ALTER TABLE CHANGE" (walaupun tidak umum) bisa dimaksudkan untuk mengubah struktur tabel dengan mengganti atau memodifikasi kolom yang ada dengan nama kolom baru, tipe data baru, atau atribut kolom lainnya.

**Struktur Query:**
```sql
ALTER TABLE nama_tabel
CHANGE nama_kolom_lama nama_kolom_baru tipe_data [atribut_kolom];
```
**Contoh Query:**
```sql
 ALTER TABLE mobil
     CHANGE batas_waktu_pinjam deadline DATE;
```
**Hasil:**
![[Pasted image 20231102143045.png]]

**Penampilan Select*From:**
![[Pasted image 20231102143117.png]]

**Analisis Query:**
1. **ALTER TABLE mobil**: Perintah ini mengindikasikan bahwa Anda ingin mengubah struktur tabel "mobil".
    
2. **CHANGE batas_waktu_pinjam deadline DATE**: Bagian ini menentukan perubahan yang akan dilakukan.
    
    - "CHANGE" digunakan untuk mengganti nama kolom.
    - "batas_waktu_pinjam" adalah nama kolom yang akan diganti.
    - "deadline" adalah nama baru yang akan diberikan kepada kolom tersebut.
	- "DATE" adalah tipe data baru yang akan diterapkan pada kolom "deadline," yang merupakan tipe data tanggal.

**Kesimpulan:**
Dengan perubahan ini, tabel "mobil" sekarang memiliki kolom "deadline" yang akan digunakan untuk menyimpan informasi terkait tanggal batas waktu peminjaman mobil.
### Tipe Data
Perintah SQL "ALTER TABLE MODIFY COLUMN" (yang sesuai) digunakan untuk mengubah definisi atau struktur kolom yang ada dalam tabel.

**Struktur Query:**
```sql
ALTER TABLE nama_tabel
MODIFY COLUMN nama_kolom tipe_data [atribut_kolom];
```
**Contoh Query:**
```sql
 ALTER TABLE mobil
    MODIFY COLUMN deadline varchar(10);
```
**Hasil:**
![[Pasted image 20231102144310.png]]

**Analisis query:**
- `nama_tabel`: Nama tabel yang ingin Anda ubah strukturnya.
- `MODIFY COLUMN`: Ini adalah bagian yang menunjukkan bahwa Anda ingin memodifikasi kolom.
- `nama_kolom`: Nama kolom yang akan dimodifikasi.
- `tipe_data`: Tipe data baru yang ingin Anda berikan pada kolom.
- `atribut_kolom` (opsional): Atribut tambahan seperti NOT NULL, DEFAULT, dll., yang dapat diterapkan pada kolom.

**Kesimpulan:**
perintah ini digunakan untuk mengubah tipe data kolom "deadline" dalam tabel "mobil" sehingga kolom tersebut dapat digunakan untuk menyimpan teks atau karakter dengan panjang maksimum 10 karakter.
### Menambah/mengubah Constraint

Perintah untuk mengatur nilai default kolom dalam sebuah tabel digunakan untuk menentukan nilai default yang akan digunakan jika tidak ada nilai yang diberikan saat memasukkan data ke kolom tersebut. Ini adalah salah satu cara untuk mengatur standar nilai di dalam tabel.

**Struktur Query:**
```sql
ALTER TABLE nama_tabel
ALTER nama_kolom SET constraint;
```
**Contoh Query**:
```sql
ALTER TABLE mobil
    ALTER deadline SET DEFAULT 'Ready';
```
**Hasil:**
![[Pasted image 20231102145257.png]]

**Analisis Query:**
1. `ALTER TABLE mobil`: Ini adalah perintah yang digunakan untuk mengubah struktur tabel "mobil."
2. `ALTER deadline`: Ini adalah bagian yang menunjukkan bahwa Anda ingin mengubah kolom "deadline."
3. `SET DEFAULT 'Ready'`: Ini adalah bagian yang digunakan untuk mengatur nilai default kolom "deadline" menjadi 'Ready'. Ini berarti jika tidak ada nilai yang diberikan saat memasukkan data ke kolom "deadline," maka nilainya akan secara otomatis diatur menjadi 'Ready'.

**Pengujian:**
```sql
INSERT INTO mobil
    -> (id_mobil, no_plat, no_mesin, warna, pemilik, harga_rental)
    -> VALUES (6, "DD 1223 JK", "RPL2023", "HITAM", "Valen", 250000);
```
**Hasil Pengujian:**
![[Pasted image 20231102150507.png]]

**Kesimpulan:**
Dengan menjalankan perintah ini, Anda mengubah kolom "deadline" dalam tabel "mobil" sehingga jika tidak ada nilai yang diberikan saat memasukkan data ke kolom tersebut, maka kolom akan memiliki nilai default 'Ready'.
## Menghapus Constrain
Perintah "ALTER TABLE ALTER DROP" digunakan untuk menghapus kolom atau constraint yang ada dalam sebuah tabel. Ini memungkinkan Anda untuk mengubah struktur tabel dengan menghapus elemen tertentu.

**Struktur Query:**
```sql
ALTER TABLE nama_tabel
ALTER nama_kolom DROP constraint;
```
**Contoh Query:**
```sql
ALTER TABLE mobil
    ALTER deadline DROP DEFAULT;
```
**Hasil:**
*Sebelum:*
![[Pasted image 20231102151723.png]]

*Sesudah:*
![[Pasted image 20231102151741.png]]

**Analisis Query:**
1. `ALTER TABLE mobil`: Ini adalah perintah yang digunakan untuk mengubah struktur tabel "mobil."
2. `ALTER deadline`: Ini adalah bagian yang menunjukkan bahwa Anda ingin mengubah kolom "deadline."
3. `DROP DEFAULT`: Ini adalah bagian yang digunakan untuk menghapus nilai default dari kolom "deadline."

**Kesimpulan:**
Dengan menjalankan perintah ini, Anda mengubah kolom "deadline" dalam tabel "mobil" sehingga nilai default yang mungkin sebelumnya diterapkan pada kolom "deadline" akan dihapus.
## Menghapus Kolom
Perintah "ALTER TABLE DROP COLUMN" digunakan untuk menghapus satu atau beberapa kolom dari sebuah tabel. Hal ini memungkinkan Anda untuk mengurangi kompleksitas tabel dan menghilangkan kolom yang tidak lagi diperlukan.

**Struktur Query:**
```sql
ALTER TABLE nama_tabel
DROP COLUMN nama_kolom1, nama_kolom2, ...;
```
**Contoh Query:**

**Tabel Sebelumnya:**
![[Pasted image 20231102153531.png]]
```sql
 ALTER TABLE mobil
 DROP COLUMN deadline;
```
**Hasil:**
![[Pasted image 20231102153509.png]]

**Analisis Query:**
1. `ALTER TABLE mobil`: Ini adalah perintah yang digunakan untuk mengubah struktur tabel "mobil."
2. `DROP COLUMN deadline`: Ini adalah bagian yang menunjukkan bahwa Anda ingin menghapus kolom "deadline" dari tabel "mobil."

**Kesimpulan**
Dengan menjalankan perintah ini, Anda akan mengubah struktur tabel "mobil" dengan menghapus kolom "deadline" dari tabel tersebut. Ini akan mengakibatkan kolom "deadline" tidak lagi ada dalam tabel "mobil."
# VIEW
## Create
View adalah tampilan table yang terdiri dari hasil query SELECT. View tidak menyimpan data secara fisik; sebaliknya, mereka hanya menampilkan query yang diselect. Ini memungkinkan kita untuk menyederhanakan tampilan data query, menyembunyikan detail tabel, dan memberikan akses terbatas ke data.

**Struktur Quey:**
```sql
CREATE VIEW nama_view AS
SELECT kolom1, kolom2
FROM nama_tabel
WHERE kondisi;
```
**Contoh Query:**
```sql
CREATE VIEW info_pemilik AS
SELECT id_mobil, pemilik, no_plat
FROM mobil
WHERE pemilik = "Ibhe";
```
**Hasil:**
![[Pasted image 20231109135212.png]]

**Analisis Query:**
1. **CREATE VIEW info_pemilik:** Bagian ini mengindikasikan bahwa kita sedang membuat sebuah view dengan nama `info_pemilik`.
2. **AS:** Ini digunakan untuk memberikan nama pada view yang akan dibuat.
3. **SELECT id_mobil, pemilik, no_plat:** Dalam view ini, kita memilih kolom `id_mobil`, `pemilik`, dan `no_plat` dari tabel `mobil`.
4. **FROM mobil:** Menunjukkan bahwa kita mengambil data dari tabel `mobil`.
5. **WHERE pemilik = "Ibhe";** Hanya data yang memenuhi kondisi `pemilik = "Ibhe"` yang akan dimasukkan ke dalam view. Artinya, view `info_pemilik` hanya akan berisi data mobil yang dimiliki oleh "Ibhe".

**Kesimpulan:**
Jadi, secara keseluruhan, query ini membuat sebuah view bernama `info_pemilik` yang berisi informasi tentang mobil (id_mobil, pemilik, no_plat) yang dimiliki oleh "Ibhe" dari tabel `mobil`.
## Select
Perintah `SELECT` pada view dalam SQL digunakan untuk menampilkan data dari view yang telah kita buat sebelumnya.

**Struktur Query:**
```sql
SELECT*FROM nama_view;
```
**Contoh Query:**
```sql
SELECT*FROM info_pemilik
```
**Hasil:**
![[Pasted image 20231109135351.png]]

**Analisis query:**
1. **SELECT:** Ini adalah perintah yang digunakan untuk memilih data dari tabel atau view.
2. `*`:Merepresentasikan semua kolom yang ada dalam view. Dengan menggunakan bintang, kita memilih untuk menampilkan semua kolom yang telah didefinisikan dalam view `info_pemilik`.
3. **FROM info_pemilik:** Menunjukkan bahwa kita ingin mengambil data dari view dengan nama `info_pemilik`.

**Kesimpulan:**
Jadi, secara keseluruhan, perintah `SELECT * FROM info_pemilik;` ini akan mengembalikan semua baris dan kolom yang telah didefinisikan dalam view `info_pemilik`.
## Drop
Perintah `DROP` pada SQL digunakan untuk menghapus objek database tertentu, termasuk view.

**Struktur Query:**
```sql
DROP VIEW nama_view;
```
**Contoh Query:**
```sql
DROP VIEW info_pemilik
```
**Hasil:**
![[Pasted image 20231109135514.png]]

**Analisis Query:**
1. **DROP VIEW:** Perintah ini menunjukkan niat untuk menghapus sebuah view dari database.
2. **info_pemilik:** Nama view yang akan dihapus.

**Kesimpulan:**
Jadi, secara keseluruhan, query ini berarti "Hapus view dengan nama `info_pemilik` dari database."
# AGREGASI
## Sum
Perintah SUM digunakan untuk menghitung total dari nilai-nilai numerik dalam suatu kolom. Ini sering digunakan bersama dengan pernyataan SELECT untuk mengambil hasil agregasi dari data dalam tabel.

**Struktur Query:**
```sql
SELECT SUM(nama_kolom) AS total
FROM nama_tabel
WHERE kondisi_opsional;
```
**Contoh Query:**
```sql
SELECT SUM(harga_rental) FROM mobil;
```
**Hasil:**
![[Pasted image 20231109153701.png]]

**Analisis query:**
1. **SUM(harga_rental):** Ini adalah fungsi agregasi SUM yang digunakan untuk menjumlahkan semua nilai dalam kolom harga_rental.
    
2. **FROM mobil:** Menunjukkan bahwa data diambil dari tabel dengan nama "mobil". Jadi, pernyataan ini menghitung total harga_rental dari semua baris dalam tabel "mobil".

**Kesimpulan:**
Hasil dari query ini akan menjadi total dari semua nilai dalam kolom "harga_rental" dalam tabel "mobil". Misalnya, jika tabel "mobil" memiliki beberapa baris dengan harga_rental yang berbeda, hasilnya akan menjadi jumlah dari semua nilai tersebut.
## Count
Perintah COUNT digunakan untuk menghitung jumlah baris yang memenuhi suatu kondisi atau untuk menghitung jumlah baris dalam suatu tabel. 

**Struktur Query:**
```sql
SELECT COUNT(*) AS jumlah
FROM nama_tabel
WHERE kondisi_opsional;
```
**Contoh Query:**
count pemilik:
```sql
 SELECT COUNT(pemilik) FROM mobil;
```
Hasil:
![[Pasted image 20231109154144.png]]
count peminjam:
```sql
 SELECT COUNT(peminjam) FROM mobil;
```
Hasil:
![[Pasted image 20231109154033.png]]
**Analisis Query:**
1. **COUNT(pemilik):** Ini adalah fungsi COUNT yang digunakan untuk menghitung jumlah baris di mana nilai kolom "pemilik" tidak NULL. COUNT menghitung jumlah nilai non-NULL dalam kolom yang ditentukan.
2. **FROM mobil:** Menunjukkan bahwa data diambil dari tabel dengan nama "mobil". Jadi, pernyataan ini menghitung jumlah baris di mana kolom "pemilik" tidak NULL dalam tabel "mobil".

**Perbedaan dengan SUM**
Count bertujuan untuk Menghitung jumlah baris dalam suatu tabel atau jumlah baris yang memenuhi suatu kondisi tertentu. Sedangkan sum bertujuan untuk menghitung **total** nilai dari suatu kolom numerik dalam suatu tabel atau total nilai yang memenuhi suatu kondisi tertentu.

**Kesimpulan:**
Hasil dari query ini akan menjadi jumlah baris di mana nilai kolom "pemilik"  yang tidak NULL dalam tabel "mobil"
## Min
Fungsi MIN digunakan untuk menemukan nilai minimum dalam suatu kolom. Fungsi ini berguna ketika kita ingin mengetahui nilai terkecil dalam satu set data. 
**Struktur Query:**
```sql
SELECT MIN(nama_kolom) AS nilai_minimum
FROM nama_tabel
WHERE kondisi_opsional;
```
**Contoh Query:**
```sql
SELECT MIN(harga_rental) AS MINIMAL FROM mobil;
```
**Hasil:**
![[Pasted image 20231109154350.png]]

**Analisis Query:**
1. **MIN(harga_rental):** Ini adalah fungsi MIN yang digunakan untuk menemukan nilai minimum dari kolom "harga_rental". Fungsi ini akan mengambil nilai terkecil dari semua nilai yang ada dalam kolom "harga_rental".
2. **AS MINIMAL:** Memberikan nama pada kolom hasil perhitungan. Dalam hal ini, hasil perhitungan diberi nama "MINIMAL", yang dapat digunakan untuk merujuk pada nilai minimum dalam hasil query.
3. **FROM mobil:** Menunjukkan bahwa data diambil dari tabel dengan nama "mobil". Jadi, pernyataan ini menemukan nilai minimum dari kolom "harga_rental" dalam tabel "mobil".

**Kesimpulan:**
Hasil dari query ini akan menjadi nilai minimum dari semua nilai dalam kolom "harga_rental" dalam tabel "mobil".
## Max
Fungsi MAX digunakan untuk menemukan nilai maksimum dari suatu kolom. Fungsi ini berguna ketika kita ingin mengetahui nilai terbesar dalam satu set data.

**Struktur Query:**
```sql
SELECT MAX(nama_kolom) AS nilai_maksimum
FROM nama_tabel
WHERE kondisi_opsional;
```
**Contoh Query:**
```SQL
 SELECT MAX(harga_rental) AS MAXIMAL
 FROM mobil
```
**Hasil:**
![[Pasted image 20231109154543.png]]

**Analisis Query:**
1. **MAX(harga_rental):** Ini adalah fungsi MAX yang digunakan untuk menemukan nilai maksimum dari kolom "harga_rental". Fungsi ini akan mengambil nilai terbesar dari semua nilai yang ada dalam kolom "harga_rental".
2. **AS MAXIMAL:** Memberikan nama pada kolom hasil perhitungan. Dalam hal ini, hasil perhitungan diberi nama "MAXIMAL", yang dapat digunakan untuk merujuk pada nilai maksimum dalam hasil query.
3. **FROM mobil:** Menunjukkan bahwa data diambil dari tabel dengan nama "mobil". Jadi, pernyataan ini menemukan nilai maksimum dari kolom "harga_rental" dalam tabel "mobil".

**Kesimpulan:**
Hasil dari query ini akan menjadi nilai maksimum dari semua nilai dalam kolom "harga_rental" dalam tabel "mobil".
## AVG
fungsi agregasi yang digunakan untuk menghitung nilai rata-rata dari suatu kolom yang berisi data numerik. Fungsi AVG sangat berguna ketika kita ingin mengetahui nilai rata-rata dari suatu set data. Berikut adalah penjelasan mengenai AVG beserta strukturnya:

**Struktur Query:**
```sql
SELECT AVG(nama_kolom) AS rata_rata
FROM nama_tabel
WHERE kondisi_opsional;

```
**Contoh Query:**
```SQL
 SELECT AVG(harga_rental) AS RATA_RATA FROM mobil;
```
**Hasil:**
![[Pasted image 20231109154845.png]]

**Analisis Query:**
1. **AVG(harga_rental):** Ini adalah fungsi AVG yang digunakan untuk menghitung nilai rata-rata dari kolom "harga_rental". Fungsi ini akan mengambil nilai rata-rata dari semua nilai yang ada dalam kolom "harga_rental".
2. **AS RATA_RATA:** Memberikan nama pada kolom hasil perhitungan. Dalam hal ini, hasil perhitungan diberi nama "RATA_RATA", yang dapat digunakan untuk merujuk pada nilai rata-rata dalam hasil query.
3. **FROM mobil:** Menunjukkan bahwa data diambil dari tabel dengan nama "mobil". Jadi, pernyataan ini menghitung nilai rata-rata dari kolom "harga_rental" dalam tabel "mobil".

**Kesimpulan**
Hasil dari query ini akan menjadi nilai rata-rata dari semua nilai dalam kolom "harga_rental" dalam tabel "mobil".