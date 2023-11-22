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
