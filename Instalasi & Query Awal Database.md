# Instalasi MysQL

## Menggunakan termux

1. Buka Aplikasi Termux
2. Ketik "termux-setup-storage"
3. Ketik izinkan/allow access
4. Lakukan update atau upgrade paket. Ketik "pkg update && upgrade -y"
5. jika ada informasi untuk melanjutkan instalasi ketik "y"
6. Hasil aplikasi mariadb dengan mengetik "pkg install mariadb"
7. Ketika proses berhenti dan ada pilihan "y/n" ketik saja "y" untuk melanjutkan proses penginstalan
8. ketik "mysqld_safe" untuk memberi keamanan.
9. Ketik CNTRL+Z agar bisa ngesave datanya.
## Referensi Link Vidio YouTube 

https://youtu.be/dmhJQ4zs_WY?si=yLCNgx8ZNHbEbFDx
# Penggunaan Awal MySQL

## QUERY
Printah `CREATE DATABASE nama_database;` digunakan untuk membuat basis data baru di Mysql.

`CREATE DATABASE xi_rpl_1;`

digunakan untuk membuat sebuah database baru dengan nama `xi_rpl_1`. Database tersebut akan menjadi wadah untuk menyimpan tabel, relasi, dan data terkait dalam sistem manajemen basis data yang digunakan.

## HASIL

![[show_tbl.jpg.jpg]]

## ANALISIS

Perintah `CREATE DATABASE xi_rpl_1;`digunakan untuk membuat sebuah database baru dengan nama "xi_rpl_1". Database ini akan digunakan untuk menyimpan semua struktur dan data.

## Kesimpulan

Perintah `CREATE DATABASE xi_rpl_1;` digunakan untuk membuat sebuah database baru dengan nama "xi_rpl_1". Dengan menggunakan perintah ini, Anda membuat ruang penyimpanan yang terorganisir di dalam sistem manajemen basis data yang digunakan untuk menyimpan tabel dan data,

## Mysql
MySQL merujuk pada proses evaluasi dan pemahaman kinerja serta efisiensi operasi basis data menggunakan MySQL. Ini melibatkan pemantauan kinerja, identifikasi masalah kinerja, optimasi kueri, tuning konfigurasi server, dan penerapan praktik terbaik untuk meningkatkan kinerja dan efisiensi basis data.
## -u
Opsi `-u` pada perintah MySQL digunakan untuk menentukan pengguna (user) yang akan digunakan untuk login ke server MySQL. Misalnya, jika Anda ingin login sebagai pengguna "username", Anda dapat menggunakan `-u`.  

## root
Root pada MySQL merujuk kepada akun pengguna dengan hak akses tertinggi (superuser). Akun root memiliki semua hak akses ke semua basis data dan tabel di server MySQL. Ini adalah akun yang memiliki kekuatan penuh untuk mengelola dan mengontrol konfigurasi serta operasi MySQL, termasuk membuat, menghapus, dan mengatur izin pengguna lainnya. Oleh karena itu, sangat penting untuk menjaga keamanan akun root dan hanya menggunakan aksesnya dengan bijaksana.
## -p
Opsi `-p` pada perintah MySQL digunakan untuk meminta penggunaan kata sandi (password) saat mencoba untuk login ke server MySQL. Saat Anda menggunakan `-p` dalam perintah mysql, sistem akan meminta Anda untuk memasukkan kata sandi pengguna yang sesuai dengan pengguna yang ditentukan dengan opsi `-u` (jika digunakan). Misalnya, jika Anda menggunakan `mysql -u username -p`, Anda akan diminta untuk memasukkan kata sandi untuk pengguna "username" sebelum dapat login ke server MySQL.

## KESIMPULAN 
Mysql adalah perintah untuk memulai klien MySQL Command Line Interface (CLI), yang memungkinkan Anda berinteraksi dengan server MySQL dari baris perintah.

- -u: `u` pada MySQL adalah bahwa opsi tersebut digunakan untuk menentukan pengguna (user) yang akan digunakan untuk login ke server MySQL. Dengan menggunakan `-u`, Anda dapat menyediakan nama pengguna yang sesuai dengan akun yang ingin Anda gunakan untuk mengakses server MySQL.

