# AND
## Struktur Query
```mysql
select kolom1,kolom2 from nama_tabel, where kolom1="nilai1" AND kolom2="nilai2;
```
## Contoh Query
```mysql
select warna,pemilik from mobil where warna='HITAM' AND pemilik='RANI';
```
## Hasil
![image](ASET/s1.png)
## Analisis
1. `SELECT warna, pemilik`: Ini menentukan bahwa kita ingin memilih kolom warna dan pemilik dari tabel mobil.
2. `FROM mobil`: Ini menentukan tabel yang kolomnya ingin kita pilih, yaitu tabel mobil.
3. `WHERE warna='HITAM' AND pemilik='RANI'`: Ini menentukan kondisi yang harus dipenuhi suatu baris agar dapat dipilih. Dalam hal ini kolom warna harus 'HITAM' dan kolom pemilik harus 'RANI'. Kata kunci AND menetapkan bahwa kedua kondisi harus benar agar suatu baris dapat dipilih.

## Kesimpulan
Query di atas mempermudah kita dalam mencari data yang akurat tanpa harus mengecek semua..

# OR
## Struktur Query
```mysql
select kolom1,kolom2 from nama_tabel, where kolom1="nilai1" AND kolom2="nilai2;
```
## Contoh Query
 ```mysql
select warna,pemilik from mobil where warna='HITAM' AND pemilik='RANI';
```
## Hasil
![image](aset/s2.png)

## Analisis 
1. `SELECT warna, pemilik`: Bagian query ini menentukan kolom yang ingin saya ambil dari tabel mobil. Dalam hal ini, Anda ingin mengambil kolom warna (warna) dan pemilik (pemilik).
2. `FROM mobil`: Bagian query ini menentukan tabel tempat saya ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.
3. `WHERE warna='HITAM' AND pemilik='RANI`': Bagian query ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, saya ingin mengambil data dimana warna (warna) adalah 'HITAM' (hitam) dan pemilik (pemilik) adalah 'RANI'.
## Kesimpulan 
perintah tersebut digunakan untuk mencari mobil dengan warna `'HITAM'` yang dimiliki oleh `'RANI'` dari tabel `"mobil`".

# BETWEEN - AND
## Struktur Query
```mysql
select * from nama_tabel where kolom1 between nilai1 AND nilai2;
```

## Contoh Query
```mysql
select * from mobil where harga_rental between 100000 AND 150000;
```

## Hasil
![image](aset/s3.png)

## Analisis
`SELECT *`: Bagian query ini menentukan bahwa Anda ingin mengambil semua kolom dari tabel seluler.

`FROM mobil`: Bagian query ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.

`WHERE harga_rental BETWEEN 100000 AND 150000`: Bagian query ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data yang `harga_rental` (harga sewa) antara `100.000` dan `150.000`.

## Kesimpulan
Perintah tersebut digunakan untuk mencari mobil dengan harga sewa antara 100.000 hingga 150.000.

# NOT BETWEEN
## Struktur Query
```mysql
select * from nama_tabel where kolom1 not between nilai1 AND nilai2;
```
## Contoh Query

```mysql
 select * from mobil where harga_rental not between 1000000 AND 20000;
```
## Hasil 
![image](aset/s4.png)
## Analisis
1. `SELECT *`: Bagian Query ini menentukan bahwa Anda ingin mengambil semua kolom dari tabel seluler.
2. `FROM mobil`: Bagian query ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.
3. `WHERE harga_rental not beetween 1000000 and 20000`: Bagian query ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data yang harga_rental (harga sewa) bukan antara 1.000.000 dan 20.000.
## Kesimpulan
Perintah tersebut digunakan untuk mencari mobil dengan harga sewa di luar rentang 20.000 hingga 1.000.000.

# <=
## Struktur Query
```mysql
 select * from nama_tabel where kolom1 <= nilai1;
```
## Contoh Query
```mysql
 select * from mobil where harga_rental <= 50000;
```

## Hasil
![image](aset/s5.png)

## Analisis
1. `SELECT *`: Bagian kueri ini menentukan bahwa Anda ingin mengambil semua kolom dari tabel seluler.
2. `FROM mobil`: Bagian kueri ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.
3. `WHERE harga_rental <= 50000`: Bagian kueri ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data dimana harga_rental (harga sewa) kurang dari atau sama dengan 50.000.
## Kesimpulan
Perintah tersebut digunakan untuk mencari mobil dengan harga sewa yang kurang dari atau sama dengan 50.000.
# >=
## Struktur Query
```mysql
select * from nama_tabel where kolom1 <= nilai1;
```
## Contoh Query
```mysql
 select * from mobil where harga_rental >= 50000;
 ```

## Hasil
![[s6.png]]
## Analisis
1.  `SELECT *`: Bagian kueri ini menentukan bahwa Anda ingin mengambil semua kolom dari tabel seluler.
2. `FROM mobil`: Bagian kueri ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.
3. `WHERE harga_rental >= 50000`: Bagian query ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data dimana harga_rental (harga sewa) lebih besar atau sama dengan 50.000.
## Kesimpulan
Hasil dari perintah tersebut akan mengembalikan semua baris dari tabel "mobil" di mana nilai kolom "harga_rental" lebih besar dari atau sama dengan 50.000. Semua kolom dari baris-baris yang memenuhi kondisi tersebut akan ditampilkan dalam hasilnya.
# <> atau !=
## Struktur Query
```mysql
select * from nama_tabel where kolom1 <> nilai1;
```
## Contoh Query
```mysql
select * from mobil where harga_rental <> 50000;
```

