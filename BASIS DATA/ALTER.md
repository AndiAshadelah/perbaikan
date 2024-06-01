![[Pasted image 20240423134833.png]]
# Menambahkan Kolom
## Struktur Query
```mysql
alter table nama_tabel add nama_kolom_baru varchar(10) after namakolom;
```
## Contoh Query
```mysql
alter table mobil add batas_peminjam varchar(10) after peminjam;
```
## Hasil
![[Pasted image 20240423135109.png]]
## Analisis
**AFTER** : opsional untuk digunakan, jika tidak 
**FIRST** : 
## Kesimpulan

## Tambahan
### Struktur Query
### Contoh Query
```mysql
 update mobil set batas_peminjam = "24-04-2023" where peminjam is not null;
```
### Hasil
![[Pasted image 20240423142042.png]]

# Mengubah nama kolom
## Struktur Query
```mysql
 alter table namatabel change namakolom namaygdiganti varchar(10);
```
## Contoh Query
```mysql
 alter table mobil change batas_peminjam deadline varchar(10);
```
## Hasil
![[Pasted image 20240423142911.png]]
## Analisis
## Kesimpulan
# Mengubah tipe data
## Struktur Query
## Contoh Query 
```mysql
alter table mobil modify deadline date;
```

## Hasil
![[Pasted image 20240423145808.png]]
## Analisis
## Kesimpulan
## Tambahan
### Contoh Query
### Hasil


# Menambahkan constraint
![[Pasted image 20240423145705.png]]

# Menghapus constraint
# Menghapus kolom
# Mengganti nama tabel

## Contoh Query
```mysql
alter table rename to daftar_mobil;
```
## Hasil
![[Pasted image 20240423153327.png]]

