---
title: Youtube
date : 2023-11-22
draft: true
---

# Video YouTube HTML

Cara termudah untuk memutar video dalam HTML adalah dengan menggunakan YouTube.

Kesulitan dengan Format Video? 

Mengonversi video ke format lain bisa jadi sulit dan memakan waktu.

Solusi yang lebih mudah adalah membiarkan YouTube memutar video di halaman web Anda.

Nomor Video YouTube

YouTube akan menampilkan id (seperti tgbNymZ7vqY), saat Anda menyimpan (atau memutar) video.

Anda dapat menggunakan id ini, dan merujuk ke video Anda dalam kode HTML.

## Memutar Video YouTube dalam HTML

Untuk memutar video Anda di halaman web, lakukan hal berikut:

Unggah videonya ke YouTube

Catat id videonya

Tentukan elemen `<iframe>` di halaman web Anda

Biarkan atribut src menunjuk ke URL video

Gunakan atribut lebar dan tinggi untuk menentukan dimensi pemutar

Tambahkan parameter lain ke URL (lihat di bawah)

Contoh :
```sh
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```

## Putar Otomatis YouTube + Bisukan

Anda dapat membiarkan video Anda mulai diputar secara otomatis saat pengguna mengunjungi laman tersebut, dengan menambahkan autoplay=1 ke URL 

YouTube. Namun, memulai video secara otomatis mengganggu pengunjung Anda!

Tambahkan mute=1 setelah autoplay=1 agar video Anda mulai diputar secara otomatis (tetapi dalam mode mute).

Contoh :
```sh
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>
```

## Daftar Putar YouTube

Daftar video yang dipisahkan koma untuk diputar (selain URL asli).

## Lingkaran YouTube

Tambahkan loop=1 agar video Anda berputar selamanya.

Nilai 0 (default): Video hanya akan diputar satu kali.

Nilai 1: Video akan berulang (selamanya).

Contoh : 
```sh
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```

## Kontrol YouTube

Tambahkan kontrol=0 untuk tidak menampilkan kontrol di pemutar video.

Nilai 0: Kontrol pemutar tidak ditampilkan.

Nilai 1 (default): Tampilan kontrol pemutar.

Contoh : 
```sh
<iframe width="420" height="315"
src="https://www.youtube.com/embed/tgbNymZ7vqY?controls=0">
</iframe>
```