## Hasil
![image](aset/s7.png)
## Analisis
1. `SELECT *`: Bagian kueri ini menentukan bahwa Anda ingin mengambil semua kolom dari tabel seluler.
2. `FROM mobil`: Bagian kueri ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.
3. `WHERE harga_rental <> 50000`: Bagian kueri ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data yang harga_rental (harga sewa) tidak sama dengan 50.000.
## Kesimpulan
Hasil dari perintah tersebut akan mengembalikan semua baris dari tabel "mobil" di mana nilai kolom "harga_rental" tidak sama dengan 50.000. Semua kolom dari baris-baris yang tidak memenuhi kondisi tersebut akan ditampilkan dalam hasilnya.
# IN
## Stuktur Query
```mysql
 select * from nama_tabel where kolom in('nilai1','nilai2');
```
## Contoh Query
```mysql
 select * from mobil where warna in('silver','merah');
```
## Hasil 
![image](aset/s8.png)
## Analisis
1. `SELECT *`: Bagian kueri ini menentukan bahwa Anda ingin mengambil semua kolom dari tabel seluler.
2. `FROM mobil`: Bagian kueri ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari tabel mobile.
3. `WHERE warna IN ('silver', 'merah')`: Bagian kueri ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data yang warnanya 'silver' atau 'merah'.
## Kesimpulan
Hasil dari perintah tersebut akan mengembalikan semua baris dari tabel "mobil" di mana nilai kolom "warna" adalah 'silver' atau 'merah'. Semua kolom dari baris-baris yang memenuhi kondisi tersebut akan ditampilkan dalam hasilnya

# IN +AND
## Struktur Query          
```mysql
select * from nama_tabel
-> where nama_kolom in ('nilai','nilai2')
-> AND nama_kolom = nilai3
```
## Contoh Query
```mysql
select * from mobil
    -> where warna IN ('hitam','silver')
    -> and harga_rental = 50000;
```
## Hasil
![image](aset/s9.png)

## Analisis
- `SELECT *`: Bagian kueri ini menentukan bahwa Anda ingin mengambil semua kolom dari `mobil`tabel.
- `FROM mobil`: Bagian kueri ini menentukan tabel tempat Anda ingin mengambil data. Dalam hal ini, Anda ingin mengambil data dari `mobil`tabel.
- `WHERE warna IN ('hitam', 'silver') AND harga_rental = 50000`: Bagian kueri ini menentukan kondisi yang harus dipenuhi data agar dapat diambil. Dalam hal ini, Anda ingin mengambil data yang `warna`(warnanya) adalah 'hitam' atau 'perak' dan `harga_rental`(harga sewa) sama dengan 50.000.
## Kesimpulan
perintah tersebut digunakan untuk mencari mobil dengan warna 'hitam' atau 'silver' dan harga sewa sebesar 50.000 dari tabel "mobil".  

# IN + OR
## Struktur Query
```mysql
select * from nama_tabel
-> where nama_kolom in ('nilai','nilai2')
-> OR nama_kolom = nilai3
```

## Contoh Query
```mysql
select * from mobil
    -> where warna IN ('hitam','silver')
    -> and harga_rental = 50000;
```
## Hasil
![image](aset/s10.png)

## Analisis
1. `warna IN ('hitam', 'silver')`: Kondisi ini akan memfilter baris berdasarkan kolom "warna", memeriksa apakah nilainya adalah "hitam" atau "silver". Perintah ini akan memilih hanya baris-baris di mana warnanya adalah hitam atau silver.
2. `harga_rental = 50000`: Kondisi ini akan memfilter baris berdasarkan kolom "harga_rental", memilih hanya baris-baris di mana harga sewanya adalah 50.000
## Kesimpulan
semua baris dari tabel "`mobil`" yang memiliki warna "`hitam`" atau "`silver`" dan harga_rental sebesar `50000`.

# IN + AND + OPERATOR 
## Struktur Query
```mysql
select * from nama_tabel
-> where nama_kolom in ('nilai','nilai2')
-> AND nama_kolom > nilai3
```

```mysql
select * from nama_   tabel
-> where nama_kolom in ('nilai','nilai2')
-> AND nama_kolom < nilai3
```
## Contoh Query
```mysql
select * from mobil
    -> where warna IN ('hitam','silver')
    -> and harga_rental > 50000;
```

```mysql
select * from mobil
    -> where warna IN ('hitam','silver')
    -> and harga_rental < 50000;
```

## Hasil
![image](aset/s11.png)
![image](aset/s12.png)