- root: adalah bahwa "root" merujuk kepada akun pengguna dengan hak akses tertinggi (superuser) dalam sistem manajemen basis data MySQL. Akun "root" memiliki semua hak akses ke semua basis data dan tabel di server MySQL dan memiliki kekuatan penuh untuk mengelola, mengontrol, dan mengatur konfigurasi serta operasi MySQL.

- -p: Argumen ini memberi tahu klien MySQL bahwa Anda ingin memasukkan kata sandi setelah menjalankan perintah ini untuk otentikasi. Setelah Anda mengetikkan perintah dan menekan Enter, sistem akan meminta Anda untuk memasukkan kata sandi.
# Database
## Buat Database

### query
Perintah CREATE DATABASE xi_rpl_1; digunakan untuk membuat sebuah database baru dengan nama "xi_rpl_1". Jika database dengan nama yang sama sudah ada, perintah ini akan menghasilkan pesan kesalahan karena database dengan nama yang sama tidak dapat dibuat duplikat.

### hasil

![[buatdtbs.jpg.jpg]]

### analisis 
Di sini, nama_database adalah nama yang Anda inginkan untuk basis data baru yang akan Anda buat. Misalnya, jika Anda ingin membuat basis data dengan nama "tokobuku", Anda akan menulis: CREATE DATABASE;

### kesimpulan 
kesimpulan dari proses membuat database berserta format di MySQL adalah bahwa ini adalah langkah penting dalam mempersiapkan lingkungan pengembangan data yang sesuai dan merupakan fondasi untuk pengembangan aplikasi yang sukses.


## Tampilkan Database 

### query
Perintah `SHOW DATABASES;` digunakan untuk menampilkan daftar semua database yang ada dalam sistem manajemen basis data yang sedang digunakan. Ini memberikan gambaran tentang semua database yang tersedia untuk digunakan oleh pengguna yang sedang aktif.

### hasil

![[Tampilkan database.jpg]]

### analisis
Perintah ini akan menghasilkan output yang berisi daftar semua basis data yang ada di server MySQL. Untuk menampilkan informasi lebih lanjut tentang sebuah basis data tertentu, Anda dapat menggunakan perintah SHOW  DATABASES nama_database;. Ini akan menampilkan pernyataan SQL yang digunakan untuk membuat basis data tersebut, termasuk karakter set dan kolasi yang digunakan

### kesimpulan 
perintah SHOW DATABASES; adalah alat yang penting dalam administrasi dan pengelolaan basis data di MySQL karena memberikan daftar semua basis data yang tersedia, memudahkan navigasi di antara basis data, dan membantu dalam pengambilan keputusan terkait struktur data.


## Hapus Database

### query
Perintah `DROP DATABASE xi_rpl_1;` digunakan untuk menghapus database dengan nama "xi_rpl_1" beserta semua tabel dan data yang ada di dalamnya. Ini adalah perintah yang bersifat permanen dan akan menghapus seluruh struktur dan informasi yang terkait dengan database tersebut dari sistem manajemen basis data yang digunakan.

### hasil

![[hapus database.jpg]]

### analisis
Di sini, x1_ adalah nama basis data yang ingin Anda hapus. Misalnya, jika Anda ingin menghapus basis data dengan nama "tokobuku", Anda akan menulis: DROP DATABASE;

### kesimpulan 
kesimpulan dari proses menghapus database berserta format di MySQL adalah bahwa ini adalah tindakan serius yang memerlukan pertimbangan dan persiapan yang matang untuk memastikan bahwa data tidak hilang secara tidak sengaja dan bahwa dampaknya dipahami dengan baik.

## Gunakan Database

### query 
`USE xi_rpl_1;`. Perintah ini digunakan untuk beralih konteks ke database "xi_rpl_1", sehingga semua perintah SQL yang dijalankan setelahnya akan berlaku untuk database tersebut.

### hasil

![[Gunakan database.jpg]]

### analisis
Perintah `USE DATABASE xi_rpl_1;` digunakan untuk beralih ke database "xi_rpl_1" sehingga semua perintah SQL yang dijalankan setelahnya akan berlaku untuk database tersebut. Ini memungkinkan Anda untuk bekerja dengan tabel, relasi, dan data yang tersimpan di dalam database "xi_rpl_1". Dengan beralih ke database tertentu, Anda dapat menjalankan query yang terkait dengan operasi pembacaan atau penulisan data ke dalam database tersebut, serta melakukan operasi lain seperti membuat tabel baru, menghapus data, dan mengubah struktur tabel.

