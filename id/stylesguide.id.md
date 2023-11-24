# Panduan Gaya HTML
Kode HTML yang konsisten, bersih, dan rapi memudahkan orang lain membaca dan memahami kode Anda.
Berikut beberapa panduan dan tips membuat kode HTML yang baik.
## Selalu Deklarasikan Jenis Dokumen
Selalu nyatakan jenis dokumen sebagai baris pertama dalam dokumen Anda.
Jenis dokumen yang benar untuk HTML adalah:
```sh
<!DOCTYPE html>
```
## Gunakan Nama Elemen Huruf Kecil
HTML memungkinkan pencampuran huruf besar dan kecil dalam nama elemen.
Namun, sebaiknya gunakan nama elemen dengan huruf kecil, karena:
Mencampur nama huruf besar dan kecil terlihat buruk
Pengembang biasanya menggunakan nama huruf kecil
Huruf kecil terlihat lebih bersih
Huruf kecil lebih mudah untuk ditulis
### Good:
```sh
<body>
<p>This is a paragraph.</p>
</body>
```
### Bad:
```sh
<BODY>
<P>This is a paragraph.</P>
</BODY>
```
## Tutup Semua Elemen HTML
Dalam HTML, Anda tidak harus menutup semua elemen (misalnya elemen <p>).
Namun, kami sangat menyarankan untuk menutup semua elemen HTML, seperti ini:
### Good:
```sh
<section>
  <p>This is a paragraph.</p>
  <p>This is a paragraph.</p>
</section>
```
### Bad:
```sh
<section>
  <p>This is a paragraph.
  <p>This is a paragraph.
</section>
```
## Gunakan Nama Atribut Huruf Kecil
HTML memungkinkan pencampuran huruf besar dan kecil dalam nama atribut.
Namun, sebaiknya gunakan nama atribut dengan huruf kecil, karena:
Mencampur nama huruf besar dan kecil terlihat buruk
Pengembang biasanya menggunakan nama huruf kecil
Huruf kecil terlihat lebih bersih
Huruf kecil lebih mudah untuk ditulis
### Good:
```sh
<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
```
### Bad:
```sh
<a HREF="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
```
## Selalu Kutip Nilai Atribut
HTML mengizinkan nilai atribut tanpa tanda kutip.
Namun, kami menyarankan untuk mengutip nilai atribut, karena:
Pengembang biasanya mengutip nilai atribut
Nilai yang dikutip lebih mudah dibaca
Anda HARUS menggunakan tanda kutip jika nilainya mengandung spasi
### Good:
```sh
<table class="striped">
```
### Bad:
```sh
<table class=striped>
```
### Very bad:
Ini tidak akan berhasil, karena nilainya mengandung spasi:
```sh
<table class=table striped>
```
## Selalu Tentukan alt, lebar, dan tinggi untuk Gambar
Selalu tentukan atribut alt untuk gambar. Atribut ini penting jika gambar karena alasan tertentu tidak dapat ditampilkan.
Selain itu, selalu tentukan lebar dan tinggi gambar. Hal ini mengurangi kedipan, karena browser dapat menyediakan ruang untuk gambar sebelum memuat.
### Good:
```sh
<img src="html5.gif" alt="HTML5" style="width:128px;height:128px">
```
### Bad:
```sh
<img src="html5.gif">
```
## Spasi dan Tanda Sama Dengan
HTML mengizinkan spasi di sekitar tanda sama dengan. Namun tanpa ruang lebih mudah dibaca dan mengelompokkan entitas dengan lebih baik.
### Good:
```sh
<link rel="stylesheet" href="styles.css">
```
### Bad:
```sh
<link rel = "stylesheet" href = "styles.css">
```
## Hindari Baris Kode yang Panjang
Saat menggunakan editor HTML, TIDAK nyaman untuk menggulir ke kanan dan ke kiri untuk membaca kode HTML.
Cobalah untuk menghindari baris kode yang terlalu panjang.
## Garis Kosong dan Indentasi
Jangan menambahkan baris kosong, spasi, atau lekukan tanpa alasan.
Agar mudah dibaca, tambahkan baris kosong untuk memisahkan blok kode yang besar atau logis.
Agar mudah dibaca, tambahkan dua spasi indentasi. Jangan gunakan tombol tab.
### Good:
```sh
<body>

<h1>Famous Cities</h1>

<h2>Tokyo</h2>
<p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>

<h2>London</h2>
<p>London is the capital city of England. It is the most populous city in the United Kingdom.</p>

<h2>Paris</h2>
<p>Paris is the capital of France. The Paris area is one of the largest population centers in Europe.</p>

</body>
```
### Bad:
```sh
<body>
<h1>Famous Cities</h1>
<h2>Tokyo</h2><p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area, and the most populous metropolitan area in the world.</p>
<h2>London</h2><p>London is the capital city of England. It is the most populous city in the United Kingdom.</p>
<h2>Paris</h2><p>Paris is the capital of France. The Paris area is one of the largest population centers in Europe.</p>
</body>
```
### Good Table Example:
```sh
<table>
  <tr>
    <th>Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>A</td>
    <td>Description of A</td>
  </tr>
  <tr>
    <td>B</td>
    <td>Description of B</td>
  </tr>
</table>
```
### Good List Example:
```sh
<ul>
  <li>London</li>
  <li>Paris</li>
  <li>Tokyo</li>
</ul>
```
## Jangan Pernah Lewati Elemen `<title>`
Elemen `<title>` diperlukan dalam HTML.
Isi judul halaman sangat penting untuk optimasi mesin pencari (SEO)! Judul halaman digunakan oleh algoritma mesin pencari untuk menentukan urutan ketika mencantumkan halaman dalam hasil pencarian.
Elemen `<title>`:
mendefinisikan judul di toolbar browser
memberikan judul untuk halaman ketika ditambahkan ke favorit
menampilkan judul halaman di hasil mesin pencari
Jadi, usahakan untuk membuat judul seakurat dan bermakna mungkin:
```sh
<title>HTML Style Guide and Coding Conventions</title>
```
## Menghilangkan `<html>` dan `<body>`?
Halaman HTML akan divalidasi tanpa tag `<html>` dan `<body>`:
Contoh : 
```sh
<!DOCTYPE html>
<head>
  <title>Page Title</title>
</head>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>
```
Namun, kami sangat menyarankan untuk selalu menambahkan tag `<html>` dan `<body>`!
Menghilangkan `<body>` dapat menghasilkan kesalahan pada browser lama.
Menghilangkan `<html>` dan `<body>` juga dapat menyebabkan crash pada perangkat lunak DOM dan XML.
## Menghilangkan `<head>`?
Tag HTML `<head>` juga dapat dihilangkan.
Browser akan menambahkan semua elemen sebelum `<body>`, ke elemen `<head>` default.
Contoh : 
```sh
<!DOCTYPE html>
<html>
<title>Page Title</title>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
Namun, kami menyarankan penggunaan tag <head>.
```
## Tutup Elemen HTML Kosong?
Dalam HTML, menutup elemen kosong adalah opsional.
## Allowed:
```sh
<meta charset="utf-8">
```
## Also Allowed:
```sh
<meta charset="utf-8" />
```
Jika Anda mengharapkan perangkat lunak XML/XHTML mengakses halaman Anda, pertahankan garis miring penutup (/), karena ini diperlukan dalam XML dan XHTML.
## Tambahkan Atribut lang
Anda harus selalu menyertakan atribut lang di dalam tag `<html>`, untuk mendeklarasikan bahasa halaman Web. Ini dimaksudkan untuk membantu mesin pencari dan browser.
Contoh : 
```sh
<!DOCTYPE html>
<html lang="en-us">
<head>
  <title>Page Title</title>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
## Data Meta
Untuk memastikan interpretasi yang tepat dan pengindeksan mesin pencari yang benar, bahasa dan pengkodean karakter `<meta charset="charset">` harus didefinisikan sedini mungkin dalam dokumen HTML:
```sh
<!DOCTYPE html>
<html lang="en-us">
<head>
  <meta charset="UTF-8">
  <title>Page Title</title>