### Analisis
1. `warna IN ('hitam', 'silver')`: Kondisi ini akan memfilter baris berdasarkan kolom "warna", memeriksa apakah nilainya adalah "hitam" atau "silver". Perintah ini akan memilih hanya baris-baris di mana warnanya adalah hitam atau silver.
2. `harga_rental > 50000`: Kondisi ini akan memfilter baris berdasarkan kolom "harga_rental", memilih hanya baris-baris di mana harga sewanya lebih besar dari 50.000.
### Kesimpulan
emua baris dari tabel "`mobil`" yang memiliki warna "`hitam`" atau "`silver`" dan `harga_rental` kurang dari `50000`.
# LIKE
## Mencari Awalan
### Struktur Query
```mysql
 select * from mobil
-> where pemilik like 'ad%';
```

### Contoh Query
```mysql
select * from [nama_tabel]
-> where [nama_kolom] like 'nama_awal';
```
### Hasil
![IMAGE](s13.png)
### Analisis
`pemilik LIKE 'ad%'`: Kondisi ini akan memfilter baris berdasarkan kolom "pemilik", mencocokkan nilai dengan pola yang diberikan. Dalam hal ini, pola yang diberikan adalah 'ad%', yang berarti mencari nilai pemilik yang dimulai dengan huruf 'ad'. Tanda '%' dalam pola tersebut menunjukkan bahwa ada nol atau lebih karakter setelah 'ad'.
### Kesimpulan
semua baris dari tabel "`mobil`" di mana nilai kolom "`pemilik`" dimulai dengan huruf '`ad`'.

## Mencari Akhiran
###  Struktur Query
```mysql
SELECT * FROM mobil  
-> WHERE pemilik LIKE '%i';
```
### Contoh Query
```mysql
select * from [nama_tabel]
-> where [nama_kolom] like 'nama_akhir';
```
### Hasil
![image](aset/s14.png)
### Analisis
`pemilik LIKE '%i'`: Kondisi ini akan memfilter baris berdasarkan kolom "pemilik", mencocokkan nilai dengan pola yang diberikan. Dalam hal ini, pola yang diberikan adalah '%i', yang berarti mencari nilai pemilik yang diakhiri dengan huruf 'i'. Tanda '%' di depan pola menunjukkan bahwa ada nol atau lebih karakter sebelum 'i'.
### Kesimpulan 
Hanya mobil-mobil yang memiliki nilai pada kolom "`pemilik`" yang diakhiri dengan huruf '`i`' yang akan dipilih.
## Mencari Awalan & Akhiran
### Struktur Query
```mysql
select * from [nama_tabel]
-> where [nama_kolom] like 'namaawal%namakhir';
```
### Contoh Query
```mysql
select * from mobil
-> where pemilik like 'r%i';
```
### Hasil
![image](aset/s15.png)
### Analisis
- `pemilik LIKE`: Mengindikasikan pencocokan pola pada kolom "pemilik".
- `'r%i'`: Pola yang digunakan untuk pencocokan. Huruf 'r' menunjukkan bahwa nilai kolom "pemilik" harus diawali dengan huruf 'r', sedangkan '%i' menunjukkan bahwa setelah huruf 'r', ada nol atau lebih karakter, dan diakhiri dengan huruf 'i'.
### Kesimpulan
yang memiliki nilai pada kolom "pemilik" yang diawali dengan huruf 'r', diikuti oleh nol atau lebih karakter, dan diakhiri dengan huruf 'i' yang akan dipilih.
## Mencari berdasarkan total karakter
### Struktur Query
```mysql
select * from [nama_tabel]
-> where [nama_kolom] like 'awalan___';
```
### Contoh Query
```mysql
select * from mobil
-> where pemilik like 'r___';
```
### Hasil
![image](aset/s16.png)
### Analisis
1.`pemilik LIKE 'r___'`: Kondisi ini akan memfilter baris berdasarkan kolom "pemilik", mencocokkan nilai dengan pola yang diberikan. Dalam hal ini, pola yang diberikan adalah 'r___', yang berarti mencari nilai pemilik yang terdiri dari lima karakter, di mana karakter pertama adalah 'r' dan tiga karakter berikutnya boleh apa saja.
### Kesimpulan 
digunakan untuk mencari total karakter
## Kombinasi
### Struktur Query
```mysql
select * from [nama_tabel]
-> where [nama_kolom] like '___akhiran%';
```
### Contoh Query
```mysql
select * from mobil
-> where pemilik like '___i%';
```
### Hasil

### Analisis
`pemilik LIKE '___i%'`: Kondisi ini akan memfilter baris berdasarkan kolom "pemilik", mencocokkan nilai dengan pola yang diberikan. Dalam hal ini, pola yang diberikan adalah '___i%', yang berarti mencari nilai pemilik yang terdiri dari setidaknya empat karakter, di mana karakter ketiga adalah 'i', dan karakter-karakter berikutnya boleh apa saja
### Kesimpulan

