---
title: CSS
date : 2023-11-22
draft: true
---

# GAYA HTML – CSS
CSS adalah singkatan dari Cascading Style Sheet.

CSS menghemat banyak pekerjaan. Itu dapat mengontrol tata letak beberapa halaman web sekaligus.
![alt text](https://github.com/uin-unit/docs-html/blob/main/images/CSS.png)
## Apa itu CSS?
Cascading Style Sheets (CSS) digunakan untuk memformat tata letak halaman web.

Dengan CSS, Anda dapat mengontrol warna, font, ukuran teks, jarak antar elemen, bagaimana elemen diposisikan dan ditata, gambar latar belakang atau warna latar belakang apa yang akan digunakan, tampilan berbeda untuk perangkat dan ukuran layar berbeda, dan lebih banyak!
## Menggunakan CSS
CSS dapat ditambahkan ke dokumen HTML dengan 3 cara:
- Inline - by using the style attribute inside HTML elements
- Internal - by using a `<style>` element in the <head> section
- External - by using a `<link>` element to link to an external CSS file
Cara paling umum untuk menambahkan CSS adalah dengan menyimpan gaya di file CSS eksternal. Namun, dalam tutorial ini kita akan menggunakan gaya inline dan internal, karena ini lebih mudah untuk didemonstrasikan, dan lebih mudah bagi Anda untuk mencobanya sendiri.
### CSS sebaris
CSS sebaris digunakan untuk menerapkan gaya unik ke satu elemen HTML.
CSS sebaris menggunakan styleatribut elemen HTML.
Contoh berikut mengatur warna teks elemen `<h1>` menjadi biru, dan warna teks `<p>` elemen menjadi merah:
Contoh : 
```sh
<h1 style="color:blue;">A Blue Heading</h1>
```
```sh
<p style="color:red;">A red paragraph.</p>
```
## Internal CSS
CSS internal digunakan untuk menentukan gaya untuk satu halaman HTML.
CSS internal didefinisikan di `<head>` bagian halaman HTML, di dalam sebuah `<style>` elemen.
Contoh berikut mengatur warna teks SEMUA `<h1>` elemen (di halaman itu) menjadi biru, dan warna teks SEMUA elemen `<p>` menjadi merah. Selain itu, halaman akan ditampilkan dengan warna latar belakang "biru bubuk": 
Contoh : 
```sh
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
## CSS eksternal
Lembar gaya eksternal digunakan untuk menentukan gaya pada banyak halaman HTML.
Untuk menggunakan style sheet eksternal, tambahkan link ke dalamnya di bagian `<head>` pada setiap halaman HTML:
Contoh : 
```sh
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
Style sheet eksternal dapat ditulis di editor teks apa pun. File tidak boleh berisi kode HTML apa pun, dan harus disimpan dengan ekstensi .css.
Berikut tampilan file "styles.css":
"styles.css":
```sh
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
```
## Warna, Font, dan Ukuran CSS
Di sini, kami akan mendemonstrasikan beberapa properti CSS yang umum digunakan. Anda akan mempelajari lebih lanjut tentang mereka nanti.
Properti warna CSS mendefinisikan warna teks yang akan digunakan.
Properti font-family CSS mendefinisikan font yang akan digunakan.
Properti ukuran font CSS menentukan ukuran teks yang akan digunakan.
Contoh : 
Gunakan  CSS `color`, `font-family` and `font-size` properti:
```sh
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: blue;
  font-family: verdana;
  font-size: 300%;
}
p {
  color: red;
  font-family: courier;
  font-size: 160%;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
## Border CSS
Properti perbatasan CSS mendefinisikan batas di sekitar elemen HTML.
Tip: Anda dapat menentukan batas untuk hampir semua elemen HTML.
Contoh : 
Gunakan of CSS `border` properti: 
```sh
p {
  border: 2px solid powderblue;
}
```
## Padding CSS
Properti padding CSS mendefinisikan padding (spasi) antara teks dan batas.
Contoh : 
Gunakan CSS `border` and `padding` properti:
```sh
p {
  border: 2px solid powderblue;
  padding: 30px;
}
```
## Margin CSS
Properti margin CSS mendefinisikan margin (spasi) di luar batas.
Contoh : 
Use of CSS `border` and `margin` properties:
```sh
p {
  border: 2px solid powderblue;
  margin: 50px;
}
```
## Tautan ke CSS Eksternal
Style sheet eksternal dapat direferensikan dengan URL lengkap atau dengan jalur yang berhubungan dengan halaman web saat ini.
Contoh : 
Contoh ini menggunakan URL lengkap untuk menautkan ke lembar gaya:
```sh
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```
Contoh : 
Contoh ini menautkan ke lembar gaya yang terletak di folder html di situs web saat ini:
```sh
<link rel="stylesheet" href="/html/styles.css">
```
Contoh : 
Contoh ini menautkan ke lembar gaya yang terletak di folder yang sama dengan halaman saat ini:
```sh
<link rel="stylesheet" href="styles.css">
```
### Ringkasan Bab
Gunakan atribut gaya HTML untuk penataan gaya sebaris
Gunakan elemen HTML `<style>` untuk mendefinisikan CSS internal
Gunakan elemen HTML `<link>` untuk merujuk ke file CSS eksternal
Gunakan elemen HTML `<head>` untuk menyimpan elemen `<style>` dan `<link>`
Gunakan properti warna CSS untuk warna teks
Gunakan properti font-family CSS untuk font teks
Gunakan properti ukuran font CSS untuk ukuran teks
Gunakan properti perbatasan CSS untuk batas
Gunakan properti padding CSS untuk ruang di dalam perbatasan
Gunakan properti margin CSS untuk ruang di luar batas
