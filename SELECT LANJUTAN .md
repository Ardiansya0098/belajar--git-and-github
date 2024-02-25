# AND
## Struktur

```mysql
select nama_kolom1,nama_kolom2 from nama_tabel where nama_kolom3"nilai_kolom1" and nama_kolom4"nilai_kolom2";
```

## Contoh

```mysql
select warna,pemilik from desc_mobil where warna="Hitam" and pemilik="Ibrahim";
```

## Hasil

![And.](And.jpg)

## Analisis 

- `SELECT warna, pemilik`: Perintah ini menginstruksikan database untuk mengambil kolom `warna` dan `pemilik` dari tabel.
- `FROM desc_mobil`: Ini menentukan tabel yang akan digunakan untuk mengambil data, yaitu `desc_mobil`.
- `WHERE warna="Hitam" AND pemilik="Ibrahim"`: Ini adalah klausul WHERE yang digunakan untuk memfilter baris-baris dalam tabel `desc_mobil`. Hanya baris-baris yang memenuhi kedua kondisi ini yang akan dipilih: warna mobil harus "Hitam" dan pemilik mobil harus "Ibrahim".

Jadi, query tersebut akan mengambil warna dan pemilik mobil dari tabel `desc_mobil` dimana warna mobil adalah "Hitam" dan pemilik mobil adalah "Ibrahim".

## Kesimpulan 

Query tersebut mengambil data dari tabel `desc_mobil` di mana nilai kolom `warna` adalah "Hitam" dan nilai kolom `pemilik` adalah "Ibrahim". Jadi Hasil kesimpulannya akan menampilkan kolom `warna` dan `pemilik` untuk baris-baris yang memenuhi kondisi tersebut.

# OR
## Struktur

```mysql
select nama_kolom1,nama_kolom2 from nama_tabel where nama_kolom3"nilai_kolom1" or nama_kolom4"nilai_kolom2";
```

## Contoh

```mysql
select warna,pemilik from desc_mobil where warna="Hitam" or pemilik="Ibrahim";
```

## Hasil

![[OR.jpg]]

## Analisis 

-  `SELECT`: Ini adalah kata kunci yang digunakan untuk memilih kolom-kolom tertentu dari tabel.
-  `warna, pemilik`: Ini adalah daftar kolom yang dipilih untuk diekstraksi dari tabel `desc_mobil`. Dalam hal ini, kita akan mendapatkan nilai dari kolom `warna` dan `pemilik`.
-  `FROM desc_mobil`: Ini menentukan bahwa data akan diambil dari tabel bernama `desc_mobil`.
-  `WHERE`: Ini adalah kata kunci yang digunakan untuk memberikan kriteria seleksi untuk baris-baris yang akan diambil. Hanya baris-baris yang memenuhi kriteria ini yang akan ditampilkan.
-  `warna="Hitam" or pemilik="Ibrahim"`: Ini adalah kriteria seleksi. Ini berarti kita hanya ingin baris-baris di mana nilai kolom `warna` adalah "Hitam" atau nilai kolom `pemilik` adalah "Ibrahim".

Jadi, secara keseluruhan, ini akan mengembalikan semua baris dari tabel `desc_mobil` di mana nilai kolom `warna` adalah "Hitam" atau nilai kolom `pemilik` adalah "Ibrahim", dan hanya kolom `warna` dan `pemilik` yang akan ditampilkan.
 
## Kesimpulan 

- `Kolom warna`: Berisi warna mobil yang cocok dengan kriteria "Hitam".

- `Kolom pemilik`: Berisi nama pemilik mobil yang cocok dengan kriteria "Ibrahim".

Jadi, kesimpulan dari query ini adalah mengembalikan daftar mobil dengan warna "Hitam" atau dimiliki oleh "Ibrahim".

# BETWEEN-AND
## Struktur

```mysql
select * from nama_tabel where nama_kolom between nilai_kolom1 and nilai_kolom2;
```

## Contoh

```mysql
select * from desc_mobil where harga_rental between 100000 and 200000;
```

## Hasil

![[between and.jpg]]

## Analisis

-  `SELECT *`: Ini menunjukkan bahwa kita ingin mengambil semua kolom dari tabel `desc_mobil`.

-  `FROM desc_mobil`: Ini menunjukkan bahwa kita ingin mengambil data dari tabel bernama `desc_mobil`.

-  `WHERE harga_rental BETWEEN 100000 AND 200000`: Ini adalah klausa yang membatasi hasil query. Kita hanya akan mengambil baris-baris di mana nilai `harga_rental` berada di antara 100.000 dan 200.000.

Jadi, secara keseluruhannya ialah akan mengambil semua kolom dari tabel `desc_mobil` di mana nilai `harga_rental` berada di antara 100.000 dan 200.000.

## Kesimpulan

mengambil semua kolom dari tabel desc_mobil di mana nilai kolom harga_rental berada dalam rentang antara 100.000 dan 200.000. Ini berarti hasilnya akan berisi semua entri mobil yang memiliki harga sewa antara 100.000 dan 200.000.

# NOT BETWEEN
## Struktur

