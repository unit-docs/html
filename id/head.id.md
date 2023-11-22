---
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---

# HTML - Elemen Kepala
Elemen HTML <head> adalah wadah untuk elemen berikut: <title>, <style>, <meta>, <link>, <script>, dan <base>.
## Elemen HTML <head>
Elemen <head> merupakan wadah metadata (data tentang data) dan ditempatkan di antara tag <html> dan tag <body>.
Metadata HTML adalah data tentang dokumen HTML. Metadata tidak ditampilkan.
Metadata biasanya menentukan judul dokumen, kumpulan karakter, gaya, skrip, dan
## Elemen HTML <judul>
Elemen <title> mendefinisikan judul dokumen. Judul harus berupa teks saja, dan ditampilkan di bilah judul browser atau di tab halaman.
Elemen <title> diperlukan dalam dokumen HTML!
Konten judul halaman sangat penting untuk optimasi mesin pencari (SEO)! Judul halaman digunakan oleh algoritma mesin pencari untuk menentukan urutan ketika mencantumkan halaman dalam hasil pencarian.
Elemen <judul>:
mendefinisikan judul di toolbar browser
memberikan judul untuk halaman ketika ditambahkan ke favorit
menampilkan judul halaman di hasil mesin pencari
Jadi, usahakan untuk membuat judul seakurat dan bermakna mungkin!
Dokumen HTML sederhana:
Contoh : 
```sh
<!DOCTYPE html>
<html>
<head>
  <title>A Meaningful Page Title</title>
</head>
<body>

The content of the document......

</body>
</html>
```
## Elemen HTML <gaya>
Elemen <style> digunakan untuk mendefinisikan informasi gaya untuk satu halaman HTML:
Contoh : 
```sh
<style>
  body {background-color: powderblue;}
  h1 {color: red;}
  p {color: blue;}
</style>
```
## Elemen HTML <link>
Elemen <link> mendefinisikan hubungan antara dokumen saat ini dan sumber daya eksternal.
Tag <link> paling sering digunakan untuk menautkan ke style sheet eksternal:
Contoh : 
```sh
<link rel="stylesheet" href="mystyle.css">
```
## Elemen HTML <meta>
Elemen <meta> biasanya digunakan untuk menentukan kumpulan karakter, deskripsi halaman, kata kunci, penulis dokumen, dan pengaturan area pandang.
Metadata tersebut tidak akan ditampilkan pada halaman, tetapi digunakan oleh browser (cara menampilkan konten atau memuat ulang halaman), oleh mesin pencari (kata kunci), dan layanan web lainnya.
Contoh :

Tentukan kumpulan karakter yang digunakan

`<meta charset="UTF-8">`

Tentukan kata kunci untuk mesin pencari:

`<meta name="keywords" content="HTML, CSS, JavaScript">`

Tentukan deskripsi halaman web Anda:

`<meta name="description" content="Free Web tutorials">`

Tentukan penulis halaman:

`<meta name="author" content="John Doe">`

Segarkan dokumen setiap 30 detik:

`<meta http-equiv="refresh" content="30">`

Mengatur area pandang agar situs web Anda terlihat bagus di semua perangkat:

`<meta name="viewport" content="width=device-width, initial-scale=1.0">`

Contoh tag <meta>:
Contoh
```sh
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="John Doe">
```
Mengatur Area Pandang
Area pandang adalah area halaman web yang terlihat oleh pengguna. Ukurannya berbeda-beda tergantung perangkatnya - ukurannya akan lebih kecil di ponsel dibandingkan di layar komputer.
Anda harus menyertakan elemen <meta> berikut di semua halaman web Anda:
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`

ini memberikan instruksi kepada browser tentang cara mengontrol dimensi dan penskalaan halaman.
Bagian width=device-width mengatur lebar halaman agar mengikuti lebar layar perangkat (yang bervariasi tergantung pada perangkat).
Bagian skala awal=1.0 mengatur tingkat zoom awal saat halaman pertama kali dimuat oleh browser.
Berikut adalah contoh halaman web tanpa meta tag viewport, dan halaman web yang sama dengan meta tag viewport:
## Elemen <script> HTML
Elemen <base> menentukan URL dasar dan/atau target untuk semua URL relatif di halaman.
Tag <base> harus memiliki atribut href atau target, atau keduanya.
Hanya ada satu elemen <base> dalam sebuah dokumen!
Contoh :
### Tentukan URL default dan target default untuk semua tautan pada halaman:
```sh
<head>
<base href="https://www.w3schools.com/" target="_blank">
</head>
<body>
<img src="images/stickman.gif" width="24" height="39" alt="Stickman">
<a href="tags/tag_base.asp">HTML base Tag</a>
</body>
```
## Ringkasan Bab
Elemen <head> merupakan wadah untuk metadata (data tentang data)
Elemen <head> ditempatkan di antara tag <html> dan tag <body>
Elemen <title> diperlukan dan mendefinisikan judul dokumen
Elemen <style> digunakan untuk mendefinisikan informasi gaya untuk satu dokumen
Tag <link> paling sering digunakan untuk menghubungkan ke style sheet eksternal
Elemen <meta> biasanya digunakan untuk menentukan rangkaian karakter, deskripsi halaman, kata kunci, penulis dokumen, dan pengaturan area pandang
Elemen <script> digunakan untuk mendefinisikan JavaScript sisi klien
Elemen <base> menentukan URL dasar dan/atau target untuk semua URL relatif di halaman
Elemen kepala HTML
## Deskripsi Tag
<head> Mendefinisikan informasi tentang dokumen
<title> Mendefinisikan judul dokumen
<base> Mendefinisikan alamat default atau target default untuk semua link pada halaman
<link> Mendefinisikan hubungan antara dokumen dan sumber daya eksternal
<meta> Mendefinisikan metadata tentang dokumen HTML
<script> Mendefinisikan skrip sisi klien
<style> Mendefinisikan informasi gaya untuk suatu dokumen
