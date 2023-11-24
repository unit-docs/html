---
title: Input Type
date : 2023-11-22
draft: true
---

# Jenis Masukan HTML
Bab ini menjelaskan berbagai tipe elemen `<input>` HTML.

## Jenis Masukan HTML

Berikut adalah berbagai jenis masukan yang dapat Anda gunakan dalam HTML:

- `<input type="button">`
- `<input type="checkbox">`
- `<input type="color">`
- `<input type="date">`
- `<input type="datetime-local">`
- `<input type="email">`
- `<input type="file">`
- `<input type="hidden">`
- `<input type="image">`
- `<input type="month">`
- `<input type="number">`
- `<input type="password">`
- `<input type="radio">`
- `<input type="range">`
- `<input type="reset">`
- `<input type="search">`
- `<input type="submit">`
- `<input type="tel">`
- `<input type="text">`
- `<input type="time">`
- `<input type="url">`
- `<input type="week">`

Tip: Nilai default atribut type adalah "teks".

## Teks Jenis Masukan

`<input type="text">` mendefinisikan kolom input teks satu baris:

Contoh
```sh
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```
## Jenis Masukan Kata Sandi

`<input type="password">` mendefinisikan bidang kata sandi:


Contoh
```sh
<form>
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd">
</form>
```
Kata sandi:

Karakter dalam bidang kata sandi ditutupi (ditampilkan sebagai tanda bintang atau lingkaran).

## Jenis Masukan Kirim

`<input type="submit">` mendefinisikan tombol untuk mengirimkan data formulir ke penangan formulir.

Pengendali formulir biasanya merupakan halaman server dengan skrip untuk memproses data masukan.

Pengendali formulir ditentukan dalam atribut tindakan formulir:

Contoh
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

Jika Anda menghilangkan atribut nilai tombol kirim, tombol tersebut akan mendapatkan teks default:


Contoh
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit">
</form>
```
## Reset Tipe Masukan

`<input type="reset">` mendefinisikan tombol reset yang akan mengatur ulang semua nilai formulir ke nilai defaultnya:

Contoh : 
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset" value="Reset">
</form>
```

Jika Anda mengubah nilai input dan kemudian mengklik tombol "Reset", data formulir akan diatur ulang ke nilai default



## Radio Tipe Masukan

`<input type="radio">` mendefinisikan tombol radio.


Tombol radio memungkinkan pengguna memilih HANYA SATU dari sejumlah pilihan:


Contoh
```sh
<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```


## Kotak Centang Jenis Masukan

`<input type="checkbox">` mendefinisikan kotak centang.

Kotak centang memungkinkan pengguna memilih opsi NOL atau LEBIH BANYAK dari sejumlah pilihan terbatas.

Contoh
```sh
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
```

## Tombol Jenis Masukan

`<input type="button">` mendefinisikan sebuah tombol:

Contoh
```sh
<input type="button" onclick="alert('Halo Dunia!')" value="Klik Saya!">
```
Beginilah tampilan kode HTML di atas pada browser:

## Jenis Masukan Warna

`<input type="color">` digunakan untuk kolom input yang harus berisi warna.

Tergantung pada dukungan browser, pemilih warna dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor">
</form>
```
## Jenis Masukan Tanggal

`<input type="date">` digunakan untuk kolom input yang harus berisi tanggal.

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday">
</form>
```
Anda juga dapat menggunakan atribut min dan max untuk menambahkan batasan pada tanggal:

Contoh
```sh
<form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>
  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02">
</form>
```

## Jenis Input Tanggalwaktu-lokal