```mysql
select * from nama_tabel where nama_kolom not between nilai_kolom1 and nilai_kolom2;
```

## Contoh

```mysql
select * from desc_mobil where harga_rental not between 100000 and 200000;
```

### Hasil

![[not between and.jpg]]

## Analisis

- `SELECT *` : Memilih semua kolom dari tabel.
 
 - `FROM desc_mobil`: Menentukan tabel yang digunakan untuk melakukan seleksi, yaitu tabel desc_mobil.

- `WHERE harga_rental NOT BETWEEN 100000 AND 200000`: Mengaplikasikan kondisi dimana nilai dalam kolom harga_rental tidak berada di antara 100.000 dan 200.000.

Jadi, hasil query akan mengembalikan semua baris dari tabel desc_mobil dimana nilai dalam kolom harga_rental tidak berada di antara 100.000 dan 200.000.

## Kesimpulan 

memilih semua entri dari tabel `desc_mobil` di mana nilai kolom `harga_rental` tidak berada di antara 100.000 dan 200.000. Ini akan mengambil semua data mobil yang memiliki harga sewa di luar rentang tersebut.

# <=
## Struktur

```mysql
select * from nama_tabel where nama_kolom <= nilai_kolom;
```

## Contoh

```mysql
select * from desc_mobil where harga_rental <= 50000;
```

## Hasil

![[lebih kecil sama dengan.jpg]]

## Analisis 

 `SELECT * FROM desc_mobil WHERE harga_rental <= 50000;` Ini berarti Anda ingin mengambil semua data dari tabel `desc_mobil` di mana nilai dalam kolom `harga_rental` kurang dari atau sama dengan 50000.

- `SELECT *`: Ini berarti Anda ingin mengambil semua kolom dari tabel.
- `FROM desc_mobil`: Ini menunjukkan bahwa Anda ingin mengambil data dari tabel bernama `desc_mobil`.
- `WHERE harga_rental <= 50000;`: Ini adalah klausa WHERE yang membatasi baris yang akan dikembalikan. Hanya baris dengan nilai `harga_rental` kurang dari atau sama dengan 50000 yang akan disertakan dalam hasilnya.

Jadi, secara keseluruhan, ini akan mengembalikan semua data dari tabel `desc_mobil` di mana nilai dalam kolom `harga_rental` kurang dari atau sama dengan 50000.

## Kesimpulan 

meminta untuk memilih semua kolom dari tabel `desc_mobil` di mana nilai pada kolom `harga_rental` kurang dari atau sama dengan 50.000. Ini akan menghasilkan daftar semua mobil yang memiliki harga rental kurang dari atau sama dengan 50.000.

# >=
## Struktur

```mysql
select * from nama_tabel where nama_kolom >= nilai_kolom;
```

## Contoh

```mysql
select * from desc_mobil where harga_rental >= 50000;
```

## Hasil

![[lebih besar sama dengan 1.jpg]]

## Analisis 

- `SELECT *`: Mengambil semua kolom dari tabel `desc_mobil`.
- `FROM desc_mobil`: Menunjukkan bahwa data akan diambil dari tabel bernama `desc_mobil`.
- `WHERE harga_rental >= 50000`: Menyaring baris-baris di mana nilai pada kolom `harga_rental` lebih besar atau sama dengan 50000.

Jadi, query ini akan mengembalikan semua baris dari tabel `desc_mobil` di mana nilai pada kolom `harga_rental` lebih besar atau sama dengan 50000.

## Kesimpulan

menampilkan semua kolom dari tabel desc_mobil di mana nilai harga_rental lebih besar atau sama dengan 50000. Artinya, Anda ingin menampilkan semua entri mobil yang memiliki harga sewa 50000 atau lebih.

# <> ATAU !=
## Struktur

```mysql
select * from nama_tabel where nama_kolom <> nilai_kolom;
```

## Contoh

```mysql
select * from desc_mobil where harga_rental <> 50000;
```

## Hasil

![[atau.jpg]]

## Analisis

 menggunakan perintah SQL `SELECT * FROM desc_mobil WHERE harga_rental <> 50000;` yang bertujuan untuk mengambil semua data dari tabel `desc_mobil` di mana nilai pada kolom `harga_rental` tidak sama dengan 50000.

- `SELECT *`: Memilih semua kolom dari tabel `desc_mobil`.
- `FROM desc_mobil`: Menentukan tabel yang akan digunakan, yaitu `desc_mobil`.
- `WHERE harga_rental <> 50000`: Menetapkan kriteria pencarian dengan menyatakan bahwa hanya baris-baris yang memiliki nilai `harga_rental` yang tidak sama dengan 50000 yang akan dipilih.

Jadi, hasilnya akan mengembalikan semua baris dari tabel `desc_mobil` di mana nilai pada kolom `harga_rental` tidak sama dengan 50000.

## Kesimpulan

akan mengembalikan semua baris dari tabel `desc_mobil` di mana nilai dalam kolom `harga_rental` tidak sama dengan 50000. Dengan kata lain, nilai tersebut akan mengambil semua data mobil yang memiliki harga sewa yang tidak sama dengan 50000.
