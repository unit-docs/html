---
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---

# Atribut Input HTML ( HTML Input Attributes )

Bab ini menjelaskan atribut yang berbeda untuk elemen HTML.

## Atribut value (The value Attribute)

Atribut input menentukan nilai awal untuk bidang input:value

Contoh
Bidang input dengan nilai awal (default):

```sh
<form>
  <label for="fname">Nama depan:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Nama belakang:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```

## Atribut readonly (The readonly Attribute)

Atribut input menentukan bahwa field input bersifat read-only.readonly

Bidang input baca-saja tidak dapat dimodifikasi (namun, pengguna dapat menandainya, menyorotnya, dan menyalin teks darinya).

Nilai bidang input baca-saja akan dikirim saat mengirimkan formulir!

Contoh
Bidang input baca-saja:
```sh
<form>
  <label for="fname">Nama depan:</label><br>
  <input type="text" id="fname" name="fname" value="John" readonly><br>
  <label for="lname">Nama belakang:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```

## Atribut yang dinonaktifkan (The disabled Attribute)

Atribut input menentukan bahwa bidang input harus dinonaktifkan.disabled

Bidang input yang dinonaktifkan tidak dapat digunakan dan tidak dapat diklik.

Nilai bidang input yang dinonaktifkan tidak akan dikirim saat mengirimkan formulir!

Contoh
Bidang input yang dinonaktifkan:
```sh
<form>
  <label for="fname">Nama depan:</label><br>
  <input type="text" id="fname" name="fname" value="John" dinonaktifkan><br>
  <label for="lname">Nama belakang:</label><br>
  <input type="text" id="lname" name="lname" value="Doe">
</form>
```
## Ukuran Atribut (The size Attribute)

Atribut input menentukan lebar yang terlihat, dalam karakter, dari bidang input.size

Nilai default untuk adalah 20.size

Nota: Atribut Bekerja dengan jenis input berikut: teks, pencarian, tel, URL, email, dan kata sandi.size

Contoh
Atur lebar untuk bidang input:
```sh
<form>
  <label for="fname">Nama depan:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" size="4">
</form>
```
## Atribut maxlength (The maxlength Attribute)

Atribut input menentukan jumlah maksimum karakter yang diizinkan dalam bidang input.maxlength

Nota: Ketika a diatur, bidang input tidak akan menerima lebih dari jumlah karakter tertentu. Namun, atribut ini tidak memberikan umpan balik apa pun. Jadi, jika Anda ingin mengingatkan pengguna, Anda harus menulis kode JavaScript.maxlength

Contoh
Tetapkan panjang maksimum untuk bidang input:
```sh
<form>
  <label for="fname">Nama depan:</label><br>
  <input type="text" id="fname" name="fname" size="50"><br>
  <label for="pin">PIN:</label><br>
  <input type="text" id="pin" name="pin" maxlength="4" size="4">
</form>
```
## Atribut min dan max (The min and max Attributes)

Input dan atribut menentukan nilai minimum dan maksimum untuk bidang input.minmax

Atribut dan berfungsi dengan jenis input berikut: number, range, date, datetime-local, month, time dan week.minmax

Ujung: Gunakan atribut max dan min bersama-sama untuk membuat rentang nilai hukum.

Contoh
Tetapkan tanggal maksimal, tanggal minimum, dan rentang nilai legal:
```sh
<form>
  <label for="datemax">Masukkan tanggal sebelum 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

<label for="datemin">Masukkan tanggal setelah 01-01-2000:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>

<label for="quantity">Quantity (antara 1 dan 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
```
## Beberapa Atribut (The multiple Attribute)

Atribut input menentukan bahwa pengguna diizinkan untuk memasukkan lebih dari satu nilai dalam bidang input.multiple

Atribut berfungsi dengan jenis input berikut: email, dan file.multiple

Contoh
Kolom upload file yang menerima beberapa nilai:
```sh
<form>
  <label for="files">Pilih file:</label>
  <input type="file" id="files" name="files" multiple>
</form>
```
## Atribut pola (The pattern Attribute)

Atribut input menentukan ekspresi reguler bahwa Nilai bidang input dicentang, saat formulir dikirimkan.pattern

Atribut berfungsi dengan jenis input berikut: teks, tanggal, pencarian, url, telp, email, dan kata sandi.pattern

Ujung: Gunakan atribut judul global untuk mendeskripsikan pola guna membantu pengguna.

Ujung: Pelajari lebih lanjut tentang ekspresi reguler dalam tutorial JavaScript kami.

Contoh
Bidang input yang hanya dapat berisi tiga huruf (tidak ada angka atau khusus karakter):
```sh
<form>
  <label for="country_code">Kode negara:</label>
  <input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Kode negara tiga huruf">
</form>
```
## Atribut placeholder (The placeholder Attribute)

Atribut input menentukan petunjuk singkat yang menjelaskan nilai yang diharapkan dari bidang input (nilai sampel atau deskripsi singkat dari format yang diharapkan).placeholder