## Not like
### Struktur Query
```mysql
select * from [nama_tabel] where [namakolom] not like 'awalan%';
```
### Contoh Query
```mysql
select * from mobil where peminjam not like 'r%';
```
### Hasil
![image](aset/s17.png)
### Analisis
### Kesimpulan
# NULL & NOT NULL
## Mencari data kosong
### Struktur Query
```mysql
SELECT * FROM [namatabel] WHERE [namakolom] IS NULL;
```
### Contoh Query
```mysql
SELECT * FROM mobil WHERE peminjam IS NULL;
```
### Hasil
![image](aset/s18.png)
### Analisis
- `SELECT`: Digunakan untuk memilih kolom atau data yang ingin ditampilkan dalam hasil query.
- _Tanda asterisk (_) digunakan sebagai wildcard dalam SQL, yang berarti "semua kolom". Dalam konteks ini, "* "menunjukkan bahwa semua kolom dalam tabel "mobil" akan ditampilkan dalam hasil query.
- `FROM`: Digunakan untuk menentukan tabel sumber data dari mana data akan diambil. Dalam hal ini, tabel sumber data adalah "mobil".
- `mobil`: Nama tabel yang spesifik di mana data akan diambil.
- `WHERE`: Digunakan untuk memberikan kriteria atau kondisi yang harus dipenuhi untuk mengambil data yang relevan. Dalam kasus ini, kondisi adalah "peminjam IS NULL", yang berarti hanya baris dengan kolom "peminjam" yang memiliki nilai `NULL` yang akan dimasukkan dalam hasil query.
### Kesimpulan
Perintah `SELECT *` digunakan untuk memilih semua kolom dari tabel '`mobil`'. Kemudian, `FROM mobil` menunjukkan tabel yang digunakan untuk mengambil data, yaitu tabel '`mobil`'. Selanjutnya, `WHERE peminjam IS NULL` menggunakan klausa `WHERE` untuk memfilter baris-baris yang akan diambil. Kondisi peminjam IS NULL digunakan untuk memeriksa apakah nilai kolom '`peminjam`' adalah `NULL`. Operator `IS NULL` digunakan untuk memeriksa apakah nilai kolom adalah NULL. Dengan demikian, query ini akan mengembalikan baris-baris di mana kolom 'peminjam' memiliki nilai `NULL`.
## Mencari data yang tidak kosong
### Struktur Query
```mysql
SELECT * FROM [namatabel] WHERE [namakolom] IS NOT NULL;
```
### Contoh Query
```mysql
SELECT * FROM mobil WHERE peminjam IS NOT NULL;
```
### Hasil
![image](aset/s19.png)
### Analisis
- `SELECT`: Digunakan untuk memilih kolom atau data yang ingin ditampilkan dalam hasil query.
- _: Tanda (_) digunakan sebagai wildcard dalam SQL, yang berarti "semua kolom". Dalam konteks ini, "* "menunjukkan bahwa semua kolom dalam tabel "mobil" akan ditampilkan dalam hasil query.
- `FROM`: Digunakan untuk menentukan tabel sumber data dari mana data akan diambil. Dalam hal ini, tabel sumber data adalah "mobil".
- `mobil`: Nama tabel yang spesifik di mana data akan diambil.
- `WHERE`: Digunakan untuk memberikan kriteria atau kondisi yang harus dipenuhi untuk mengambil data yang relevan. Dalam kasus ini, kondisi adalah "peminjam IS NOT NULL", yang berarti hanya baris dengan kolom "peminjam" yang memiliki nilai tidak NULL yang akan dimasukkan dalam hasil query.
### Kesimpulan
Perintah SQL SELECT * FROM mobil WHERE peminjaman IS NOT NULL; digunakan untuk mengambil semua baris dari tabel "mobil" di mana kolom "peminjaman" memiliki nilai yang tidak NULL. Dengan kata lain, perintah ini mengambil data mobil yang sedang dipinjam atau sudah dipinjam dari tabel tersebut.
# ORDEY BY & LIMIT 8
## Mengurutkan data dari data terkecil
### Struktur Query
```mysql
SELECT * FROM [namatabel] ORDER BY namakolom ASC;
```
### Contoh Query
```mysql
SELECT * FROM mobil ORDER BY pemilik ASC;
```
### Hasil
![image](aset/s20.png)
### Analisis
- SELECT: Digunakan untuk memilih kolom atau data yang ingin ditampilkan dalam hasil query.
- _: Tanda asterisk (_) digunakan sebagai wildcard dalam SQL, yang berarti "semua kolom". Dalam konteks ini, "* "menunjukkan bahwa semua kolom dalam tabel "mobil" akan ditampilkan dalam hasil query.
- FROM: Digunakan untuk menentukan tabel sumber data dari mana data akan diambil. Dalam hal ini, tabel sumber data adalah "mobil".
- mobil: Nama tabel yang spesifik di mana data akan diambil.
- ORDER BY: Digunakan untuk mengurutkan hasil query berdasarkan kolom tertentu.
- pemilik: Nama kolom yang akan digunakan sebagai kriteria pengurutan. Dalam kasus ini, kolom "pemilik" akan digunakan.
- ASC: Singkatan dari "ascending" yang menandakan pengurutan secara menaik (dari nilai terkecil ke nilai terbesar).
### Kesimpulan
Perintah SQL ini memberikan hasil berupa semua data yang ada dalam tabel "mobil", diurutkan berdasarkan kolom "pemilik" secara menaik. Hasilnya akan mengembalikan semua baris dalam tabel "mobil" dalam urutan yang diinginkan.
## Mengurutkan data dari data terbesar
### Struktur Query
```mysql
SELECT * FROM [namatabel] ORDER BY namakolom ASC;
```
### Contoh Query
```mysql
SELECT * FROM mobil ORDER BY peminjam DESC;
```
### Hasil
![image](aset/s21.png)
### Analisis
- SELECT: Digunakan untuk memilih kolom atau data yang ingin ditampilkan dalam hasil query.
- _: Tanda asterisk (_) digunakan sebagai wildcard dalam SQL, yang berarti "semua kolom". Dalam konteks ini, "* "menunjukkan bahwa semua kolom dalam tabel "mobil" akan ditampilkan dalam hasil query.
- FROM: Digunakan untuk menentukan tabel sumber data dari mana data akan diambil. Dalam hal ini, tabel sumber data adalah "mobil".
- mobil: Nama tabel yang spesifik di mana data akan diambil.
- ORDER BY: Digunakan untuk mengurutkan hasil query berdasarkan kolom tertentu.
- peminjam: Nama kolom yang akan digunakan sebagai kriteria pengurutan. Dalam kasus ini, kolom "peminjam" akan digunakan.
- DESC: Singkatan dari "descending" yang menandakan pengurutan secara menurun (dari nilai terbesar ke nilai terkecil).
### Kesimpulan
Perintah SQL ini menghasilkan semua data yang ada dalam tabel "mobil" dan mengurutkannya secara menurun berdasarkan kolom "peminjam". Urutan menurun (descending) ditentukan oleh kata kunci "DESC" yang digunakan dalam perintah "ORDER BY".

