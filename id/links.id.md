---
title: "Links-HTML"
date : 2023-10-22
draft: true
---

# Tautan HTML

Tautan ditemukan di hampir semua halaman web. Tautan memungkinkan pengguna mengeklik dari halaman ke halaman.

## Tautan HTML - Hyperlink

Tautan HTML adalah hyperlink.
Anda dapat mengeklik tautan dan melompat ke dokumen lain.
Saat Anda menggerakkan mouse ke atas link, panah mouse akan berubah menjadi tangan kecil.
Tautan HTML - Syntax
Tag HTML `<a>` mendefinisikan hyperlink. Ini memiliki syntax berikut:
```sh
<a href="url">link text</a>
```
Atribut terpenting dari elemen `<a>` adalah atribut href, yang menunjukkan tujuan tautan.
Teks tautan adalah bagian yang akan terlihat oleh pembaca.
Mengklik teks tautan, akan mengirim pembaca ke alamat URL yang ditentukan.
Contoh : 

Contoh ini menunjukkan cara membuat tautan ke W3Schools.com:
```sh
<a href="https://www.w3schools.com/">Visit W3Schools.com!</a>
```
Tautan yang belum dikunjungi digarisbawahi dan berwarna biru
Tautan yang dikunjungi digarisbawahi dan berwarna ungu
Tautan aktif digarisbawahi dan berwarna merah

## Tautan HTML - Atribut target

Secara default, halaman tertaut akan ditampilkan di jendela browser saat ini. Untuk mengubahnya, Anda harus menentukan target lain untuk tautan tersebut.
Atribut `target` menentukan tempat untuk membuka dokumen tertaut.

Atribut `target` dapat memiliki salah satu nilai berikut:
- `_self -` Bawaan. Membuka dokumen di jendela/tab yang sama dengan yang diklik
- `_blank - `Membuka dokumen di jendela atau tab baru
- `_parent -` Membuka dokumen di bingkai induk
- `_top -` Membuka dokumen di seluruh isi jendela

contoh : 
Gunakan target=`"_blank"` untuk membuka dokumen yang ditautkan di jendela atau tab browser baru:
```sh
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```
## URL Absolut vs. URL Relatif

Kedua contoh di atas menggunakan URL absolut (alamat web lengkap) pada atribut href.
Tautan lokal (tautan ke halaman dalam situs web yang sama) ditentukan dengan URL relatif (tanpa bagian "https://www"):

Contoh : 
```sh
<h2>Absolute URLs</h2>
<p><a href="https://www.w3.org/">W3C</a></p>
<p><a href="https://www.google.com/">Google</a></p>
```
```sh
<h2>Relative URLs</h2>
<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>
```

## Tautan HTML - Gunakan Gambar sebagai Tautan

Untuk menggunakan gambar sebagai link, cukup masukkan tag `<img>` di dalam tag `<a>`:

Contoh : 
```sh
<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

## Tautan ke Alamat Email

Gunakan mailto: di dalam atribut href untuk membuat tautan yang membuka program email pengguna (agar mereka dapat mengirim email baru):

Contoh : 
```sh
<a href="mailto:someone@example.com">Send email</a>
```
## Tombol sebagai Tautan

Untuk menggunakan tombol HTML sebagai tautan, Anda harus menambahkan beberapa kode JavaScript.
JavaScript memungkinkan Anda menentukan apa yang terjadi pada peristiwa tertentu, seperti mengklik tombol:

Contoh : 
```sh
<button onclick="document.location='default.asp'">HTML Tutorial</button>
```
## Judul Tautan

Atribut title menentukan informasi tambahan tentang suatu elemen. Informasi ini paling sering ditampilkan sebagai teks keterangan alat saat mouse bergerak di atas elemen.

Contoh : 
```sh
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```
Lebih lanjut tentang URL Absolut dan URL Relatif

Contoh : 

Gunakan URL lengkap untuk menautkan ke halaman web:
```sh
<a href="https://www.w3schools.com/html/default.asp">HTML tutorial</a>
```
Contoh : 
Tautan ke halaman yang terletak di folder html di situs web saat ini:
```sh
<a href="/html/default.asp">HTML tutorial</a>
```
Contoh : 
Tautan ke halaman yang terletak di folder yang sama dengan halaman saat ini:
```sh
<a href="default.asp">HTML tutorial</a>
```
