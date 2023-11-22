---
title: Favicon
date : 2023-11-22T10:28:51+07:00
draft: true
---

# Favikon HTML
Favicon adalah gambar kecil yang ditampilkan di sebelah judul halaman di tab browser.

### Cara Menambahkan Favicon di HTML

Anda dapat menggunakan gambar apa pun yang Anda suka sebagai favicon Anda. Anda juga dapat membuat favicon sendiri di situs seperti https://www.favicon.cc.

Tip: Favicon adalah gambar kecil, jadi sebaiknya gambar sederhana dengan kontras tinggi.

Gambar favicon ditampilkan di sebelah kiri judul halaman di tab browser, seperti ini:

 ![favicon](https://github.com/uin-unit/docs-html/blob/main/images/favicon1.png)

Untuk menambahkan favicon ke situs web Anda, simpan gambar favicon Anda ke direktori akar server web Anda, atau buat folder di direktori akar bernama gambar, dan simpan gambar favicon Anda di folder ini. Nama umum untuk gambar favicon adalah "favicon.ico".

Selanjutnya, tambahkan elemen `<link>` ke file "index.html" Anda, setelah elemen `<title>`, seperti ini:
Contoh : 

```sh
<!DOCTYPE html>
<html>
<head>
  <title>My Page Title</title>
  <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
Sekarang, simpan file "index.html" dan muat ulang di browser Anda. Tab browser Anda sekarang akan menampilkan gambar favicon Anda di sebelah kiri judul halaman.

Dukungan Format File Favicon

Tabel berikut menunjukkan dukungan format file untuk gambar favicon:

 ![favicon](https://github.com/uin-unit/docs-html/blob/main/images/favicon2.png)

### Ringkasan Bab

Gunakan elemen HTML <link> untuk menyisipkan favicon
