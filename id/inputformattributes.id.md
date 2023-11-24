---
title: Input From Attribute
date : 2023-11-22
draft: true
---

# Formulir Input HTML* Atribut (HTML Input form* Attributes)

Bab ini menjelaskan atribut yang berbeda untuk elemen HTML. form* `<input>`


## Bentuk Atribut (The form Attribute)

Atribut input menentukan formulir elemen milik.form `<input>`

Nilai atribut ini harus sama dengan atribut id dari <form> elemen miliknya.

Contoh
Bidang input yang terletak di luar formulir HTML (tetapi masih merupakan bagian dari formulir):
```sh
<form action="/action_page.php" id="form1">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
</form>

<label for="lname">Last name:</label>
<input type="text" id="lname" name="lname" form="form1">
```
## Atribut formaction (The formaction Attribute)

Atribut input menentukan URL File yang akan memproses input saat formulir dikirimkan.formaction

Nota: Atribut ini menimpa atribut elemen. action `<form>`

Atribut berfungsi dengan Jenis input berikut: Kirim dan gambar.formaction

Contoh
Formulir HTML dengan dua tombol kirim, dengan tindakan berbeda:
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formaction="/action_page2.php" value="Submit as Admin">
</form>
```
## Atribut formenctype (The formenctype Attribute)

Atribut input menentukan bagaimana form-data harus dikodekan saat dikirimkan (hanya untuk formulir dengan method="post").formenctype

Nota: Atribut ini menimpa atribut enctype elemen. `<form>`

Atribut berfungsi dengan Jenis input berikut: Kirim dan gambar.formenctype

Contoh
Formulir dengan dua tombol kirim. Yang pertama mengirimkan data-formulir dengan pengkodean default, Yang kedua mengirimkan form-data yang dikodekan sebagai "multipart/form-data":
```sh
<form action="/action_page_binary.asp" method="post">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formenctype="multipart/form-data"
  value="Submit as Multipart/form-data">
</form>
```
## Atribut formmethod (The formmethod Attribute)

Atribut input mendefinisikan metode HTTP untuk mengirim form-data ke URL tindakan.formmethod

Nota: Atribut ini menimpa atribut method elemen.<form>

Atribut berfungsi dengan Jenis input berikut: Kirim dan gambar.formmethod

Data-formulir dapat dikirim sebagai variabel URL (method="get") atau sebagai posting HTTP transaksi (method="post").

Catatan tentang metode "dapatkan":

Metode ini menambahkan data formulir ke URL dalam pasangan nama/nilai

Metode ini berguna untuk pengiriman formulir di mana pengguna ingin bookmark Hasilnya

Ada batasan berapa banyak data yang dapat Anda tempatkan di URL (bervariasi antara browser), oleh karena itu, Anda tidak dapat memastikan bahwa semua data-formulir akan Ditransfer dengan benar

Jangan pernah menggunakan metode "dapatkan" untuk menyampaikan informasi sensitif! (kata sandi atau Informasi sensitif lainnya akan terlihat di bilah alamat browser)

Catatan tentang metode "posting":

Metode ini mengirimkan form-data sebagai transaksi posting HTTP

Pengiriman formulir dengan metode "posting" tidak dapat ditandai

Metode "post" lebih kuat dan aman daripada "get", dan "post" melakukannya tidak memiliki batasan ukuran

Contoh
Formulir dengan dua tombol kirim. Yang pertama mengirimkan data-formulir dengan method="dapatkan". Yang kedua mengirimkan form-data dengan method="post":
```sh
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit using GET">
  <input type="submit" formmethod="post" value="Submit using POST">
</form>
```
## Atribut formtarget (The formtarget Attribute)

Atribut input menentukan nama atau kata kunci yang menunjukkan di mana untuk menampilkan respons yang diterima setelah mengirimkan formulir.formtarget

Nota: Atribut ini menimpa atribut target elemen.<form>

Atribut berfungsi dengan Jenis input berikut: Kirim dan gambar.formtarget

Contoh
Formulir dengan dua tombol kirim, dengan jendela target yang berbeda:
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formtarget="_blank" value="Submit to a new window/tab">
</form>
```
## Atribut formnovalidate (The formnovalidate Attribute)

Atribut input menentukan bahwa elemen <input> tidak boleh divalidasi saat dikirimkan.formnovalidate

Nota: Atribut ini menimpa atribut novalidate elemen.<form>

Atribut berfungsi dengan Jenis input berikut: Kirim.formnovalidate

Contoh
Formulir dengan dua tombol kirim (dengan dan tanpa validasi):
```sh
<form action="/action_page.php">
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="Submit">
  <input type="submit" formnovalidate="formnovalidate"
  value="Submit without validation">
</form>
```
## Atribut novalidate (The novalidate Attribute)

Atribut adalah atribut.novalidate<form>

Saat ada, novalidate menentukan bahwa semua data formulir tidak boleh divalidasi saat dikirimkan.

Contoh
Tentukan bahwa tidak ada data formulir yang harus divalidasi saat mengirimkan:
```sh
<form action="/action_page.php" novalidate>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="Submit">
</form>
```
