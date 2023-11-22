# HTML ELEMENTS
Elemen HTML ditentukan oleh tag awal, beberapa konten, dan tag akhir.
## Elemen HTML
Elemen HTML adalah segalanya mulai dari tag awal hingga tag akhir:
<tagname>Konten ada di sini...</tagname>
Contoh beberapa elemen HTML:
``` sh
<h1>Judul Pertama Saya</h1>
```
``` sh
<p>Paragraf pertama saya.</p>
```

![ibnu](https://github.com/uin-unit/docs-html/blob/main/images/elements.png)

Elemen HTML dapat disarangkan (artinya elemen dapat berisi elemen lain).
Semua dokumen HTML terdiri dari elemen HTML bersarang.
Contoh berikut berisi empat elemen HTML (`<html>`, `<body>`,  `<h1>` dan `<p>`):
Contoh : 
``` sh
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```
## MENJELASKAN CONTOH
Elemen `<html>` adalah elemen root dan mendefinisikan keseluruhan dokumen HTML.
Ini memiliki tag awal `<html>` dan tag akhir `</html>`.
Kemudian, di dalam elemen `<html>` terdapat elemen <body>:
``` sh
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
```
Elemen `<body>` mendefinisikan isi dokumen.
Ini memiliki tag awal `<body>` dan tag akhir `</body>`.
Lalu, di dalam elemen `<body>` terdapat dua elemen lainnya: `<h1>` dan `<p>`:
``` sh
<h1>My First Heading</h1>
<p>My first paragraph.</p>
```
Elemen `<h1>` mendefinisikan sebuah judul.
Ini memiliki tag awal `<h1>` dan tag akhir `</h1>`:
``` sh
<h1>My First Heading</h1>
```
Elemen `<p>` mendefinisikan sebuah paragraf.
Ini memiliki tag awal `<p>` dan tag akhir `<p>`:
``` sh
<p>My first paragraph.</p>
```
## Jangan Pernah Lewati Tag Akhir
Beberapa elemen HTML akan ditampilkan dengan benar, meskipun Anda lupa tag penutupnya:
Contoh : 
``` sh
<html>
<body>

<p>This is a paragraph
<p>This is a paragraph

</body>
</html>
```
Namun, jangan pernah mengandalkan ini! Hasil yang tidak terduga dan kesalahan mungkin terjadi jika Anda lupa tag penutup!
## Elemen HTML Kosong
Elemen HTML yang tidak memiliki konten disebut elemen kosong.
Tag `<br>` mendefinisikan jeda baris, dan merupakan elemen kosong tanpa tag penutup:
Contoh : 
``` sh
<p>This is a <br> paragraph with a line break.</p>
```
## HTML Tidak Peka Huruf Besar-kecil
Tag HTML tidak membedakan huruf besar-kecil: `<P>` artinya sama dengan `<p>`.
Standar HTML tidak memerlukan tag huruf kecil, tetapi W3C merekomendasikan huruf kecil dalam HTML, dan memerlukan huruf kecil untuk jenis dokumen yang lebih ketat seperti XHTML.
