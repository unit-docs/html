---
title: Webstorage
date : 2023-09-22T10:28:51+07:00
draft: true
---

# Penyimpanan Web HTML API


Penyimpanan Web HTML; Lebih baik daripada cookies.

### Apa itu Penyimpanan Web HTML?

Dengan penyimpanan web, aplikasi web dapat menyimpan data secara lokal di dalam browser pengguna.

Sebelum HTML5, data aplikasi harus disimpan dalam cookie, disertakan dalam setiap permintaan server. Penyimpanan web lebih aman, dan data dalam jumlah besar dapat disimpan secara lokal, tanpa memengaruhi kinerja situs web.

Berbeda dengan cookie, batas penyimpanannya jauh lebih besar (setidaknya 5MB) dan informasi tidak pernah ditransfer ke server.

Penyimpanan web per asal (per domain dan protokol). Semua halaman, dari satu asal, dapat menyimpan dan mengakses data yang sama.

### Peramban Pendukung

Angka-angka dalam tabel menentukan versi browser pertama yang sepenuhnya mendukung Penyimpanan Web.

![webstorage](https://github.com/uin-unit/docs-html/blob/main/images/webstorage.png)


### Objek Penyimpanan Web HTML
Penyimpanan web HTML menyediakan dua objek untuk menyimpan data pada klien:

window.localStorage - menyimpan data tanpa tanggal kedaluwarsa

window.sessionStorage - menyimpan data untuk satu sesi (data hilang saat tab browser ditutup)

Sebelum menggunakan penyimpanan web, periksa dukungan browser untuk Penyimpanan lokal dan Penyimpanan sesi:

Contoh : 

```sh
if (typeof(Storage) !== "undefined") {
  // Code for localStorage/sessionStorage.
} else {
  // Sorry! No Web Storage support..
}
```

### Objek Penyimpanan Lokal

Objek penyimpanan lokal menyimpan data tanpa tanggal kedaluwarsa. Data tidak akan dihapus saat browser ditutup, dan akan tersedia pada hari, minggu, atau tahun berikutnya

Contoh : 
```sh
// Store
localStorage.setItem("lastname", "Smith");

// Retrieve
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
```

Penjelasan Contoh : 

Membuat penyimpanan lokal nama/pasangan nilai dengan nama=”namabelakang” dan nilai=”smith”
.ambil nilai "nama belakang" dan masukkan ke dalam elemen dengan id="hasil"

Contoh di atas bisa juga ditulis seperti ini: 
```sh
// Store
localStorage.lastname = "Smith";
// Retrieve
document.getElementById("result").innerHTML = localStorage.lastname;
```

Sintaks untuk menghapus item penyimpanan lokal "nama belakang" adalah sebagai berikut:

localStorage.removeItem("lastname");

Catatan: Pasangan nama/nilai selalu disimpan sebagai string. Ingatlah untuk mengonversinya ke format lain bila diperlukan!

Contoh berikut menghitung berapa kali pengguna mengklik sebuah tombol. Dalam kode ini string nilai diubah menjadi angka untuk dapat menambah penghitung:


Contoh : 
```sh
if (localStorage.clickcount) {
  localStorage.clickcount = Number(localStorage.clickcount) + 1;
} else {
  localStorage.clickcount = 1;
}
document.getElementById("result").innerHTML = "You have clicked the button " +
localStorage.clickcount + " time(s).";
```

### Sesi Objek Penyimpanan
Sesi objek penyimpanan sama dengan objek Penyimpanan lokal, kecuali objek tersebut menyimpan data hanya untuk satu sesi. Data dihapus ketika pengguna menutup tab browser tertentu.
Contoh berikut menghitung berapa kali pengguna mengklik tombol, dalam sesi saat ini:

```sh
Contoh : 
if (sessionStorage.clickcount) {
  sessionStorage.clickcount = Number(sessionStorage.clickcount) + 1;
} else {
  sessionStorage.clickcount = 1;
}
document.getElementById("result").innerHTML = "You have clicked the button " +
sessionStorage.clickcount + " time(s) in this session.";
```
