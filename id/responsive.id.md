# Desain Web Responsif HTML
Desain web responsif adalah tentang membuat halaman web yang terlihat bagus di semua perangkat!
Desain web yang responsif akan secara otomatis menyesuaikan dengan ukuran layar dan area pandang yang berbeda.
## Apa itu Desain Web Responsif?
Desain Web Responsif adalah tentang penggunaan HTML dan CSS untuk secara otomatis mengubah ukuran, menyembunyikan, mengecilkan, atau memperbesar situs web, agar terlihat bagus di semua perangkat (desktop, tablet, dan ponsel):
## Mengatur Area Pandang
Untuk membuat situs web responsif, tambahkan tag <meta> berikut ke semua halaman web Anda:

Contoh :
```sh
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
Ini akan mengatur area pandang halaman Anda, yang akan memberikan instruksi kepada browser tentang cara mengontrol dimensi dan penskalaan halaman.
Berikut adalah contoh halaman web tanpa meta tag viewport, dan halaman web yang sama dengan meta tag viewport:
![radhi](https://github.com/uin-unit/docs-html/blob/main/images/image%20responsif.png)

## Gambar Responsif
Gambar responsif adalah gambar yang dapat diskalakan dengan baik agar sesuai dengan ukuran browser apa pun.
Menggunakan Properti lebar
Jika properti lebar CSS disetel ke 100%, gambar akan responsif dan skalanya naik dan turun:

Contoh : 
```sh
<img src="img_girl.jpg" style="width:100%;">
```
Perhatikan bahwa pada contoh di atas, gambar dapat diperbesar menjadi lebih besar dari ukuran aslinya. Solusi yang lebih baik, dalam banyak kasus, adalah dengan menggunakan properti max-width.
Menggunakan Properti max-width
Jika properti max-width diatur ke 100%, gambar akan diperkecil jika perlu, namun jangan pernah diperbesar hingga lebih besar dari ukuran aslinya:

Contoh : 
```sh
<img src="img_girl.jpg" style="max-width:100%;height:auto;">
```


Tampilkan Gambar Berbeda Tergantung Lebar Browser
Elemen HTMl <  picture  > memungkinkan Anda menentukan gambar berbeda untuk ukuran jendela browser berbeda.
Ubah ukuran jendela browser untuk melihat bagaimana gambar di bawah berubah tergantung pada lebarnya:

Contoh : 
```sh
<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
  <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
  <source srcset="flowers.jpg">
  <img src="img_smallflower.jpg" alt="Flowers">
</picture>
```
Ukuran Teks Responsif
Ukuran teks dapat diatur dengan satuan "vw", yang berarti "lebar viewport".
Dengan begitu ukuran teks akan mengikuti ukuran jendela browser:

Contoh : 
```sh
<h1 style="font-size:10vw">Hello World</h1>
```
## Pertanyaan Media
Selain mengubah ukuran teks dan gambar, penggunaan kueri media di halaman web responsif juga umum dilakukan.
Dengan kueri media, Anda dapat menentukan gaya yang sangat berbeda untuk ukuran browser berbeda.
Contoh: ubah ukuran jendela browser untuk melihat bahwa tiga elemen div di bawah ini akan ditampilkan secara horizontal pada layar besar dan ditumpuk secara vertikal pada layar kecil:

Left Menu



Main Content



Right Content

Contoh : 
```sh
<style>
.left, .right {
  float: left;
  width: 20%; /* The width is 20%, by default */
}

.main {
  float: left;
  width: 60%; /* The width is 60%, by default */
}

/* Use a media query to add a breakpoint at 800px: */
@media screen and (max-width: 800px) {
  .left, .main, .right {
    width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
  }
}
</style>
```
## Halaman Web Responsif - Contoh Lengkap
Halaman web yang responsif akan terlihat bagus di layar desktop besar dan di ponsel kecil.
## Desain Web Responsif - Kerangka Kerja
Semua Kerangka CSS populer menawarkan desain responsif.
Semuanya gratis dan mudah digunakan.

W3.CSS

W3.CSS adalah kerangka kerja CSS modern dengan dukungan untuk desain desktop, tablet, dan seluler secara default.

W3.CSS lebih kecil dan lebih cepat dibandingkan kerangka CSS serupa.

W3.CSS dirancang untuk tidak bergantung pada jQuery atau pustaka JavaScript lainnya.

