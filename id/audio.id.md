---
title: Audio
date : 2023-11-22
draft: true
---

# Audio HTML
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

![audio1](https://github.com/uin-unit/docs-html/blob/main/images/audio1.png)

## Format Audio HTML

Ada tiga format audio yang didukung: MP3, WAV, dan OGG. Dukungan browser untuk berbagai format adalah: 

| Browser	 | MP3 | WAV | OGG |
| ----------- | ----------- |----------- |----------- |
| Edge/IE	 | YES | YES*| YES*|
| Chrome | YES | YES | YES |
| Firefox | YES | YES | YES |
| Safari | YES | YES | NO |
| Opera	 | YES | YES | YES |

*Dari Tepi 79

## Audio HTML - Jenis Media

| File Format	 | Media Type |
| ----------- | ----------- |
| MP3 | audio/mpeg |
| OGG	 | audio/ogg |
| WAV | audio/wav |

## Audio HTML - Metode, Properti, dan Acara

HTML DOM mendefinisikan metode, properti, dan peristiwa untuk <audio>elemen.

Ini memungkinkan Anda memuat, memutar, dan menjeda audio, serta mengatur durasi dan volume.

Ada juga peristiwa DOM yang dapat memberi tahu Anda saat audio mulai diputar, dijeda, dll.

Untuk referensi DOM lengkap, buka Referensi DOM Audio/Video HTML kami .

## Tandai HTML Audio

| Tag	 | Deskripsi |
| ----------- | ----------- |
| `<audio>` |Mendefinisikan konten suara |
| `<source>`	 | Mendefinisikan beberapa sumber daya media untuk elemen media, seperti <video> dan <audio> |