</head>
```
## Mengatur Area Pandang
Area pandang adalah area halaman web yang terlihat oleh pengguna. Ukurannya berbeda-beda tergantung perangkatnya - ukurannya akan lebih kecil di ponsel dibandingkan di layar komputer.
Anda harus menyertakan elemen `<meta>` berikut di semua halaman web Anda:
```sh
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
Ini memberikan instruksi kepada browser tentang cara mengontrol dimensi dan penskalaan halaman.
Bagian `width=device-width` mengatur lebar halaman agar mengikuti lebar layar perangkat (yang bervariasi tergantung pada perangkat).
Bagian skala awal=1.0 mengatur tingkat zoom awal saat halaman pertama kali dimuat oleh browser.
Berikut adalah contoh halaman web tanpa meta tag viewport, dan halaman web yang sama dengan meta tag viewport:
## Komentar HTML
Komentar singkat sebaiknya ditulis dalam satu baris, seperti ini:
```sh
<!-- This is a comment -->
```
Komentar yang lebih dari satu baris, sebaiknya ditulis seperti ini:
```sh
<!--
  This is a long comment example. This is a long comment example.
  This is a long comment example. This is a long comment example.
-->
```
Komentar yang panjang lebih mudah diamati jika diindentasi dengan dua spasi.
## Menggunakan Style Sheet
Gunakan sintaks sederhana untuk menghubungkan ke style sheet (atribut type tidak diperlukan):
```sh
<link rel="stylesheet" href="styles.css">
```
Aturan CSS singkat dapat ditulis terkompresi, seperti ini:
```sh
p.intro {font-family:Verdana;font-size:16em;}
```
Aturan CSS yang panjang harus ditulis dalam beberapa baris:
```sh
body {
  background-color: lightgrey;
  font-family: "Arial Black", Helvetica, sans-serif;
  font-size: 16em;
  color: black;
}
```
Tempatkan braket pembuka pada garis yang sama dengan pemilih
Gunakan satu spasi sebelum braket pembuka
Gunakan dua spasi lekukan
Gunakan titik koma setelah setiap pasangan nilai properti, termasuk yang terakhir
Hanya gunakan tanda kutip di sekitar nilai jika nilai tersebut mengandung spasi
Tempatkan tanda kurung tutup pada baris baru, tanpa spasi di depannya
## Memuat JavaScript dalam HTML
Gunakan sintaks sederhana untuk memuat skrip eksternal (atribut type tidak diperlukan):
```sh
<script src="myscript.js">
```
## Mengakses Elemen HTML dengan JavaScript
Menggunakan kode HTML yang "tidak rapi" dapat mengakibatkan kesalahan JavaScript.
Kedua pernyataan JavaScript ini akan menghasilkan hasil yang berbeda:
Contoh : 
```sh
getElementById("Demo").innerHTML = "Hello";
```
```sh
getElementById("demo").innerHTML = "Hello";
```
getElementById("demo").innerHTML = "Hello";
## Gunakan Nama File Huruf Kecil
Beberapa server web (Apache, Unix) peka huruf besar-kecil mengenai nama file: "london.jpg" tidak dapat diakses sebagai "London.jpg".
Server web lain (Microsoft, IIS) tidak peka huruf besar-kecil: "london.jpg" dapat diakses sebagai "London.jpg".
Jika Anda menggunakan campuran huruf besar dan kecil, Anda harus mewaspadai hal ini.
Jika Anda berpindah dari server yang tidak peka huruf besar/kecil ke server peka huruf besar/kecil, kesalahan kecil sekalipun akan merusak web Anda!
Untuk menghindari masalah ini, selalu gunakan nama file dengan huruf kecil!
## Ekstensi File
File HTML harus memiliki ekstensi .html (.htm diperbolehkan).
File CSS harus memiliki ekstensi .css.
File JavaScript harus memiliki ekstensi .js.
## Perbedaan Antara .htm dan .html?
Tidak ada perbedaan antara ekstensi file .htm dan .html!

