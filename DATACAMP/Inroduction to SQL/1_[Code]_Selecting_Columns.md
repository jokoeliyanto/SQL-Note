# Memilih Kolom dengan `SELECT`
Pada bab ini kita belajar comman dasar pada SQL untuk melakukan seleksi baik kolom atau baris berdasarkan kriteria tertentu. Selain itu kita juga belajar beberapa fungsi agregasi dasar seperti 'SUM', 'AVG', dan lainnya.

## Bagian 1: Command Seleksi Dasar
- SELECT (single)
- SELECT (multiple)
- SELECT DISTINCT

Catatan Penting:
- `*` : Memilih semua kolom
- `SELECT` : Command untuk melakukan query
- `DISTINCT` :  Memilih semua nilai unik dalam sebuah kolom

#### LATIHAN: Memilih Sebuah Kolom
Memilih sebuah kolom tertentu dari Tabel `films`
```sql
SELECT ___
FROM films;
```
Memilih kolom `title` dari tabel `films`
```sql
SELECT title
FROM films;
```
Memilih kolom `release_year` dari tabel `films`
```sql
SELECT release_year
FROM films;
```
Memilih kolom `name` dari tabel `films`
```sql
SELECT name
FROM people;
```
#### LATIHAN: Memilih Beberapa Kolom
Memilih kolom `title` dari tabel `films`
```sql
SELECT title
FROM films;
```
Memilih kolom `title`, `release_year` dari tabel `films`
```sql
SELECT title, release_year
FROM films;
```
Memilih kolom `title`, `release_year`, `country` dari tabel `films`
```sql
SELECT title, release_year, country
FROM films;
```
Memilih semua kolom dari tabel `films`
```sql
SELECT *
FROM films;
```
#### LATIHAN: Memilih Nilai Unik Pada Sebuah Kolom
Memilih nilai-nilai unik(daftar negara asal film) pada kolom `country` dari tabel `films` 
```sql
SELECT DISTINCT country
FROM films;
```
Memilih nilai-nilai unik(jenis sertifikasi film) pada kolom `certifications` dari tabel `films` 
```sql
SELECT DISTINCT certification
FROM films;
```
Memilih nilai-nilai unik(jenis role) pada kolom `role` dari tabel `films`
```sql
SELECT DISTINCT role
FROM roles;
```

## Bagian 1: Fungsi Agregasi Dasar
- COUNT
- COUNT DISTINCT
- COUNT(column_name) vs COUNT(\*)
- SUM (single)
- AVG (single)
- MIN (single)
- MAX (single)

Catatan Penting:
- `COUNT` : Menghitung jumlah baris tak kosong pada sebuah kolom
- `SUM` : Menjumlahkan nilai-nilai numerik pada sebuah kolom
- `AVG` :  Menghitung nilai rata-rata numerik pada sebuah kolom
- `MIN` :  Menghitung nilai minimum numerik pada sebuah kolom
- `MAX` :  Menghitung nilai maksimum numerik pada sebuah kolom
- 
#### LATIHAN: Fungsi Agregasi Pada SQL

```sql
SELECT COUNT(*)
FROM people;
```




















