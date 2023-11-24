---
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---

# Gambar HTML
Gambar dapat meningkatkan desain dan tampilan halaman web.

Contoh :
```sh
<img src="pic_trulli.jpg" alt="Italian Trulli">
```
Contoh : 
```sh
<img src="img_girl.jpg" alt="Girl in a jacket">
```
Contoh : 
```sh
<img src="img_chania.jpg" alt="Flowers in Chania">
```
## Syntax Gambar HTML

Tag HTML `<img>` digunakan untuk menyematkan gambar di halaman web.


Gambar secara teknis tidak dimasukkan ke dalam halaman web; gambar ditautkan ke halaman web. Tag `<img>` membuat ruang tunggu untuk gambar yang direferensikan.

Tag `<img>` kosong, hanya berisi atribut, dan tidak memiliki tag penutup.

Tag `<img>` memiliki dua atribut yang diperlukan:

- src - Menentukan jalur ke gambar

- alt - Menentukan teks alternatif untuk gambar

## Syntax
```sh
<img src="url" alt="alternatetext">
```
## Atribut src

Atribut src yang diperlukan menentukan jalur (URL) ke gambar.

Catatan: Saat halaman web dimuat, pada saat itulah browserlah yang mengambil gambar dari server web dan menyisipkannya ke halaman. Oleh 
karena itu, pastikan gambar tersebut benar-benar tetap berada di tempat yang sama dengan halaman web, jika tidak pengunjung Anda akan mendapatkan ikon tautan rusak. Ikon tautan rusak dan teks alt ditampilkan jika browser tidak dapat menemukan gambar.

Contoh : 
```sh
<img src="img_chania.jpg" alt="Flowers in Chania">
```
Atribut alt

Atribut alt yang diperlukan menyediakan teks alternatif untuk gambar, jika pengguna karena alasan tertentu tidak dapat melihatnya (karena koneksi lambat, kesalahan pada atribut src, atau jika pengguna menggunakan pembaca layar).

Nilai atribut alt harus mendeskripsikan gambar:

Contoh : 
```sh
<img src="img_chania.jpg" alt="Flowers in Chania">
```
Jika browser tidak dapat menemukan gambar, maka akan menampilkan nilai atribut alt:

Contoh : 
```sh
<img src="wrongname.gif" alt="Flowers in Chania">
```
## Ukuran Gambar - Lebar dan Tinggi

Anda dapat menggunakan atribut style untuk menentukan lebar dan tinggi gambar.

Contoh : 
```sh
<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
```
Alternatifnya, Anda dapat menggunakan atribut lebar dan tinggi:

Contoh : 
```sh
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```
Atribut lebar dan tinggi selalu menentukan lebar dan tinggi gambar dalam piksel.

## Lebar dan Tinggi, atau Gaya?

Atribut lebar, tinggi, dan gaya semuanya valid dalam HTML.
Namun, kami menyarankan untuk menggunakan atribut style. Ini mencegah style sheet mengubah ukuran gambar:

Contoh : 
```sh
<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 100%;
}
</style>
</head>
<body>

<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">

<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">

</body>
</html>
```

## Gambar di Folder Lain

Jika Anda memiliki gambar di sub-folder, Anda harus menyertakan nama folder di atribut src:

Contoh : 
```sh
<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
```
## Gambar di Server/Situs Lain

Beberapa situs web menunjuk ke gambar di server lain.
Untuk menunjuk ke gambar di server lain, Anda harus menentukan URL absolut (lengkap) di atribut src:

Contoh : 
```sh
<img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
```
## Gambar Animasi

HTML memungkinkan GIF animasi:

Contoh : 
```sh
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
```
Gambar sebagai Tautan
Untuk menggunakan gambar sebagai link, letakkan tag `<img>` di dalam tag `<a>`:

Contoh : 
```sh
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```
## Gambar Mengambang

Gunakan properti float CSS untuk membiarkan gambar melayang ke kanan atau ke kiri teks:

Contoh : 
```sh
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</p>
```
```sh
<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</p>
```

Format Gambar Umum

Berikut adalah jenis file gambar yang paling umum, yang didukung di semua browser (Chrome, Edge, Firefox, Safari, Opera):

## Ekstensi File Format File Singkatan

Grafik Jaringan Portabel Animasi APNG .apng

Format Pertukaran Grafik GIF .gif

ICO Ikon Microsoft .ico, .cur

Gambar Kelompok Pakar Fotografi Gabungan JPEG .jpg, .jpeg, .jfif, .pjpeg, .pjp

Grafik Jaringan Portabel PNG .png

Grafik Vektor Skalabel SVG .svg
## Ringkasan Bab

Gunakan elemen HTML <img> untuk mendefinisikan gambar

Gunakan atribut HTML src untuk menentukan URL gambar

Gunakan atribut alt HTML untuk menentukan teks alternatif untuk gambar, jika tidak dapat ditampilkan

Gunakan atribut lebar dan tinggi HTML atau properti lebar dan tinggi CSS untuk menentukan ukuran gambar