`<input type="datetime-local">` menentukan kolom input tanggal dan waktu, tanpa zona waktu.

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
</form>
```
## Jenis Masukan Email

`<input type="email">` digunakan untuk kolom input yang harus berisi alamat email.

Tergantung pada dukungan browser, alamat email dapat divalidasi secara otomatis saat dikirimkan.

Beberapa ponsel cerdas mengenali jenis email, dan menambahkan ".com" ke keyboard untuk mencocokkan masukan email.

Contoh
```sh
<form>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
</form>
```

## Jenis Gambar Masukan

`<input type="image">` mendefinisikan gambar sebagai tombol kirim.

Jalur ke gambar ditentukan dalam atribut src.

Contoh
```sh
<form>
<input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
```

## File Jenis Masukan

<input type="file"> mendefinisikan bidang pemilihan file dan tombol "Jelajahi" untuk mengunggah file.

Contoh
```sh
<form>
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile">
</form>
```

## Jenis Masukan Tersembunyi

`<input type="hidden"> `mendefinisikan kolom input tersembunyi (tidak terlihat oleh pengguna).

Bidang tersembunyi memungkinkan pengembang web memasukkan data yang tidak dapat dilihat atau diubah oleh pengguna saat formulir dikirimkan.

Bidang tersembunyi sering kali menyimpan catatan database apa yang perlu diperbarui saat formulir dikirimkan.


Catatan: Meskipun nilai tidak ditampilkan kepada pengguna di konten halaman, nilai tersebut terlihat (dan dapat diedit) menggunakan alat pengembang browser apa pun atau fungsi "Lihat Sumber". Jangan gunakan masukan tersembunyi sebagai bentuk keamanan!


Contoh
```sh
<form>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="hidden" id="custId" name="custId" value="3487">
  <input type="submit" value="Submit">
</form>
```

## Jenis Masukan Bulan

`<input type="month">` memungkinkan pengguna memilih bulan dan tahun.

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
</form>
```

## Nomor Jenis Masukan
`<input type="number">` mendefinisikan kolom input numerik.

Anda juga dapat mengatur batasan nomor mana yang diterima.

Contoh berikut menampilkan kolom input numerik, tempat Anda dapat memasukkan nilai dari 1 hingga 5:

Contoh
```sh
<form>
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
```

Batasan Masukan
Berikut adalah daftar beberapa batasan masukan yang umum:

### Deskripsi Atribut
| Atribut | Deskripsi |
| ----------- | ----------- |
| checked | Menentukan bahwa kolom input harus dipilih sebelumnya saat halaman dimuat (untuk type="checkbox" atau type="radio") |
| disabled | Menentukan bahwa kolom input harus dinonaktifkan |
| max | Menentukan nilai maksimum untuk kolom input |
| maxlength | Menentukan jumlah karakter maksimum untuk kolom input |
| min | Menentukan nilai minimum untuk kolom input |
| pattern | Menentukan ekspresi reguler untuk memeriksa nilai input |
| readonly | Menentukan bahwa kolom masukan bersifat hanya baca (tidak dapat diubah) |
| required | Menentukan bahwa kolom masukan wajib diisi (harus diisi) |
| size | Menentukan lebar (dalam karakter) kolom input |
| step | Menentukan interval angka resmi untuk kolom input |
| value | Menentukan nilai default untuk kolom input |

Anda akan mempelajari lebih lanjut tentang pembatasan masukan di bab berikutnya.


Contoh berikut menampilkan kolom input numerik, tempat Anda dapat memasukkan nilai dari 0 hingga 100, dalam langkah 10. Nilai defaultnya adalah 30:

Contoh
```sh
<form>
  <label for="quantity">Quantity:</label>
  <input type="number" id="quantity" name="quantity" min="0" max="100" step="10" value="30">
</form>
```


## Jenis Masukan Kirim

`<input type="submit">` mendefinisikan tombol untuk mengirimkan data formulir ke penangan formulir.

Pengendali formulir biasanya merupakan halaman server dengan skrip untuk memproses data masukan.

Pengendali formulir ditentukan dalam atribut tindakan formulir:

Contoh
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```
Jika Anda menghilangkan atribut nilai tombol kirim, tombol tersebut akan mendapatkan teks default:

Contoh
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit">
</form>
```

## Reset Tipe Masukan
`<input type="reset">` mendefinisikan tombol reset yang akan mengatur ulang semua nilai formulir ke nilai defaultnya:

Contoh : 
```sh
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset" value="Reset">
</form>
```
Jika Anda mengubah nilai input dan kemudian mengklik tombol "Reset", data formulir akan diatur ulang ke nilai default



## Radio Tipe Masukan

`<input type="radio">` mendefinisikan tombol radio.

Tombol radio memungkinkan pengguna memilih HANYA SATU dari sejumlah pilihan:

Contoh
```sh
<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```


## Kotak Centang Jenis Masukan

`<input type="checkbox">` mendefinisikan kotak centang.

Kotak centang memungkinkan pengguna memilih opsi NOL atau LEBIH BANYAK dari sejumlah pilihan terbatas.

Contoh
```sh
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
```

## Tombol Jenis Masukan

`<input type="button">` mendefinisikan sebuah tombol:

Contoh
```sh
<input type="button" onclick="alert('Halo Dunia!')" value="Klik Saya!">
```


