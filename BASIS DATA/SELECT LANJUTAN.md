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
![[Pasted image 20240220142420.png]]
## Analisis

## Kesimpulan

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
![[Pasted image 20240220142727.png]]

## Analisis
## Kesimpulan 

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
![[Pasted image 20240220143115.png]]

## Analisis

## Kesimpulan

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
![[Pasted image 20240220143950.png]]
## Analisis
## Kesimpulan

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
![[Pasted image 20240220144312.png]]

## Analisis 
## Kesimpulan 

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
![[Pasted image 20240220144847.png]]
## Analisis

## Kesimpulan

# <> atau !=
## Struktur Query
```mysql
select * from nama_tabel where kolom1 <= nilai1;
```
## Contoh Query
```mysql
select * from mobil where harga_rental <> 50000;
```

## Hasil
![[Pasted image 20240220150303.png]]
## Analisis
## Kesimpulan

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
![[Pasted image 20240220150818.png]]
## Analisis
## Kesimpulan

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
![[Pasted image 20240220151506.png]]

## Analisis
## Kesimpulan

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
![[Pasted image 20240220152051.png]]

## Analisis
## Kesimpulan

# IN + AND + OPERATOR 
## Struktur Query
```mysql
select * from nama_tabel
-> where nama_kolom in ('nilai','nilai2')
-> AND nama_kolom > nilai3
```

```mysql
select * from nama_tabel
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
![[Pasted image 20240220152653.png]]
![[Pasted image 20240220152953.png]]