## Membatasi data yang tampil
```mysql
select * from mobil where warna = "hitam" order by harga asc limit 2;
```

# DISTINCT
## Struktur Query
```mysql
SELECT DISTINCT(namakolom) FROM namatabel;
```

```mysql
SELECT DISTINCT(namakolom) FROM namatabel ORDER BY namakolom DESC;
```
## Contoh Query
```mysql
SELECT DISTINCT(pemilik) FROM mobil;
```

```mysql
SELECT DISTINCT(harga_rental) FROM mobil ORDER BY harga_rentalDESC;
```
## Hasil
![image](aset/s22.png)
![image](aset/s23.png)
## Analisis
1. SELECT DISTINCT(harga_rental): Perintah ini mengambil nilai unik dari kolom "harga_rental" dalam tabel "mobil". Klausa DISTINCT digunakan untuk memastikan bahwa hanya nilai unik yang diambil, sehingga tidak ada duplikasi dalam hasil.

2. FROM mobil: Ini menunjukkan bahwa tabel yang digunakan dalam perintah ini adalah "mobil". Pastikan tabel "mobil" ada dalam database yang aktif.

3. ORDER BY harga_rental DESC: Ini adalah klausa yang digunakan untuk mengurutkan nilai unik "harga_rental" secara menurun (descending). DESC adalah kata kunci yang menunjukkan urutan menurun.

## Kesimpulan
Perintah SQL ini memberikan hasil berupa nilai unik dari kolom "harga_rental" dalam tabel "mobil", diurutkan secara menurun. Hasilnya akan mengembalikan daftar harga rental yang unik dalam urutan menurun.

# CONCAT, CONCAT_WS, AS
## Menggabungkan kolom tanpa pemisah
### Struktur Query
```mysql
SELECT CONCAT(nama_kolom) FROM nama_tabel;
```
### Contoh Query
```mysql
SELECT CONCAT(pemilik,warna) FROM daftar_mobil;
```
### Hasil
![image](aset/s25.png)
### Analisis
1. SELECT CONCAT(pemilik, warna): Perintah ini menggunakan fungsi CONCAT untuk menggabungkan nilai dari kolom "pemilik" dan "warna" dalam tabel "daftar_mobil". Fungsi CONCAT digunakan untuk menggabungkan dua atau lebih string menjadi satu string.
    
2. FROM daftar_mobil: Ini menunjukkan bahwa tabel yang digunakan dalam perintah ini adalah "daftar_mobil". Pastikan tabel "daftar_mobil" ada dalam database yang aktif.
### Kesimpulan
Perintah SQL ini menghasilkan hasil berupa string yang merupakan hasil penggabungan nilai dari kolom "pemilik" dan "warna" dalam tabel "daftar_mobil".
## Menggabungkan kolom dengan pemisah
### Struktur Query
```mysql
SELECT CONCAT_WS("-",nama2_kolom) FROM nama_tabel;
```
### Contoh Query
```mysql
SELECT CONCAT_WS("-",no_plat,no_mesin,id_mobil) FROM daftar_mobil;
```
### Hasil
![image](aset/s26.png)
### Analisis
1. SELECT CONCAT_WS("-", no_plat, no_mesin, id_mobil): Perintah ini menggunakan fungsi CONCAT_WS untuk menggabungkan nilai dari kolom "no_plat", "no_mesin", dan "id_mobil" dalam tabel "daftar_mobil". Fungsi CONCAT_WS (Concatenate With Separator) menggabungkan nilai-nilai string dengan memasukkan pemisah yang ditentukan di antara mereka.
    
