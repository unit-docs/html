---
title: Geolocation
date : 2023-09-22T10:28:51+07:00
draft: true
---

# API Geolokasi HTML

API Geolokasi HTML digunakan untuk menemukan posisi pengguna.

## Menemukan Posisi Pengguna

API Geolokasi HTML digunakan untuk mendapatkan posisi geografis pengguna.

Karena hal ini dapat membahayakan privasi, posisi ini tidak tersedia kecuali jika pengguna menyetujuinya.

Catatan: Geolokasi paling akurat untuk perangkat dengan GPS, seperti ponsel pintar.

## Dukungan Peramban

Angka-angka pada tabel menunjukkan versi peramban pertama yang sepenuhnya mendukung Geolokasi.

API : Chrome, Microsoft Edge, Firefox, Safari, Opera 

Geolokasi : 5.0-49.0 (http) 5.0 (https), 9.0,3.5, 5.0, 16.0

Catatan: Mulai Chrome 50, API Geolokasi hanya akan berfungsi pada konteks yang aman seperti HTTPS. Jika situs Anda di-host pada sumber yang tidak aman (seperti HTTP), permintaan untuk mendapatkan lokasi pengguna tidak akan berfungsi lagi.

## Menggunakan Geolokasi HTML

Metode `getCurrentPosition()` digunakan untuk mengembalikan posisi pengguna.

Contoh di bawah ini mengembalikan garis lintang dan garis bujur posisi pengguna:


Contoh : 

```sh
<script>
const x = document.getElementById("demo");


function getLocation() {
  if (navigator.geolocation) {
	navigator.geolocation.getCurrentPosition(showPosition);
  } else {
	x.innerHTML = "Geolocation is not supported by this browser.";
  }
}


function showPosition(position) {
  x.innerHTML = "Latitude: " + position.coords.latitude +
  "<br>Longitude: " + position.coords.longitude;
}
</script>
```

Contoh dijelaskan:

## Periksa apakah Geolokasi didukung

Jika didukung, jalankan metode `getCurrentPosition()`. Jika tidak, tampilkan pesan kepada pengguna

Jika metode getCurrentPosition() berhasil, ia mengembalikan objek koordinat ke fungsi yang ditentukan dalam parameter (showPosition)

Fungsi `showPosition()` menampilkan Garis Lintang dan Garis Bujur

Contoh di atas adalah skrip Geolokasi yang sangat mendasar, tanpa penanganan kesalahan.

## Menangani Kesalahan dan Penolakan

Parameter kedua dari metode `getCurrentPosition()` digunakan untuk menangani kesalahan. Ini menentukan fungsi yang akan dijalankan jika gagal mendapatkan lokasi pengguna:

Contoh : 

```sh
function showError(error) {
  switch(error.code) {
    case error.PERMISSION_DENIED:
  	x.innerHTML = "User denied the request for Geolocation."
      break;
    case error.POSITION_UNAVAILABLE:
  	x.innerHTML = "Location information is unavailable."
      break;
    case error.TIMEOUT:
  	x.innerHTML = "The request to get user location timed out."
      break;
    case error.UNKNOWN_ERROR:
      x.innerHTML = "An unknown error occurred."
      break;
  }
}
```
## Informasi spesifik lokasi

Halaman ini telah menunjukkan cara menampilkan posisi pengguna di peta.

Geolokasi juga sangat berguna untuk informasi spesifik lokasi, seperti:

## Informasi lokal terkini

Menampilkan Tempat Menarik di dekat pengguna

Navigasi belokan demi belokan (GPS)

Metode `getCurrentPosition()` - Mengembalikan Data







## Objek Geolokasi - Metode menarik lainnya

Objek Geolokasi juga memiliki metode menarik lainnya:

`watchPosition()` - Mengembalikan posisi pengguna saat ini dan terus mengembalikan posisi yang diperbarui seiring pergerakan pengguna (seperti GPS di dalam mobil).

`clearWatch()` - Menghentikan metode `watchPosition()`.

Contoh di bawah ini menunjukkan metode `watchPosition()`. Anda memerlukan perangkat GPS yang akurat untuk mengujinya (seperti ponsel cerdas):


Contoh :

```sh
<script>
const x = document.getElementById("demo");


function getLocation() {
  if (navigator.geolocation) {
	navigator.geolocation.watchPosition(showPosition);
  } else {
	x.innerHTML = "Geolocation is not supported by this browser.";
  }
}
function showPosition(position) {
  x.innerHTML = "Latitude: " + position.coords.latitude +
  "<br>Longitude: " + position.coords.longitude;
}
</script>
```
