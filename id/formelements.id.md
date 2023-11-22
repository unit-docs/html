---
title: Form Elements
date : 2023-09-22T10:28:51+07:00
draft: true
---

# Elemen Formulir HTML

Bab ini menjelaskan semua elemen bentuk HTML yang berbeda.

## Elemen HTML `<form>`

Elemen HTML `<form>` dapat berisi satu atau lebih elemen formulir berikut:

- `<input>`
- `<label>`
- `<select>`
- `<textarea>`
- `<button>`
- `<fieldset>`
- `<legend>`
- `<datalist>`
- `<output>`
- `<option>`
- `<optgroup>`

Elemen `<input>`
Salah satu elemen form yang paling banyak digunakan adalah elemen `<input>`.

Elemen `<input>` dapat ditampilkan dalam beberapa cara, bergantung pada atribut type.

Contoh
```sh
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname">
```

Semua nilai yang berbeda dari atribut type dibahas dalam bab berikutnya: Tipe Input HTML.

## Elemen `<label>`

Elemen `<label>` mendefinisikan label untuk beberapa elemen formulir.

Elemen `<label>` berguna bagi pengguna pembaca layar, karena pembaca layar akan membacakan label dengan lantang saat pengguna fokus pada elemen input.

Elemen `<label>` juga membantu pengguna yang mengalami kesulitan mengklik wilayah yang sangat kecil (seperti tombol radio atau kotak centang) - karena ketika pengguna mengklik teks dalam elemen `<label>`, tombol radio/kotak centang akan dialihkan.

Atribut for pada tag `<label>` harus sama dengan atribut id pada elemen `<input>` untuk mengikat keduanya.

## Elemen `<select>`

Elemen `<select>` mendefinisikan daftar drop-down:

Contoh
```sh
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

Elemen `<option>` mendefinisikan opsi yang dapat dipilih.

Secara default, item pertama dalam daftar drop-down dipilih.

Untuk menentukan opsi yang telah dipilih sebelumnya, tambahkan atribut yang dipilih ke opsi:

Contoh
```sh
<option value="fiat" selected>Fiat</option>
```

Nilai yang Terlihat:
Gunakan atribut size untuk menentukan jumlah nilai yang terlihat:

Contoh
```sh
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

Izinkan Banyak Pilihan:
Gunakan beberapa atribut untuk memungkinkan pengguna memilih lebih dari satu nilai:

Contoh
```sh
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="4" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

## Elemen <textarea>

Elemen <textarea> mendefinisikan kolom input multi-baris (area teks):

Contoh

```sh
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```

Atribut baris menentukan jumlah baris yang terlihat dalam area teks.

Atribut cols menentukan lebar area teks yang terlihat.

Beginilah tampilan kode HTML di atas pada browser:

Kucing itu sedang bermain di taman.

Anda juga dapat menentukan ukuran area teks dengan menggunakan CSS:

Contoh
```sh
<textarea name="message" style="width:200px; height:600px;">
The cat was playing in the garden.
</textarea>
```

## Elemen `<button>`
Elemen `<button>` mendefinisikan tombol yang dapat diklik:

Contoh
```sh
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
```

Catatan: Selalu tentukan atribut type untuk elemen tombol. Browser yang berbeda mungkin menggunakan tipe default yang berbeda untuk elemen tombol.


## Elemen <fieldset> dan <legend>

Elemen `<fieldset>` digunakan untuk mengelompokkan data terkait dalam suatu formulir.

Elemen `<legend>` mendefinisikan keterangan untuk elemen `<fieldset>`.

Contoh
```sh
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

## Elemen `<datalist>`
Elemen `<datalist>` menentukan daftar opsi yang telah ditentukan sebelumnya untuk elemen `<input>`.

Pengguna akan melihat daftar drop-down dari opsi yang telah ditentukan sebelumnya saat mereka memasukkan data.

Atribut list elemen `<input>`, harus mengacu pada atribut id elemen `<datalist>`.

Contoh
```sh
<form action="/action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Edge">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form>
```

## Elemen `<output>`
Elemen `<output>` mewakili hasil penghitungan (seperti yang dilakukan oleh skrip).

Contoh

Lakukan perhitungan dan tampilkan hasilnya dalam elemen `<output>`:
```sh
<form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form>
```