2. FROM daftar_mobil: Ini menunjukkan bahwa tabel yang digunakan dalam perintah ini adalah "daftar_mobil". Pastikan tabel "daftar_mobil" ada dalam database yang aktif.
### Kesimpulan
Perintah SQL ini menghasilkan hasil berupa string yang merupakan hasil penggabungan nilai dari kolom "no_plat", "no_mesin", dan "id_mobil" dalam tabel "daftar_mobil", dengan pemisah tanda hubung ("-") di antara mereka.
## Memberikan nama kolom alias
### Struktur Query
```mysql
SELECT CONCAT_WS("+",nama2_kolom) AS nama_kolom_baru FROM nama_tabel;
```
### Contoh Query
```mysql
SELECT CONCAT_WS("+",pemilik,peminjaman) AS COLLAB FROM mobil;
```
### Hasil
![image](aset/s27.png)
### Analisis
1. SELECT CONCAT_WS("+", pemilik, peminjaman) AS COLLAB: Perintah ini menggunakan fungsi CONCAT_WS untuk menggabungkan nilai dari kolom "pemilik" dan "peminjaman" dalam tabel "mobil". Fungsi CONCAT_WS (Concatenate With Separator) menggabungkan nilai-nilai string dengan memasukkan pemisah yang ditentukan di antara mereka. Dalam hal ini, pemisah yang digunakan adalah tanda tambah ("+"). Alias "COLLAB" digunakan untuk memberi nama kolom hasil penggabungan.

2. FROM mobil: Ini menunjukkan bahwa tabel yang digunakan dalam perintah ini adalah "mobil". Pastikan tabel "mobil" ada dalam database yang aktif.
### Kesimpulan
Perintah SQL ini menghasilkan hasil berupa kolom baru yang bernama "COLLAB", yang berisi string hasil penggabungan nilai dari kolom "pemilik" dan "peminjaman" dalam tabel "mobil", dengan pemisah tanda tambah ("+") di antara mereka.

# VIEW
## Membuat tabel virtual
### Struktur Query
```mysql
CREATE VIEW nama_kolom_baru AS
-> SELECT nama2_kolom
-> FROM nama_tabel;
-> WHERE nama_kolom = isi_kolom;
```
### Contoh Query
```mysql
CREATE VIEW info_no_platt AS
-> SELECT id_mobil, no_plat, pemilik, peminjaman
-> FROM daftar_mobil
-> WHERE pemilik = "ADEL";
```
### Hasil
![image](aset/s28.png)
### Analisis
1. CREATE VIEW info_no_platt: Ini adalah perintah untuk membuat view baru dengan nama "info_no_platt". View adalah objek database yang berfungsi sebagai tabel virtual yang terdiri dari hasil query yang ditentukan.

2. SELECT id_mobil, no_plat, pemilik, peminjaman: Ini adalah perintah SELECT yang digunakan dalam pembuatan view. Perintah ini menentukan kolom mana yang akan dipilih dari tabel "daftar_mobil" untuk dimasukkan ke dalam view "info_no_platt".

3. FROM daftar_mobil: Ini menunjukkan bahwa view "info_no_platt" akan dibuat berdasarkan data yang ada di tabel "daftar_mobil". Pastikan tabel "daftar_mobil" ada dalam database yang aktif.

4. WHERE pemilik = 'ADEL': Ini adalah klausa WHERE yang digunakan untuk memberikan kondisi untuk memilih hanya baris yang memiliki nilai pemilik sama dengan 'ADEL'. Hal ini akan memfilter data yang dimasukkan ke dalam view sehingga hanya data dengan pemilik "ADEL" yang akan ditampilkan.
### Kesimpulan
Perintah SQL ini membuat sebuah view baru dengan nama "info_no_platt" yang berisi data dari tabel "daftar_mobil" dengan kondisi bahwa pemilik mobil adalah "ADEL". View ini akan berisi kolom "id_mobil", "no_plat", "pemilik", dan "peminjaman" untuk baris-baris yang memenuhi kondisi tersebut.

## Menampilkan tabel virtual
### Struktur Query
```mysql
SELECT * FROM nama_tabel_baru b ;
```
### Contoh Query
```mysql
SELECT * FROM info_no_plat;
```
### Hasil
![image](aset/s29.png)
### Analisis
1. SELECT _: Perintah ini digunakan untuk memilih semua kolom yang ada dalam view "info_no_plat". Tanda "_" menunjukkan bahwa semua kolom akan dipilih.

2. FROM info_no_plat: Ini menunjukkan bahwa data akan diambil dari view "info_no_plat". Pastikan view "info_no_plat" sudah dibuat sebelumnya.
### Kesimpulan
Perintah SQL ini mengambil semua data yang ada dalam view "info_no_plat" dan mengembalikannya sebagai hasil query.
## Menghapus tabel virtual
### Struktur Query
```mysql
DROP VIEW nama_tabel_baru;
```
### Contoh Query
```mysql
DROP VIEW info_no_plat;
```
### Hasil
![image](aset/s30.png)
### Analisis
DROP VIEW info_no_plat: Ini adalah perintah untuk menghapus view dengan nama "info_no_plat" dari database. Perintah DROP VIEW digunakan untuk menghapus view yang telah dibuat sebelumnya.
### Kesimpulan
Perintah SQL ini menghapus view "info_no_plat" dari database.

