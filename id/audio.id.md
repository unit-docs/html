---
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---

## Audio HTML
Elemen HTML `<audio>` digunakan untuk memutar file audio di halaman web.

## Elemen HTML <audio>

Untuk memutar file audio dalam HTML, gunakan <audio>elemen:

Contoh :

```sh
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```

Audio HTML - Cara Kerjanya

Atribut tersebut controlsmenambahkan kontrol audio, seperti putar, jeda, dan volume.

Elemen ini <source>memungkinkan Anda menentukan file audio alternatif yang dapat dipilih oleh browser. Browser akan menggunakan format pertama yang dikenali.

Teks di antara tag <audio>dan </audio>hanya akan ditampilkan di browser yang tidak mendukung <audio>elemen tersebut.

HTML <audio> Putar otomatis

Untuk memulai file audio secara otomatis, gunakan autoplayatribut:


Contoh :
```sh
<audio controls autoplay>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```
Catatan: Browser Chromium tidak mengizinkan putar otomatis dalam banyak kasus. Namun, putar otomatis tanpa suara selalu diperbolehkan.

Tambahkan mutedsetelahnya autoplayagar file audio Anda mulai diputar secara otomatis (tetapi dibisukan):


Contoh :
```sh
<audio controls autoplay muted>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```
Dukungan Peramban

Angka-angka dalam tabel menentukan versi browser pertama yang sepenuhnya mendukung <audio>elemen tersebut.
## Dukungan Peramban

Angka-angka dalam tabel menentukan versi browser pertama yang sepenuhnya mendukung <audio>elemen tersebut.

