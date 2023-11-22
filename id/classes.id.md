---
title: "classes"
date : 2023-11-22
draft: true
---

# Atribut kelas HTML
Atribut kelas HTML digunakan untuk menentukan kelas untuk elemen HTML.
Beberapa elemen HTML dapat berbagi kelas yang sama.
# Menggunakan Atribut kelas
Atribut class sering digunakan untuk menunjuk ke nama kelas di style sheet. Itu juga dapat digunakan oleh JavaScript untuk mengakses dan memanipulasi elemen dengan nama kelas tertentu.
Pada contoh berikut kita memiliki tiga elemen `<div>` dengan atribut kelas dengan nilai "kota". Ketiga elemen `<div>` akan diberi gaya yang sama sesuai dengan definisi gaya .city di bagian head:
Contoh : 
``` sh
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  border: 2px solid black;
  margin: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<div class="city">
  <h2>London</h2>
  <p>London is the capital of England.</p>
</div>

<div class="city">
  <h2>Paris</h2>
  <p>Paris is the capital of France.</p>
</div>

<div class="city">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
</div>

</body>
</html>
```

Pada contoh berikut kita memiliki dua elemen `<span>` dengan atribut class dengan nilai "note". Kedua elemen `<span>` akan diberi gaya yang sama sesuai dengan definisi gaya .note di bagian head:
Contoh : 
``` sh
<!DOCTYPE html>
<html>
<head>
<style>
.note {
  font-size: 120%;
  color: red;
}
</style>
</head>
<body>

<h1>My <span class="note">Important</span> Heading</h1>
<p>This is some <span class="note">important</span> text.</p>

</body>
</html>
```

Tip: Atribut class dapat digunakan pada elemen HTML apa pun.
Catatan: Nama kelas peka huruf besar-kecil!
Tip: Anda dapat mempelajari lebih lanjut tentang CSS di Tutorial CSS kami.
# Syntax Untuk Kelas
Untuk membuat kelas; tulis karakter titik (.), diikuti dengan nama kelas. Lalu, definisikan properti CSS di dalam kurung kurawal {}:
Contoh : 
Buat kelas dengan nama "city":
``` sh
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>
</head>
<body>

<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>

</body>
</html>
```
# Beberapa Kelas
Elemen HTML dapat dimiliki lebih dari satu kelas.
Untuk mendefinisikan beberapa kelas, pisahkan nama kelas dengan spasi, mis. `<div class="kota utama">`. Elemen akan ditata sesuai dengan semua kelas yang ditentukan.
Dalam contoh berikut, elemen `<h2>` pertama milik kelas kota dan juga kelas utama, dan akan mendapatkan gaya CSS dari kedua kelas:
Contoh : 
``` sh
<h2 class="city main">London</h2>
<h2 class="city">Paris</h2>
<h2 class="city">Tokyo</h2>
```
# Elemen Berbeda Dapat Berbagi Kelas yang Sama
Elemen HTML yang berbeda dapat menunjuk ke nama kelas yang sama.
Dalam contoh berikut, `<h2>` dan `<p>` menunjuk ke kelas "kota" dan akan menggunakan gaya yang sama:
Contoh : 
``` sh
<h2 class="city">Paris</h2>
<p class="city">Paris is the capital of France</p>
```
# Penggunaan Atribut kelas dalam JavaScript
Nama kelas juga dapat digunakan oleh JavaScript untuk melakukan tugas tertentu untuk elemen tertentu.
JavaScript dapat mengakses elemen dengan nama kelas tertentu dengan metode getElementsByClassName():
Contoh : 
Klik tombol untuk menyembunyikan semua elemen dengan nama kelas "city":
``` sh
<script>
function myFunction() {
  var x = document.getElementsByClassName("city");
 for (var i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
}
</script>
```
# Ringkasan Bab
Atribut kelas HTML menentukan satu atau lebih nama kelas untuk suatu elemen
Kelas digunakan oleh CSS dan JavaScript untuk memilih dan mengakses elemen tertentu
Atribut class dapat digunakan pada elemen HTML apa pun
Nama kelas peka huruf besar-kecil
Elemen HTML yang berbeda dapat menunjuk ke nama kelas yang sama
JavaScript dapat mengakses elemen dengan nama kelas tertentu dengan metode getElementsByClassName()