# Tantangan View
## Nomor 1
### Penjelasan
CREATE VIEW mobil_tanpa_peminjam AS : adalah perintah untuk membuat sebuah view baru atau seperti tabel baru dalam basis data dengan nama mobil_tanpa_peminjam.
- `SELECT no_plat, peminjaman` : adalah perintah untuk memilih dua kolom, yaitu `no_plat` dan `peminjam`, dari tabel `mobil`.
-` FROM mobil` : Menunjukkan bahwa data diambil dari tabel bernama mobil.
-` WHERE peminjam IS NULL` :  adalah klausa `WHERE` yang mencari baris-baris dari tabel mobil dimana nilai kolom peminjam adalah `NULL`.
- `SELECT *`: adalah perintah untuk memilih semua kolom dari view atau tabel.
- `FROM mobil_Tanpa_peminjam`: Menunjukkan bahwa data diambil dari view yang disebut mobil_Tanpa_peminjam, yang telah dibuat sebelumnya.

### Query
```mysql
CREATE VIEW
-> mobil_tanpa_peminjam AS
-> SELECT no_plat,peminjaman
-> FROM mobil
-> WHERE peminjaman IS NULL;
```
### Hasil
![image](aset/s31.png)
### Kesimpulan
`CREATE VIEW mobil_tanpa_peminjam AS Select no_plat, peminjaman FROM mobil WHERE peminjaman IS NULL;` digunakan untuk membuat sebuah view baru bernama` mobil_Tanpa_peminjam`. Viewnya berisi dua kolom, yaitu no_plat dan peminjaman, yang diambil dari tabel mobil hanya baris-baris yang memiliki nilai `NULL` pada kolom peminjam yang dimasukkan ke dalam view. 
`SELECT * FROM `mobil_tanpa_peminjam; digunakan untuk menampilkan semua data dari view mobil_Tanpa_peminjam, yang telah dibuat sebelumnya dengan kriteria yang bernilai NULL.
## Nomor 2
### Penjelasan
- `UPDATE mobil`: adalah perintah untuk memperbarui data dalam tabel yang disebut mobil.
- `SET peminjaman = NULL` : menetapkan nilai kolom peminjam menjadi NULL.
- `WHERE peminjam= 'ADEL'` : adalah klausa WHERE yang membatasi update hanya pada baris-baris dimana nilai kolom peminjam adalah 'ADEL'. Maksudnya perubahan hanya akan berlaku untuk baris-baris yang memiliki peminjam dengan nama 'ADEL'.
- `SELECT *`: adalah perintah untuk memilih semua kolom dari view atau tabel.
- `FROM mobil_tanpa_peminjam`: Menunjukkan bahwa data diambil dari view yang disebut "mobil_tanpa_peminjam", yang telah dibuat sebelumnya.

### Query
```mysql
UPDATE mobil
    -> SET peminjaman = NULL
    -> WHERE peminjaman = 'ADEL';
```

### Hasil
![gambar](ASET/2.png)

![[1 1.png]]

### Kesimpulan
`UPDATE mobil SET peminjaman = NULL WHERE peminjaman = 'ADEL';` nilai pada kolom peminjaman pada tabel `mobil`yang memiliki nilai 'ADEL' akan diubah menjadi NULL.
Kesimpulannya, perintah digunakan untuk menghapus atau mengubah nilai peminjaman menjadi NULL untuk semua data di tabel mobil yang berada di kolom `peminjaman`memiliki nilai 'ADEL'.
`SELECT * FROM mobil_tanpa_peminjam; `digunakan untuk menampilkan semua data dari view mobil_tanpa_peminjam, yang telah dibuat sebelumnya dengan mengubah atau menghapus nilai peminjam menjadi NULL untuk tabel mobil dimana peminjam memiliki nilai ADEL.
## Nomor 3
View digunakan untuk menyaring data sesuai dengan kriteria tertentu, seperti menampilkan data yang memiliki nilai NULL pada kolom tertentu atau mengubah salah satu data peminjaman menjadi NULL. Memberikan pandangan yang jelas tentang mobil yang tersedia untuk disewakan atau yang belum memiliki peminjam.
Dengan membuat view, kita dapat membatasi akses ke data sensitif atau kolom tertentu dari tabel yang mungkin tidak perlu diakses oleh semua pengguna.
Dengan membuat view untuk kueri yang sering digunakan, Anda dapat menghindari pengulangan kode SQL yang sama di beberapa tempat dalam aplikasi atau prosedur penyimpanan.

# AGREGASI
## SUM
### Penjelasan
- SELECT SUM(harga_rental) : Fungsi SUM() digunakan untuk menghitung total atau jumlah dari semua nilai dalam kolom harga_rental.
- FROM mobil : Menentukan tabel mobil dari mana data akan diambil.
### Struktur Query
```mysql
SELECT SUM(nama_kolom) FROM nama_tabel;
```

### Contoh Query
```mysql
SELECT SUM(harga_rental) FROM mobil;
```

