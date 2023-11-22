---
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---
# Video HTML
Elemen HTML <video> digunakan untuk menampilkan video pada halaman web.

**Contoh**

Atas izin dari Big Buck Bunny:

**Elemen `<video>` HTML**

Untuk menampilkan video dalam HTML, gunakan elemen `<video>`:

**Contoh**
```sh
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```

**Bagaimana cara kerjanya**

Atribut kontrol menambahkan kontrol video, seperti putar, jeda, dan volume.
Sebaiknya selalu menyertakan atribut lebar dan tinggi. Jika tinggi dan lebar tidak ditetapkan, halaman mungkin berkedip saat video dimuat.
Elemen `<source>` memungkinkan Anda menentukan file video alternatif yang dapat dipilih oleh browser. Browser akan menggunakan format pertama yang dikenali.

Teks di antara tag `<video>` dan `<video>` hanya akan ditampilkan di browser yang tidak mendukung elemen `<video>`.

**HTML `<video>` Putar Otomatis**

Untuk memulai video secara otomatis, gunakan atribut autoplay:

**Contoh**

```sh
<video width="320" height="240" autoplay>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```

Catatan: Browser Chromium tidak mengizinkan pemutaran otomatis dalam banyak kasus. Namun, pemutaran otomatis yang dibisukan selalu diizinkan.

Tambahkan dibisukan setelah pemutaran otomatis agar video Anda mulai diputar secara otomatis (tetapi dibisukan):

Contoh :

```sh
<video width="320" height="240" autoplay muted>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```

**Dukungan Peramban**

Angka-angka dalam tabel menentukan versi browser pertama yang sepenuhnya mendukung elemen `<video>`.