Gunakan properti float CSS untuk membiarkan gambar melayang ke kiri atau ke kanan

# Peta Gambar HTML

Dengan peta gambar HTML, Anda dapat membuat area yang dapat diklik pada gambar.


## Peta Gambar

Tag HTML `<map>` mendefinisikan peta gambar. Peta gambar adalah gambar dengan area yang dapat diklik. Area ditentukan dengan satu atau lebih tag `<area>`.

Coba klik pada komputer, ponsel, atau secangkir kopi pada gambar di bawah ini:

Contoh : 
Here is the HTML source code for the image map above:
```sh
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm">
</map>
```
## Bagaimana cara kerjanya?

Ide dibalik peta gambar adalah Anda dapat melakukan tindakan yang berbeda-beda tergantung pada bagian gambar yang Anda klik.

Untuk membuat peta gambar, Anda memerlukan gambar, dan beberapa kode HTML yang menjelaskan area yang dapat diklik

## Foto

Gambar disisipkan menggunakan tag <img>. Satu-satunya perbedaan dari gambar lain adalah Anda harus menambahkan atribut usemap:
```sh
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">
```
Nilai usemap dimulai dengan tag hash # diikuti dengan nama peta gambar, dan digunakan untuk membuat hubungan antara gambar dan peta gambar.

## Buat Peta Gambar

Kemudian, tambahkan elemen `<map>`.
Elemen `<map>` digunakan untuk membuat peta gambar, dan ditautkan ke gambar dengan menggunakan atribut nama yang diperlukan:
```sh
<map name="workmap">
```
## Area

Kemudian, tambahkan area yang dapat diklik.

Area yang dapat diklik ditentukan menggunakan elemen `<area>`.

## bentuk

Anda harus menentukan bentuk area yang dapat diklik, dan Anda dapat memilih salah satu dari nilai berikut:

- rect - mendefinisikan wilayah persegi panjang

- lingkaran - mendefinisikan wilayah melingkar

- poli - mendefinisikan wilayah poligonal

- default - mendefinisikan seluruh wilayah

Anda juga harus menentukan beberapa koordinat untuk dapat menempatkan area yang dapat diklik pada gambar.

## Bentuk = "lurus"

Koordinat untuk bentuk = "persegi" berpasangan, satu untuk sumbu x dan satu lagi untuk sumbu y.

Jadi, koordinat 34,44 terletak 34 piksel dari margin kiri dan 44 piksel dari atas:

Koordinat 270.350 terletak 270 piksel dari margin kiri dan 350 piksel dari atas:

Sekarang kita memiliki cukup data untuk membuat area persegi panjang yang dapat diklik:

Contoh : 
```sh
<area shape="rect" coords="34, 44, 270, 350" href="computer.htm">
```

ni adalah area yang dapat diklik dan akan mengirim pengguna ke halaman "computer.htm"
## bentuk = "lingkaran"

Untuk menambah luas lingkaran, cari dulu koordinat pusat lingkarannya:
337.300

Kemudian tentukan jari-jari lingkaran:
44 piksel


Sekarang Anda memiliki cukup data untuk membuat area melingkar yang dapat diklik:
Contoh : 
```sh
<area shape="circle" coords="337, 300, 44" href="coffee.htm">
```

Ini adalah area yang dapat diklik dan akan mengarahkan pengguna ke halaman "coffee.htm

## Bentuk = "poli"

Bentuk = "poli" berisi beberapa titik koordinat, yang menghasilkan bentuk yang dibentuk dengan garis lurus (poligon).
Ini dapat digunakan untuk membuat bentuk apa pun.

Mungkin seperti bentuk croissant!

Bagaimana kita membuat croissant pada gambar di bawah ini menjadi link yang dapat diklik?

Kita harus mencari koordinat x dan y untuk semua sisi croissant:

Koordinatnya berpasangan, satu untuk sumbu x dan satu lagi untuk sumbu y:
Contoh : 
```sh
<area shape="poly" coords="140,121,181,116,204,160,204,222,191,270,140,329,85,355,58,352,37,322,40,259,103,161,128,147" href="croissant.htm">
```
Ini adalah area yang dapat diklik dan akan mengarahkan pengguna ke halaman "croissant.htm":

## Peta Gambar dan JavaScript

Area yang dapat diklik juga dapat memicu fungsi JavaScript.

Tambahkan event click ke elemen <area> untuk menjalankan fungsi JavaScript:
Contoh : 
Di sini, kita menggunakan atribut onclick untuk menjalankan fungsi JavaScript ketika area diklik:
```sh
<map name="workmap">
  <area shape="circle" coords="337,300,44" href="coffee.htm" onclick="myFunction()">
</map>

<script>
function myFunction() {
  alert("You clicked the coffee cup!");
}
</script>
```
## Ringkasan Bab

Gunakan elemen HTML `<map>` untuk mendefinisikan peta gambar