Petunjuk singkat ditampilkan di bidang input sebelum pengguna memasukkan nilai.

Atribut berfungsi dengan jenis input berikut: teks, pencarian, url, tel, email, dan kata sandi.placeholder

Contoh
Bidang input dengan teks placeholder:
```sh
<form>
  <label for="phone">Masukkan nomor telepon:</label>
  <input type="tel" id="phone" name="phone" placeholder="123-45-678" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
```
## Atribut yang diperlukan (The required Attribute)

Atribut input menentukan bahwa kolom input harus diisi sebelum mengirimkan formulir.required

Atribut berfungsi dengan jenis input berikut: teks, pencarian, url, tel, email, kata sandi, pemilih tanggal, angka, kotak centang, radio, dan file.required

Contoh
Bidang input yang diperlukan:
```sh
<form>
  <label for="nama pengguna">Nama pengguna:</label>
  <input type="text" id="username" name="username" diperlukan>
</form>
```
## Langkah Atribut (The step Attribute)

Atribut input menentukan interval nomor legal untuk bidang input.step

Contoh: jika step="3", angka hukum bisa -3, 0, 3, 6, dll.
Ujung: Atribut ini dapat digunakan bersama dengan atribut max dan min untuk membuat rentang nilai hukum.
Atribut berfungsi dengan jenis input berikut: angka, rentang, tanggal, tanggalwaktu-lokal, bulan, waktu, dan minggu.step
Contoh
Bidang input dengan interval nomor hukum tertentu:
```sh
<form>
  <label for="poin">Poin:</label>
  <input type="number" id="points" name="points" step="3">
</form>
```
Nota: Pembatasan input tidak mudah, dan JavaScript menyediakan banyak cara untuk Tambahkan input ilegal. Untuk membatasi input dengan aman, itu juga harus diperiksa oleh penerima (server)!

## Atribut fokus otomatis (The autofocus Attribute)

Atribut input menentukan bahwa Bidang input harus secara otomatis mendapatkan fokus saat halaman dimuat.autofocus

Contoh
Biarkan bidang input "Nama depan" secara otomatis mendapatkan fokus saat halaman dimuat:
```sh
<form>
  <label for="fname">Nama depan:</label><br>
  <input type="text" id="fname" name="fname" fokus otomatis><br>
  <label for="lname">Nama belakang:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```
## Tinggi dan lebar Atribut (The height and width Attributes)

Input dan atribut menentukan tinggi dan lebar `elemen.heightwidth<input type="image">`

Ujung: Selalu tentukan atribut tinggi dan lebar untuk Gambar. Jika tinggi dan lebar diatur, ruang yang diperlukan untuk gambar adalah dicadangkan saat halaman dimuat. Tanpa atribut ini, browser tidak mengetahui ukuran gambar, dan tidak dapat memesan ruang yang sesuai untuk itu. Si efeknya adalah tata letak halaman akan berubah selama pemuatan (sedangkan gambar memuat).

Contoh
Tentukan gambar sebagai tombol kirim, dengan atribut tinggi dan lebar:
```SH
<form>
  <label for="fname">Nama depan:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Nama belakang:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="gambar" src="img_submit.gif" alt="Kirim" width="48" height="48">
</form>
```
## Atribut list (The list Attribute)

Atribut input mengacu pada elemen yang berisi opsi yang telah ditentukan sebelumnya untuk elemen `<input>`.list `<datalist>`

Contoh
Elemen `<input>` dengan nilai yang telah ditentukan sebelumnya dalam <datalist>:
```SH
<form>
  <masukkan daftar="browser">
  <datalist id="browser">
    <option value="Tepi">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form>
```
## Atribut pelengkapan otomatis (The autocomplete Attribute)

Atribut input menentukan apakah formulir atau Bidang input harus mengaktifkan atau menonaktifkan pelengkapan otomatis.autocomplete

Pelengkapan otomatis memungkinkan browser memprediksi nilainya. Saat pengguna mulai Ketik bidang, browser harus menampilkan opsi untuk mengisi bidang, berdasarkan pada nilai yang diketik sebelumnya.

Atribut berfungsi dengan dan Jenis berikut: teks, pencarian, URL, tel, email, kata sandi, pemilih tanggal, rentang, dan `color.autocomplete` `<form>` `<input>`

Contoh
Formulir HTML dengan pelengkapan otomatis aktif, dan nonaktif untuk satu bidang input:
```sh
<form action="/action_page.php" pelengkapan otomatis="pada">
  <label for="fname">Nama depan:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Nama belakang:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" autocomplete="off"><br><br>
  <input type="submit" value="Kirim">
</form>
```
Ujung: Di beberapa browser, Anda mungkin perlu mengaktifkan fungsi pelengkapan otomatis agar ini berfungsi (Lihat di bawah "Preferensi" di menu browser).