### kesimpulan 
Kesimpulannya, penggunaan basis data di MySQL berserta formatnya melibatkan pemahaman tentang desain data, penggunaan SQL, keamanan, dan kinerja. Pemahaman ini diperlukan untuk memastikan pengelolaan data yang efektif dan aplikasi yang dapat diandalkan.

# Tipe Data
## Angka
- Integer (Bilangan Bulat): Digunakan untuk menyimpan bilangan bulat tanpa desimal, seperti 1, -5, atau 100.

- Float (Bilangan Desimal): Untuk menyimpan angka dengan desimal, seperti 3.14 atau -0.5.

- Long (Bilangan Bulat Panjang): Digunakan untuk menyimpan bilangan bulat yang sangat besar.

- Complex (Bilangan Kompleks): Untuk menyimpan angka kompleks yang terdiri dari bagian real dan imajiner.
## Teks
- String: Tipe data yang digunakan untuk menyimpan teks atau karakter. String diwakili oleh serangkaian karakter yang diapit oleh tanda kutip, baik itu tunggal (') atau ganda ("). Contoh: 'hello', "world", atau '123abc'.

- Char: Tipe data yang digunakan untuk menyimpan satu karakter. Char diwakili oleh tanda kutip tunggal (''). Contoh: 'a', 'b', atau '1'.

## Tanggal
- Date (Tanggal): Tipe data yang digunakan untuk merepresentasikan tanggal. Biasanya terdiri dari tahun, bulan, dan hari. Beberapa bahasa pemrograman memiliki tipe data khusus untuk tanggal, misalnya datetime.date di Python.

- Datetime (Tanggal dan Waktu): Tipe data yang digunakan untuk merepresentasikan tanggal dan waktu. Selain tahun, bulan, dan hari, tipe data ini juga menyertakan informasi waktu seperti jam, menit, dan detik. Contoh: 2024-01-27 15:30:00.
## Boolean
- adalah tipe data yang menyimpan nilai true atau false. Dalam konteks penggunaannya, nilai true direpresentasikan oleh 1 dan false direpresentasikan oleh 0. Tipe data boolean umumnya digunakan untuk menyimpan data biner, seperti status aktif/non-aktif, atau untuk mengekspresikan kebenaran suatu pernyataan dalam Query MYSQL. Misalnya, `SELECT * FROM tabel WHERE kondisi = TRUE;` akan mengembalikan baris-baris di mana kondisi yang dinyatakan benar.

## Tipe Data Pilihan 

### ENUM
ENUM adalah jenis data dalam SQL yang digunakan untuk mendefinisikan kumpulan nilai yang mungkin untuk sebuah kolom. Dengan ENUM, Anda dapat membatasi nilai yang dapat dimasukkan ke dalam kolom tersebut hanya pada satu dari beberapa nilai yang telah ditentukan.

### SET
Dalam konteks SQL, `SET` adalah klausa yang digunakan untuk menetapkan nilai ke variabel sistem, atau untuk mengatur pengaturan tertentu dalam sesi koneksi saat ini. Ini dapat digunakan untuk berbagai tujuan, seperti mengatur variabel lingkungan, mengatur pengaturan sesi, atau mengonfigurasi parameter yang berpengaruh pada operasi database.

# Tabel 

## Buat Tabel
### Struktur

```Mysql
 CREATE TABLE nama_table (
 nama_kolom_1 tipe_data(max karakter) constraint,
 nama_kolom_2 tipe_data(max karakter) constraint,
 nama_kolom_3 tipe_data(max karakter),
 ...);
```

### Contoh

```mysql
CREATE TABLE karyawan (
    -> nis_karyawan int(4) primary key not null,
    -> nama_asli varchar(25) not null,
    -> nama_panggilan varchar(25),
    -> no_telp char(12) unique );
```

## Tampilkan Tabel Database

### Hasil

![[h_table1.jpeg.jpg]]

### Analisis

1. `CREATE TABLE karyawan (:` Menunjukkan dimulainya perintah untuk membuat sebuah tabel dengan nama "karyawan".

2. `nis_karyawan int(4) primary key not null,`: Mendefinisikan kolom "nis_karyawan" dengan tipe data integer dan panjang maksimum 4 digit. Ini juga menetapkan kolom tersebut sebagai kunci utama (primary key) yang tidak boleh bernilai null, sehingga setiap baris dalam tabel harus memiliki nilai unik untuk kolom ini.

3. `nama_asli varchar(25) not null,`: Mendefinisikan kolom "nama_asli" dengan tipe data varchar yang dapat menyimpan string hingga 25 karakter. Kolom ini tidak boleh bernilai null.

4. `nama_panggilan varchar(25),`: Mendefinisikan kolom "nama_panggilan" dengan tipe data varchar yang dapat menyimpan string hingga 25 karakter. Kolom ini dibiarkan nullable, artinya nilainya bisa kosong.

5. `no_telp char(12) unique );`: Mendefinisikan kolom "no_telp" dengan tipe data char yang dapat menyimpan string dengan panjang tepat 12 karakter. Kolom ini diberi konstrain unik (unique constraint), yang berarti tidak boleh ada dua baris dengan nilai yang sama dalam kolom ini.

### Kesimpulan

1. `nis_karyawan` dengan tipe data `int` (bilangan bulat) dengan panjang maksimum 4 digit, dan diatur sebagai kunci utama (`primary key`) yang tidak boleh bernilai `NULL`.

2. `nama_asli` dengan tipe data `varchar` (string karakter variabel) dengan panjang maksimum 25 karakter, dan diatur sebagai kolom yang tidak boleh bernilai `NULL`.

3. `nama_panggilan` dengan tipe data `varchar` (string karakter variabel) dengan panjang maksimum 25 karakter. Kolom ini dapat bernilai `NULL`.

4. `no_telp` dengan tipe data `char` (string karakter tetap) dengan panjang tepat 12 karakter, dan diatur sebagai kolom unik (`unique`), yang berarti tidak ada dua entri yang dapat memiliki nomor telepon yang sama.

## QNA

>[!Faq]- Mengapa hanya kolom id_pelanggan yang menggunakan constraint PRIMARY KEY?
> Adalah kolom yang unik dan berfungsi sebagai identifikasi utama untuk setiap baris dalam tabel. Ini memastikan bahwa setiap baris dalam tabel memiliki nilai `id_pelanggan` yang unik dan tidak boleh null, yang berguna untuk keperluan pengindeksan dan pengelompokan data. Kolom lain mungkin tidak menggunakan constraint `PRIMARY KEY` karena mungkin tidak memiliki sifat yang sama seperti `id_pelanggan`, atau mungkin ada kolom lain yang bisa digunakan sebagai kunci primer alternatif.

>[!Faq]- Mengapa pada no_telp yang menggunakan tipe data char bukan varchar?
>`char` biasanya digunakan ketika panjang data dalam kolom selalu tetap atau hampir tetap. Ini mengalokasikan ruang yang tetap untuk setiap nilai dalam kolom, yang dapat meningkatkan efisiensi pencarian dan penyimpanan data, terutama jika semua nilai dalam kolom memiliki panjang yang sama.
>`Varchar` cocok digunakan ketika panjang data dalam kolom bervariasi dan tidak tetap. Ini mengalokasikan ruang yang sesuai dengan panjang aktual data yang disimpan, yang lebih hemat ruang jika panjang data bervariasi.

>[!Faq]- Mengapa hanya kolom no_telp yang menggunakan constraint UNIQUE?
>Constraint `UNIQUE` memastikan bahwa setiap nilai dalam kolom `no_telp` harus unik di antara semua baris dalam tabel, yang merupakan sifat yang penting untuk nomor telepon karena setiap nomor telepon harus unik untuk setiap pelanggan atau entitas yang direkam dalam basis data.

>[!Faq]- Mengapa kolom no_telp tidak memakai constraint NOT NULL, sementara kolom lainnya menggunakan constraint tersebut?
>Kolom `no_telp` mungkin tidak menggunakan constraint `NOT NULL` karena dalam beberapa kasus, nomor telepon mungkin tidak selalu tersedia atau tidak wajib diisi.

>[!Faq]- Perbedaan PK & Unique
>Pk:
>Digunakan untuk mengidentifikasi secara unik setiap baris dalam tabel.
Setiap tabel hanya dapat memiliki satu primary key.
Kolom primary key tidak boleh berisi nilai NULL.
Otomatis menciptakan indeks unik untuk mempercepat pencarian dan pengindeksan. 
Unique:
Menjamin bahwa setiap nilai dalam kolom tersebut adalah unik.
Tabel dapat memiliki beberapa kolom yang memiliki constraint UNIQUE.
Memungkinkan nilai NULL, kecuali jika Anda menetapkan NOT NULL bersamaan dengan UNIQUE.
Digunakan untuk memastikan bahwa tidak ada duplikasi nilai dalam kolom tertentu.

# Insert

## Insert 1 data
### Struktur

```mysql
insert into nama_tabel  values("nilai_kolom1","nilai_kolom2","nilai_kolom3","nilai_kolom4");
```


### Contoh

```mysql
insert into karyawan
values("1","ardiansya","ardi","085333405540");
```

### Hasil

![[insert 1 data.jpg.jpg]]

### Analisis

adalah sebuah perintah SQL untuk memasukkan data baru ke dalam tabel `karyawan`. Perintah `INSERT INTO` digunakan untuk menambahkan satu baris data baru ke dalam tabel yang sudah ada. 

Diikuti dengan `VALUES`, yang merupakan kata kunci yang menunjukkan bahwa kita akan menyediakan nilai untuk setiap kolom yang ada di dalam tabel. Setelah itu, dalam tanda kurung, kita menyediakan nilai untuk setiap kolom sesuai dengan urutan kolom dalam tabel.

data yang akan dimasukkan ialah:

- `"1"` untuk kolom pertama, yang mungkin merupakan ID karyawan.
- `"ardiansya"` untuk kolom kedua, mungkin nama belakang.
- `"ardi"` untuk kolom ketiga, mungkin nama depan.
- `"085333405540"` untuk kolom keempat, mungkin nomor telepon.

Setelah itu, query diakhiri dengan tanda titik koma (`;`) yang menandakan akhir perintah SQL.

### Kesimpulan

perintah untuk memasukkan data baru ke dalam tabel "karyawan" dengan nilai kolom-kolom yang disediakan.

- **Tabel**: `karyawan`
- **Kolom yang dimasukkan**: `id`, `nama`, `username`, `nomor_telepon`
- **Nilai yang dimasukkan**:
  - `id`: "1"
  - `nama`: "ardiansya"
  - `username`: "ardi"
  - `nomor_telepon`: "085333405540"

Ini akan membuat sebuah baris baru di tabel "karyawan" dengan nilai-nilai yang diberikan.

## Insert >1 data
### Struktur 

```mysql
insert into nama_tabel
values("nilai_kolom1","nilai_kolom2","nilai_kolom3","nilai_kolom4"),
("nilai_kolom1","nilai_kolom2","nilai_kolom3","nilai_kolom4"),
("nilai_kolom1","nilai_kolom2","nilai_kolom3","nilai_kolom4");
```

### Contoh

```mysql
insert into karyawan
values ("2","farhan","far","08431279465"),
("3","fadhilamir","fadil","08846379542"),
("4","alfazari","raihan","08613452764");
```


### Hasil

![[insert lebih besar 1.jpg.jpg]]

### Analisis 

- Perintah: `INSERT INTO karyawan`

- Data yang dimasukkan:

  1. Set 1: ("2", "farhan", "far", "08431279465")
  2.  Set 2: ("3", "fadhilamir", "fadil", "08846379542")
  3.  Set 3: ("4", "alfazari", "raihan", "08613452764")

- Tabel Tujuan: `karyawan`

-  Kolom yang diisi: 

2. `id_karyawan`: Nilai dari kolom ini adalah "2", "3", dan "4" untuk masing-masing set data.

3. `​nama_depan`: Nilai dari kolom ini adalah "farhan", "fadhilamir", dan "alfazari" untuk masing-masing set data.

4. `nama_belakang`: Nilai dari kolom ini adalah "far", "fadil", dan "raihan" untuk masing-masing set data.

5. `no_telepon`: Nilai dari kolom ini adalah "08431279465", "08846379542", dan "08613452764" untuk masing-masing set data.

 ini bertujuan untuk memasukkan tiga baris data ke dalam tabel `karyawan`, dengan setiap baris mewakili informasi tentang seorang karyawan termasuk ID karyawan, nama depan, nama belakang, dan nomor telepon mereka.

### Kesimpulan 

Perintah `INSERT INTO` yang digunakan untuk memasukkan data ke dalam tabel `karyawan`. Terdapat tiga set data yang dimasukkan, masing-masing terdiri dari empat nilai yang dipisahkan oleh koma. Setiap set data tersebut mengandung informasi untuk kolom-kolom dalam tabel `karyawan`, yaitu `id_karyawan`, `nama_depan`, `nama_belakang`, dan `no_telepon`.

## Menyebut Kolom
### Struktur

```mysql
insert into nama_table
    (nama_kolom1,nama_kolom2) values ("nilai_kolom1","nilai_kolom2");
```

### Contoh

```mysql
insert into karyawan
    (nama_asli,nis_karyawan) values ("agus","5");
```

### Hasil

![[menyebut kolom.jpg.jpg]]

### Analisis

Merupakan perintah untuk menambahkan data baru ke dalam tabel `karyawan`. 

- `INSERT INTO karyawan`: Ini adalah pernyataan SQL yang menunjukkan bahwa kita ingin menyisipkan data ke dalam tabel bernama `karyawan`.

- `(nama_asli, nis_karyawan)`: Bagian ini menentukan kolom-kolom di mana data akan dimasukkan. Dalam hal ini, kolom yang ditentukan adalah `nama_asli` dan `nis_karyawan`.

- `VALUES ("agus", "5")`: Ini adalah nilai yang ingin dimasukkan ke dalam kolom yang telah ditentukan sebelumnya. `"agus"` akan dimasukkan ke dalam kolom `nama_asli`, dan `"5"` akan dimasukkan ke dalam kolom `nis_karyawan`.

Jadi, secara keseluruhanya ialah akan menambahkan sebuah baris baru ke dalam tabel `karyawan` dengan nilai `"agus"` untuk kolom `nama_asli` dan nilai `"5"` untuk kolom `nis_karyawan`.

### Kesimpulan 

Adalah memasukkan record baru ke dalam tabel “karyawan” dengan nilai “agus” untuk kolom “nama_asli” dan “5” untuk kolom “nis_karyawan”.

# Select
## Seluruh Data
### Struktur

```mysql
select * from nama_tabel;
```

### Contoh

```mysql
select * from karyawan;
```


### Hasil

![[select.jpg.jpg]]

### Analisis 

`SELECT * FROM karyawan;`: mengambil semua kolom dan baris dari tabel bernama "karyawan." Ini adalah kueri dasar tanpa kondisi atau filter tertentu, yang memberikan tampilan komprehensif data di tabel "karyawan".

### Kesimpulan

 `"select * from karyawan;"` akan mengambil semua data (semua kolom) dari tabel "karyawan" dalam database yang sedang digunakan. Kesimpulannya adalah bahwa kita sedang mencoba untuk menampilkan semua informasi yang terkandung dalam tabel "karyawan".

## Data kolom tertentu 
### Struktur

```mysql
select nama_kolom1,nama_kolom2,nama_kolom3,nama_kolom4 from nama_table;
```

### Contoh

```mysql
select nama_asli from karyawan;
```

### Hasil

![[data kolom.jpg.jpg]]

### Analisis 

- `SELECT`: Kata kunci yang digunakan untuk memilih kolom atau data yang ingin ditampilkan.
- `nama_asli`: Nama kolom yang ingin ditampilkan.
- `FROM`: Kata kunci yang menunjukkan tabel sumber dari mana data akan diambil.
- `karyawan`: Nama tabel dari mana data akan diambil.

Jadi, perintah ini akan mengambil data dari kolom `nama_asli` dari tabel `karyawan`.

### Kesimpulan 

 `SELECT nama_asli FROM karyawan;` adalah pernyataan yang digunakan untuk mengambil data dari kolom `nama_asli` dari tabel `karyawan`. 

## Klausa Where
### Struktur

```mysql
select * from nama_table where nama_kolom;
```

### Contoh

```mysql
select * from karyawan
    where nis_karyawan=2;
```

### Hasil

![[klausa where.jpg.jpg]]

### Analisis 

- `SELECT`: Mengambil semua kolom dari tabel "karyawan".

- `FROM karyawan`: Menentukan tabel yang akan digunakan adalah "karyawan".

- `WHERE nis_karyawan=2`: Menerapkan kondisi seleksi dimana hanya baris-baris yang memiliki nilai kolom "nis_karyawan" sama dengan 2 yang akan dipilih.

Jadi, ini akan mengembalikan semua informasi mengenai karyawan yang memiliki nilai "nis_karyawan" sama dengan 2.

### Kesimpulan 

Adalah perintah untuk memilih semua kolom dari tabel `karyawan` di mana nilai kolom `nis_karyawan` sama dengan 2. Berarti ini akan mengembalikan semua informasi yang terkait dengan karyawan yang memiliki `nis_karyawan` sama dengan 2.

# Update (data)
## Struktur 

```mysql
update nama_tabel set nama_kolom1"nilai1" where nama_kolom2"nilai2;
```

## Contoh 

```mysql
update karyawan set no_telp="086451334044" where nis_karyawan="4";
```

## Hasil

![[update baris.jpg.jpg]]

## Analisis 

- `UPDATE karyawan`: Bagian ini menentukan tabel yang akan diperbarui, yaitu "karyawan" dalam hal ini.

- `SET no_telp="086451334044"`: Bagian ini menetapkan nilai kolom "no_telp" menjadi "086451334044" untuk record yang sesuai dengan kondisi yang ditentukan pada klausa WHERE.

- `WHERE nis_karyawan="4"`: Bagian ini menentukan kondisi yang harus dipenuhi oleh catatan agar dapat diperbarui. Dalam hal ini, memperbarui record dimana nilai pada kolom "nis_karyawan" sama dengan "4".

## Kesimpulan 

sebuah perintah SQL untuk mengubah nilai kolom nama_asli menjadi "ardiansya" di dalam tabel karyawan dimana nis_karyawan memiliki nilai "4". Kesimpulannya, perintah tersebut bertujuan untuk memperbarui data karyawan dengan nis_karyawan tertentu dengan no_telp "086451334044".

# Delete (Hapus baris data)
## Struktur

```mysql
DELETE FROM nama_tabel WHERE nama_kolom"nilai_kolom";
```

## Contoh

```mysql
DELETE FROM karyawan WHERE nis_karyawan="3";
```

## Hasil

![[delete nama tabel.jpg.jpg]]

## Analisis

**Perintah:** `DELETE FROM karyawan`
- Ini adalah perintah untuk menghapus data dari tabel "karyawan".

**Kondisi WHERE:** `nis_karyawan=3
- Ini adalah klausa WHERE yang menentukan kriteria untuk baris-baris yang akan dihapus. Dalam hal ini, baris akan dihapus jika nilai kolom "nis_karyawan" sama dengan 3.

**Tabel:** `karyawan`
- Ini adalah nama tabel yang akan dihapus barisnya.

## Kesimpulan

Perintah SQL di atas menghapus baris data dari tabel "karyawan" di mana nilai kolom "nis_karyawan" sama dengan "3". Kesimpulannya, program ini digunakan untuk menghapus informasi karyawan dengan nomor identitas "3" dari basis data.

# Hapus Tabel
## Struktur

```mysql
drop table nama_table;
```

## Contoh

```mysql
drop table pelanggan;
```

## Hasil

![[hapus table hs.jpg.jpg]]

## Analisis 

"drop table pelanggan;" adalah tentang perintah SQL untuk menghapus tabel bernama "pelanggan" dari database. 

1. **Drop Table**: Ini adalah perintah SQL yang digunakan untuk menghapus tabel dari database.
  
2. **Pelanggan**: Ini adalah nama tabel yang akan dihapus.

Jadi, secara keseluruhan, query tersebut akan menghapus tabel bernama "pelanggan" dari database yang sedang digunakan. Dengan melakukan ini, semua data yang ada dalam tabel tersebut akan dihapus dan struktur tabelnya akan dihapus dari database.

## Kesimpulan 

Query "DROP TABLE pelanggan;" akan menghapus tabel bernama "pelanggan" dari database. Ini adalah perintah SQL yang digunakan untuk menghapus tabel beserta semua data yang terkait dengan tabel tersebut dari database. Proses ini bersifat permanen, artinya setelah tabel dihapus, data yang ada di dalamnya tidak dapat dikembalikan lagi kecuali jika backup telah dibuat sebelumnya.
