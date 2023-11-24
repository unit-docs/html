---
title: Atribut Formulir
date : 2023-11-22
draft: true
---

# Atribut Formulir HTML
Bab ini menjelaskan berbagai atribut yang berbeda untuk elemen HTML `<form>`.

## Atribut Tindakan

Atribut tindakan mendefinisikan tindakan yang akan dilakukan ketika formulir dikirimkan.

Biasanya, data formulir dikirim ke sebuah file di server ketika pengguna mengklik tombol kirim.

Pada contoh di bawah ini, data formulir dikirim ke file bernama "action_page.php". File ini berisi skrip sisi server yang menangani data formulir:

Contoh:

Pada saat submit, kirimkan data formulir ke "action_page.php":
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

Tips: Jika atribut tindakan dihilangkan, tindakan ditetapkan ke halaman saat ini.

## Atribut Target/Sasaran

Atribut target menentukan tempat untuk menampilkan respons yang diterima setelah mengirimkan formulir.

Atribut target dapat memiliki salah satu dari nilai berikut:

| Value | Deskripsi |
| ----------- | ----------- |
| `_blank` | Tanggapan ditampilkan di jendela atau tab baru |
| `_self` | Tanggapan ditampilkan pada jendela saat ini |
| `_parent` | Tanggapan ditampilkan dalam bingkai induk |
| `_top` | Tanggapan ditampilkan di seluruh bagian jendela |
| `framename` | Respons ditampilkan dalam sebuah iframe bernama |



Value defaultnya adalah `_self` yang berarti respons akan terbuka di jendela saat ini.

Contoh:

Di sini, hasil yang dikirimkan akan terbuka di tab browser baru:

```sh
<form action="/action_page.php" target="_blank">
```
  
## Atribut Metode

Atribut metodeAtribut Formulir HTML

Bab ini menjelaskan berbagai atribut yang berbeda untuk elemen HTML `<form>`.

## Atribut Tindakan

Atribut tindakan mendefinisikan tindakan yang akan dilakukan ketika formulir dikirimkan.

Biasanya, data formulir dikirim ke sebuah file di server ketika pengguna mengklik tombol kirim.

Pada contoh di bawah ini, data formulir dikirim ke file bernama "action_page.php". File ini berisi skrip sisi server yang menangani data formulir:

Contoh:

Pada saat submit, kirimkan data formulir ke "action_page.php":
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

Tips: Jika atribut tindakan dihilangkan, tindakan ditetapkan ke halaman saat ini.

## Atribut Pelengkapan Otomatis

Atribut pelengkapan otomatis menentukan apakah formulir harus memiliki pelengkapan otomatis aktif atau nonaktif.

Ketika pelengkapan otomatis diaktifkan, browser secara otomatis melengkapi nilai berdasarkan nilai yang telah dimasukkan pengguna sebelumnya.

Contoh formulir dengan autocomplete diaktifkan:
```sh
<form action="/action_page.php" autocomplete="on">
```

## Atribut Novalidasi/Novalidate

Atribut novalidasi adalah atribut boolean.

Jika ada, ini menentukan bahwa data formulir (input) tidak boleh divalidasi saat dikirimkan.

Contoh formulir dengan novalidate yang aktif:

```sh
<form action="/action_page.php" novalidate>
```
