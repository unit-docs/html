---
title: Formulir
date : 2023-09-22T10:28:51+07:00
draft: true
---

# Formulir HTML

Formulir HTML digunakan untuk mengumpulkan masukan dari pengguna. Masukan dari pengguna paling sering dikirim ke server untuk diproses.

### Elemen `<form>`

Elemen HTML `<form>` digunakan untuk membuat formulir HTML untuk input pengguna:

```sh
<form>

form elements

</form>
```

Elemen `<form>` adalah wadah untuk berbagai jenis elemen input, seperti: bidang teks, kotak centang, tombol radio, tombol kirim, dll.

Semua elemen formulir yang berbeda dibahas dalam bab ini: Elemen Formulir HTML.

### Elemen `<input>`

HTML `<input>` adalah elemen bentuk yang paling sering digunakan.

Elemen `<input>` dapat ditampilkan dengan berbagai cara, tergantung pada atribut jenisnya.
Berikut contohnya:

| Tipe | Deskripsi |
| ----------------------- | -------------------------- |
| `<input type="text">` | Menampilkan bidang input teks satu baris |
| `<input type="radio">` | Menampilkan tombol radio (untuk memilih salah satu dari sekian banyak pilihan) |
| `<input type="checkbox">` | Menampilkan kotak centang (untuk memilih nol atau lebih dari sekian banyak pilihan) |
| `<input type="submit">` | Menampilkan tombol kirim (untuk mengirimkan formulir) |
| `<input type="button">` | Menampilkan tombol yang bisa diklik |


Semua jenis input yang berbeda dibahas dalam bab ini: Jenis Masukan HTML.

### Bidang Teks

`<input type="text">` mendefinisikan bidang input satu baris untuk input teks.

Contohnya:

Formulir dengan kolom input untuk teks:
```sh
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

Beginilah cara kode HTML di atas akan ditampilkan di browser:
```sh
First name:

Last name:
```

Catatan: Formulir itu sendiri tidak terlihat. Perhatikan juga bahwa lebar default bidang input adalah 20 karakter.

Elemen `<label>`

Perhatikan penggunaan elemen `<label>` pada contoh di atas.

Tag `<label>` mendefinisikan label untuk banyak elemen formulir.

Elemen `<label>` berguna bagi pengguna pembaca layar, karena pembaca layar akan membacakan label dengan lantang ketika pengguna fokus pada elemen input.


Elemen `<label>` juga membantu pengguna yang mengalami kesulitan untuk mengeklik bagian yang sangat kecil (seperti tombol radio atau kotak centang) - karena ketika pengguna mengeklik teks di dalam elemen `<label>`, maka ia akan mengalihkan tombol radio/kotak centang.

Atribut for pada tag `<label>` harus sama dengan atribut id pada elemen `<input>` untuk mengikat keduanya.

Tombol Radio
`<input type="radio">` mendefinisikan tombol radio.

Tombol radio memungkinkan pengguna memilih **SALAH SATU** dari sejumlah pilihan yang terbatas.

Contohnya:
Formulir dengan tombol radio:

<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>

Beginilah cara kode HTML di atas akan ditampilkan di browser:

Pilih bahasa web favoritmu:
- HTML
- CSS
- JavaScript

Kotak Centang
<input type="checkbox"> artinya sebuah kotak centang

Contoh formulir kotak centang:
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>

Tampilannya seperti ini:

- [x] i have a bike
- [ ] i have a car
- [ ] i have a boat

Tombol Kirim

`<input type="submit">` mendefinisikan tombol untuk mengirimkan data formulir ke penangan formulir.

Contoh formulir dengan tombol kirim/submit:
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

Munculnya seperti ini:
```sh
First name:
John
Last name:
Doe
```

### Submit

Atribut Nama untuk `<input>`

Perhatikan bahwa setiap bidang input harus memiliki atribut nama yang akan dikirimkan.

Contoh:

Contoh ini tidak akan mengirimkan nilai dari bidang input "Nama depan":
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form>
```
