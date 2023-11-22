# Elemen Semantik HTML
Unsur semantik = unsur yang mempunyai makna.


## Apa itu Elemen Semantik?
Elemen semantik dengan jelas menggambarkan maknanya bagi browser dan pengembang.
Contoh elemen non-semantik: <div> dan <span> - Tidak menceritakan apa pun tentang isinya.
Contoh elemen semantik: <form>, <table>, dan <article> - Mendefinisikan kontennya dengan jelas.
## Elemen Semantik dalam HTML
Banyak situs web berisi kode HTML seperti: <div id="nav"> <div class="header"> <div id="footer"> untuk menunjukkan navigasi, header, dan footer.
Dalam HTML ada beberapa elemen semantik yang dapat digunakan untuk mendefinisikan berbagai bagian halaman web:
- <  article  >
- <  aside  >
- <  details  >
- <  figcaption >
- <  figure  >
- <  footer  >
- <  header  >
- <  main  >
- <  mark  >
- <  nav  >
- <  section  >
- <  summary  >
- <  time  >
- ![alt text](https://github.com/uin-unit/docs-html/blob/main/images/element.gif)

## Elemen <bagian> HTML
Elemen <section> mendefinisikan bagian dalam dokumen.
Menurut dokumentasi HTML W3C: "Bagian adalah pengelompokan konten secara tematik, biasanya dengan judul."
Contoh penggunaan elemen <section>:
bab
Perkenalan
Item berita
Kontak informasi
Halaman web biasanya dapat dibagi menjadi beberapa bagian untuk pengenalan, konten, dan informasi kontak.

Contoh :
Dua bagian dalam sebuah dokumen:

<section>
<h1>WWF</h1>
<p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>

<section>
<h1>WWF's Panda symbol</h1>
<p>The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.</p>
</section>

## Elemen HTML <artikel>
Elemen <article> menentukan konten independen dan mandiri.
Sebuah artikel harus masuk akal, dan dapat didistribusikan secara terpisah dari situs web lainnya.
Contoh penggunaan elemen <article>:
Postingan forum
Postingan blog
Komentar pengguna
Kartu produk
Artikel koran
Contoh : 
Tiga artikel dengan konten yang berdiri sendiri dan mandiri:
```sh
<article>
<h2>Google Chrome</h2>
<p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
</article>
<article>
<h2>Mozilla Firefox</h2>
<p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
</article>
<article>
<h2>Microsoft Edge</h2>
<p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
</article>
```
Contoh :  2
Gunakan CSS untuk memberi gaya pada elemen <artikel>:
```sh
<html>
<head>
<style>
.all-browsers {
  margin: 0;
  padding: 5px;
  background-color: lightgray;
}
.all-browsers > h1, .browser {
  margin: 10px;
  padding: 5px;
}
.browser {
  background: white;
}
.browser > h2, p {
  margin: 4px;
  font-size: 90%;
}
</style>
</head>
<body>

<article class="all-browsers">
  <h1>Most Popular Browsers</h1>
  <article class="browser">
    <h2>Google Chrome</h2>
    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
</article>
  <article class="browser">
    <h2>Mozilla Firefox</h2>
    <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
</article>
  <article class="browser">
    <h2>Microsoft Edge</h2>
    <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
 </article>
</article>

</body>
</html>
```
## Menyusun <artikel> di <bagian> atau sebaliknya?
Elemen <article> menentukan konten independen dan mandiri.
Elemen <section> mendefinisikan bagian dalam dokumen.
Bisakah kita menggunakan definisi tersebut untuk memutuskan cara menyusun elemen-elemen tersebut? Tidak, kita tidak bisa!
Jadi, Anda akan menemukan halaman HTML dengan elemen <section> yang berisi elemen <article>, dan elemen <article> yang berisi elemen <section>.

## Elemen HTML <header>
Elemen <header> mewakili wadah untuk konten pengantar atau sekumpulan tautan navigasi.
Elemen <header> biasanya berisi:
satu atau lebih elemen judul (<h1> - <h6>)
logo atau ikon
informasi kepenulisan
Catatan: Anda dapat memiliki beberapa elemen <header> dalam satu dokumen HTML. Namun, <header> tidak dapat ditempatkan dalam elemen <footer>, <address>, atau <header> lainnya.
Contoh : 
Tajuk untuk <artikel>:
```sh
<article>
  <header>
    <h1>What Does WWF Do?</h1>
    <p>WWF's mission:</p>
  </header>
  <p>WWF's mission is to stop the degradation of our planet's natural environment,
  and build a future in which humans live in harmony with nature.</p>
</article>
```

## Elemen HTML <footer>
Elemen <footer> mendefinisikan footer untuk dokumen atau bagian.
Elemen <footer> biasanya berisi:
informasi kepenulisan
informasi hak cipta
kontak informasi
peta situs
kembali ke tautan atas
Dokumen terkait
Anda dapat memiliki beberapa elemen <footer> dalam satu dokumen.
Contoh : 
Bagian footer dalam dokumen:
```sh
<footer>
  <p>Author: Hege Refsnes</p>
  <p><a href="mailto:hege@example.com">hege@example.com</a></p>
```
## HTML Elemen <nav>
Elemen <nav> mendefinisikan sekumpulan tautan navigasi.
Contoh : 
Satu set tautan navigasi:
```sh
<nav>
  <a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav>
```
## Elemen HTML <samping>
Elemen <aside> mendefinisikan beberapa konten selain konten tempatnya ditempatkan (seperti sidebar).
Konten <aside> harus berhubungan secara tidak langsung dengan konten di sekitarnya.
Contoh : 
Menampilkan beberapa konten selain dari konten yang ditempatkan:
```sh
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
<h4>Epcot Center</h4>
<p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>
```
Contoh :  2
Gunakan CSS untuk memberi gaya pada elemen <samping>:
```sh
<html>
<head>
<style>
aside {
  width: 30%;
  padding-left: 15px;
  margin-left: 15px;
  float: right;
  font-style: italic;
  background-color: lightgray;
}
</style>
</head>
<body>

<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

<aside>
<p>The Epcot center is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
</aside>

<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>
<p>My family and I visited The Epcot center this summer. The weather was nice, and Epcot was amazing! I had a great summer together with my family!</p>

</body>
</html>
```
## Elemen HTML <figure> dan <figcaption>
Tag <figure> menentukan konten mandiri, seperti ilustrasi, diagram, foto, daftar kode, dll.
Tag <figcaption> mendefinisikan keterangan untuk elemen <figure>. Elemen <figcaption> dapat ditempatkan sebagai anak pertama atau sebagai anak terakhir dari elemen <figure>.
Elemen <img> mendefinisikan gambar/ilustrasi sebenarnya.
Contoh : 
```sh
<figure>
  <img src="pic_trulli.jpg" alt="Trulli">
  <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure>
```
Mengapa Elemen Semantik?
Menurut W3C: "Web semantik memungkinkan data untuk dibagikan dan digunakan kembali di seluruh aplikasi, perusahaan, dan komunitas."

Elemen Semantik dalam HTML
Di bawah ini adalah daftar beberapa elemen semantik dalam HTML.
## Deskripsi Tag
<artikel> Mendefinisikan konten independen dan mandiri
<aside> Mendefinisikan konten selain konten halaman
<details> Mendefinisikan detail tambahan yang dapat dilihat atau disembunyikan pengguna
<figcaption> Mendefinisikan keterangan untuk elemen <figure>
<figure> Menentukan konten mandiri, seperti ilustrasi, diagram, foto, daftar kode, dll.
<footer> Mendefinisikan footer untuk dokumen atau bagian
<header> Menentukan header untuk dokumen atau bagian
<main> Menentukan konten utama dokumen
<mark> Mendefinisikan teks yang ditandai/disorot
<nav> Mendefinisikan link navigasi
<section> Mendefinisikan bagian dalam dokumen
<summary> Mendefinisikan judul yang terlihat untuk elemen <details>
<waktu> Mendefinisikan tanggal/waktu