## Jenis Masukan Tanggal
`<input type="date">` digunakan untuk kolom input yang harus berisi tanggal.

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday">
</form>
```
Anda juga dapat menggunakan atribut min dan max untuk menambahkan batasan pada tanggal:

Contoh
```sh
<form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>
  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02">
</form>
Jenis Input Tanggalwaktu-lokal
<input type="datetime-local"> menentukan kolom input tanggal dan waktu, tanpa zona waktu.
```

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
</form>
```

## Jenis Masukan Email
`<input type="email">` digunakan untuk kolom input yang harus berisi alamat email.

Tergantung pada dukungan browser, alamat email dapat divalidasi secara otomatis saat dikirimkan.

Beberapa ponsel cerdas mengenali jenis email, dan menambahkan ".com" ke keyboard untuk mencocokkan masukan email.

Contoh
```sh
<form>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
</form>
```

## Jenis Gambar Masukan
`<input type="image">` mendefinisikan gambar sebagai tombol kirim.

Jalur ke gambar ditentukan dalam atribut src.

Contoh
```sh
<form>
<input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
```

## File Jenis Masukan
`<input type="file">` mendefinisikan bidang pemilihan file dan tombol "Jelajahi" untuk mengunggah file.

Contoh
```sh
<form>
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile">
</form>
```

## Jenis Masukan Tersembunyi
`<input type="hidden">` mendefinisikan kolom input tersembunyi (tidak terlihat oleh pengguna).

Bidang tersembunyi memungkinkan pengembang web memasukkan data yang tidak dapat dilihat atau diubah oleh pengguna saat formulir dikirimkan.

Bidang tersembunyi sering kali menyimpan catatan database apa yang perlu diperbarui saat formulir dikirimkan.

Catatan: Meskipun nilai tidak ditampilkan kepada pengguna di konten halaman, nilai tersebut terlihat (dan dapat diedit) menggunakan alat pengembang browser apa pun atau fungsi "Lihat Sumber". Jangan gunakan masukan tersembunyi sebagai bentuk keamanan!

Contoh
```sh
<form>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="hidden" id="custId" name="custId" value="3487">
  <input type="submit" value="Submit">
</form>
```

## Jenis Masukan Bulan
`<input type="month">` memungkinkan pengguna memilih bulan dan tahun.

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
</form>
```


## Rentang Jenis Masukan

`<input type="range">` mendefinisikan kontrol untuk memasukkan angka yang nilai pastinya tidak penting (seperti kontrol penggeser). Rentang defaultnya adalah 0 hingga 100. Namun, Anda dapat menetapkan batasan pada angka yang diterima dengan atribut min, max, dan step:

Contoh
```sh
<form>
  <label for="vol">Volume (between 0 and 50):</label>
  <input type="range" id="vol" name="vol" min="0" max="50">
</form>
```

## Pencarian Jenis Masukan

`<input type="search">` digunakan untuk bidang pencarian (bidang pencarian berperilaku seperti bidang teks biasa).


Contoh
```sh
<form>
  <label for="gsearch">Search Google:</label>
  <input type="search" id="gsearch" name="gsearch">
</form>
```

## Jenis Masukan Telp

`<input type="tel">` digunakan untuk kolom input yang harus berisi nomor telepon.

Contoh
```sh
<form>
  <label for="phone">Enter your phone number:</label>
  <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
```

## Jenis Masukan Waktu

`<input type="time">` memungkinkan pengguna memilih waktu (tanpa zona waktu).


Bergantung pada dukungan browser, pemilih waktu dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="appt">Select a time:</label>
  <input type="time" id="appt" name="appt">
</form>
```

## Url Jenis Masukan

`<input type="url">` digunakan untuk kolom input yang harus berisi alamat URL.

Bergantung pada dukungan browser, bidang url dapat divalidasi secara otomatis saat dikirimkan.

Beberapa ponsel cerdas mengenali jenis url, dan menambahkan ".com" ke keyboard untuk mencocokkan masukan url.


Contoh
```sh
<form>
  <label for="homepage">Add your homepage:</label>
  <input type="url" id="homepage" name="homepage">
</form>
```

## Jenis Masukan Minggu

`<input type="week">` memungkinkan pengguna memilih minggu dan tahun.

Bergantung pada dukungan browser, pemilih tanggal dapat muncul di kolom input.

Contoh
```sh
<form>
  <label for="week">Select a week:</label>
  <input type="week" id="week" name="week">
</form>
```
