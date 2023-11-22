----
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---
# Grafik HTML SVG
SVG mendefinisikan grafik berbasis vektor dalam format XML.

**Apa yang dimaksud dengan SVG?**
- SVG adalah singkatan dari Scalable Vector Graphics
- SVG digunakan untuk mendefinisikan grafik untuk Web
- SVG adalah rekomendasi W3C

 **Elemen HTML** `<svg>`
 
Elemen HTML `<svg>` adalah wadah untuk grafik SVG.
SVG memiliki beberapa metode untuk menggambar jalur, kotak, lingkaran, teks, dan gambar grafik.

**Dukungan Browser**

![grafik html svg](https://github.com/uin-unit/docs-html/blob/main/images/grafik%20html%20svg.png)

**Lingkaran SVG**

![grafik html svg1](https://github.com/uin-unit/docs-html/blob/main/images/grafik%20html%20svg(1).png)

Contoh : 
```sh
<!DOCTYPE html>
<html>
<body>

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>

</body>
</html>
```

**SVG Persegi Panjang**

![grafik html svg2](https://github.com/uin-unit/docs-html/blob/main/images/grafik%20html%20svg(2).png)

Contoh : 

```sh
<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
  style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
</svg>
```

**Bintang SVG**

![grafik html svg3](https://github.com/uin-unit/docs-html/blob/main/images/grafik%20html%20svg(3).png)

Contoh : 

``` sh
<svg width="300" height="200">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>
```

**Logo SVG**

![grafik html svg4](https://github.com/uin-unit/docs-html/blob/main/images/grafik%20html%20svg(4).png)

Contoh : 

```sh
<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
  Sorry, your browser does not support inline SVG.
</svg>
```

**Perbedaan Antara SVG dan Kanvas**

SVG adalah bahasa untuk menggambarkan grafik 2D dalam XML.
Canvas menggambar grafik 2D, dengan cepat (dengan JavaScript).
SVG berbasis XML, yang berarti setiap elemen tersedia dalam DOM SVG. Anda dapat melampirkan penangan peristiwa JavaScript untuk sebuah elemen.
Dalam SVG, setiap bentuk yang digambar diingat sebagai objek. Jika atribut objek SVG diubah, browser dapat secara otomatis merender ulang bentuk tersebut.
Kanvas dirender piksel demi piksel. Dalam kanvas, setelah grafik digambar, grafik akan dilupakan oleh browser. Jika posisinya harus diubah, seluruh adegan harus digambar ulang, termasuk objek apa pun yang mungkin tertutupi oleh grafik.

**Perbandingan Kanvas dan SVG**

Tabel di bawah ini menunjukkan beberapa perbedaan penting antara Canvas dan SVG:

| Kanvas | SVG |
| ----------- | ----------- |
| Tergantung resolusi | Resolusi independen |
| Tidak ada dukungan untuk penangan peristiwa | Dukungan untuk penangan peristiwa |
| Kemampuan rendering teks yang buruk| Paling cocok untuk aplikasi dengan area rendering yang besar (Google Maps) |
| Anda dapat menyimpan gambar yang dihasilkan sebagai .png atau .jpg | Rendering lambat jika kompleks (apa pun yang banyak menggunakan DOM akan lambat) |
| Sangat cocok untuk game dengan grafis intensif | Tidak cocok untuk aplikasi game |