### Hasil
![image](aset/s32.jpeg)

### Kesimpulan
Query  SELECT SUM(harga_rental) FROM mobil; akan menghitung dan menampilkan total atau jumlah keseluruhan dari nilai-nilai yang terdapat pada kolom harga_rental di dalam tabel mobil. Hasil query ini akan memberikan informasi total atau keseluruhan harga rental untuk semua mobil yang ada di dalam tabel tersebut.
## Count
### Penjelasan
PENJELASAN 1
- SELECT COUNT(pemilik) - Fungsi COUNT() digunakan untuk menghitung jumlah baris atau record yang ada di dalam kolom pemilik.
- FROM mobil - Menentukan tabel mobil dari mana data akan diambil.

PENJELASAN 2
- SELECT COUNT(peminjaman) - Fungsi COUNT() digunakan untuk menghitung jumlah baris atau record yang ada di dalam kolom peminjaman.
- FROM mobil - Menentukan tabel mobil dari mana data akan diambil.
### Struktur Query
```mysql
SELECT COUNT(nama_kolom) FROM nama_tabel;
SELECT COUNT(nama_kolom) FROM nama_tabel;
```

### Contoh Query
```mysql
SELECT COUNT(pemilik) FROM mobil;
SELECT COUNT(peminjaman) FROM mobil;
```

### Hasil
![image](aset/s33.jpeg)
### Kesimpulan
KESIMPULAN 1
Query SELECT COUNT(pemilik) FROM mobil; akan menghitung dan menampilkan jumlah total pemilik mobil yang ada di dalam tabel mobil. Hasil query ini akan memberikan informasi tentang berapa banyak pemilik mobil yang tercatat di dalam tabel tersebut.

KESIMPULAN 2
Query SELECT COUNT(peminjaman) FROM mobil; akan menghitung dan menampilkan jumlah total peminjaman mobil yang ada di dalam tabel mobil. Hasil query ini akan memberikan informasi tentang berapa banyak peminjaman mobil yang tercatat di dalam tabel tersebut.
## MIN
### Penjelasan
- SELECT MIN(harga_rental) : Fungsi MIN() digunakan untuk mencari nilai minimum (terkecil) dari kolom harga_rental.
- AS MINIMAL : Hasil dari fungsi MIN() akan ditampilkan dengan nama alias "MINIMAL".
- FROM mobil : Menentukan tabel mobil dari mana data akan diambil.
### Struktur Query
```mysql
SELECT MIN(nama_kolom) AS nilai_minimum FROM nama_tabel;
```

### Contoh Query
```mysql
SELECT MIN(harga_rental) AS MINIMAL FROM mobil;
```

### Hasil
![image](aset/s34.jpeg)

### Kesimpulan
Query SELECT MIN(harga_rental) AS MINIMAL FROM mobil; akan mencari dan menampilkan harga rental mobil yang paling murah atau terkecil dari semua data yang ada di dalam tabel mobil. Hasil query ini akan memberikan informasi tentang harga rental mobil terendah yang tercatat di dalam tabel tersebut.
## MAX
### Penjelasan
- SELECT MAX(harga_rental) : Fungsi MAX() digunakan untuk mencari nilai maksimum (terbesar) dari kolom harga_rental.
- AS MAXIMAL : Hasil dari fungsi MAX() akan ditampilkan dengan nama alias "MAXIMAL".
- FROM mobil : Menentukan tabel mobil dari mana data akan diambil.
### Struktur Query
```mysql
SELECT MAX(nama_kolom) AS nilai_minimum FROM nama_tabel;
```

### Contoh Query
```mysql
SELECT MAX(harga_rental) AS MAXIMAL FROM mobil;
```

### Hasil
![image](aset/s35.jpeg)

### Kesimpulan
Query SELECT MAX(harga_rental) AS MAXIMAL FROM mobil; akan mencari dan menampilkan harga rental mobil yang paling mahal atau terbesar dari semua data yang ada di dalam tabel mobil. Hasil query ini akan memberikan informasi tentang harga rental mobil tertinggi yang tercatat di dalam tabel tersebut.
## AVG
### Penjelasan
- SELECT AVG(harga_rental) : Fungsi AVG() digunakan untuk menghitung rata-rata (average) dari nilai-nilai pada kolom harga_rental.
- AS RATA_RATA : Hasil dari fungsi AVG() akan ditampilkan dengan nama alias "RATA_RATA".
- FROM mobil : Menentukan tabel mobil dari mana data akan diambil.
### Struktur Query
```mysql
SELECT AVG(nama_kolom) AS rata_rata FROM nama_tabel;
```

### Contoh Query
```mysql
SELECT AVG(harga_rental) AS RATA_RATA FROM mobil;
```

### Hasil
![image](aset/s36.jpeg)

### Kesimpulan
Query SELECT AVG(harga_rental) AS RATA_RATA FROM mobil; akan menghitung dan menampilkan rata-rata (average) harga rental mobil dari semua data yang ada di dalam tabel mobil. Hasil query ini akan memberikan informasi tentang harga rental mobil rata-rata yang tercatat di dalam tabel tersebut.


