Gunakan elemen HTML `<area>` untuk menentukan area yang dapat diklik di peta gambar

Gunakan atribut usemap HTML dari elemen `<img>` untuk menunjuk ke peta gambar

# Gambar Latar Belakang HTML

Gambar latar belakang dapat ditentukan untuk hampir semua elemen HTML.


## Gambar Latar Belakang pada elemen HTML

Untuk menambahkan gambar latar belakang pada elemen HTML, gunakan atribut style HTML dan properti CSS background-image :
Contoh : 
Menambahkan gambar latar belakang pada elemen HTML:
```sh
<p style="background-image: url('img_girl.jpg');">
```
  Anda juga dapat menentukan gambar latar belakang di elemen `<style>`, di bagian `<head>`:
Contoh : 
Tentukan gambar latar belakang di elemen `<style>`:
```sh
<style>
p {
  background-image: url('img_girl.jpg');
}
</style>
```

## Gambar Latar Belakang pada Halaman
Jika Anda ingin seluruh halaman memiliki gambar latar belakang, Anda harus menentukan gambar latar belakang pada elemen `<body>`:
Contoh : 
Menambahkan gambar latar belakang untuk seluruh halaman:
```sh
<style>
body {
  background-image: url('img_girl.jpg');
}
</style>
```
## Ulangi Latar Belakang
Jika gambar latar belakang lebih kecil dari elemennya, gambar tersebut akan berulang secara horizontal dan vertikal hingga mencapai akhir elemen:

Contoh : 
```sh
<style>
body {
  background-image: url('example_img_girl.jpg');
}
</style>
```
Untuk menghindari gambar latar belakang terulang, atur properti background-repeat menjadi no-repeat.

Contoh : 
```sh
<style>
body {
  background-image: url('example_img_girl.jpg');
  background-repeat: no-repeat;
}
</style>
```
## Sampul Latar Belakang

Jika Anda ingin gambar latar belakang menutupi seluruh elemen, Anda dapat mengatur properti background-size menjadi cover.

Selain itu, untuk memastikan seluruh elemen selalu tertutup, atur properti background-attachment menjadi fixed:

Dengan cara ini, gambar latar belakang akan menutupi seluruh elemen, tanpa peregangan (gambar akan mempertahankan proporsi aslinya):

Contoh : 
```sh
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>
```
## Peregangan Latar Belakang

Jika Anda ingin gambar latar belakang diregangkan agar sesuai dengan seluruh elemen, Anda dapat mengatur properti ukuran latar belakang menjadi 100% 100%:

Coba ubah ukuran jendela browser, dan Anda akan melihat bahwa gambar akan melebar, tetapi selalu menutupi seluruh elemen.

Contoh : 
```sh
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
}
</style>
```

Pelajari Lebih Lanjut CSS

Dari contoh di atas Anda telah belajar bahwa gambar latar belakang dapat ditata dengan menggunakan properti latar belakang CSS.

Untuk mempelajari lebih lanjut tentang properti latar belakang CSS, pelajari Tutorial Latar Belakang CSS kami.

# Elemen `<gambar>` HTML

Elemen HTML `<picture>` memungkinkan Anda menampilkan gambar berbeda untuk perangkat atau ukuran layar berbeda.

## Elemen HTML `<gambar>`

Elemen HTML `<picture>` memberi pengembang web lebih banyak fleksibilitas dalam menentukan sumber daya gambar.

Elemen `<picture>` berisi satu atau lebih elemen `<source>`, masing-masing merujuk ke gambar berbeda melalui atribut srcset. Dengan cara ini browser dapat memilih gambar yang paling sesuai dengan tampilan dan/atau perangkat saat ini.

Setiap elemen `<source>` memiliki atribut media yang menentukan kapan gambar paling cocok.

Contoh : 
Menampilkan gambar yang berbeda untuk ukuran layar yang berbeda:
```sh
<picture>
  <source media="(min-width: 650px)" srcset="img_food.jpg">
  <source media="(min-width: 465px)" srcset="img_car.jpg">
  <img src="img_girl.jpg">
</picture>
```
## Kapan menggunakan Elemen Gambar

Ada dua tujuan utama elemen `<picture>`:


1. Bandwidth

Jika Anda memiliki layar atau perangkat kecil, tidak perlu memuat file gambar berukuran besar. Browser akan menggunakan elemen <source> pertama dengan nilai atribut yang cocok, dan mengabaikan elemen berikut.


2. Dukungan Format

Beberapa browser atau perangkat mungkin tidak mendukung semua format gambar. Dengan menggunakan elemen <picture>, Anda dapat menambahkan gambar dalam semua format, dan browser akan menggunakan format pertama yang dikenalinya, dan mengabaikan salah satu elemen berikut.

Contoh : 
Browser akan menggunakan format gambar pertama yang dikenali:
```sh
<picture>
  <source srcset="img_avatar.png">
  <source srcset="img_girl.jpg">
  <img src="img_beatles.gif" alt="Beatles" style="width:auto;">
</picture>
```
