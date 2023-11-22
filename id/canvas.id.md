---
title: Canvas
date : 2023-11-22
draft: true
---

# Canvas HTML

![canvas1](https://github.com/uin-unit/docs-html/blob/main/images/canvas1.png)

Elemen HTML <canvas> digunakan untuk menggambar grafik pada halaman web.

![canvas1](https://github.com/uin-unit/docs-html/blob/main/images/canvas1.png)

Grafik di sebelah kiri dibuat dengan `<canvas>`. Grafik tersebut menunjukkan empat elemen: persegi panjang merah, persegi panjang gradien, persegi 

panjang multiwarna, dan teks multiwarna.

## Apa yang dimaksud dengan Kanvas HTML?

Elemen HTML `<canvas>` digunakan untuk menggambar grafik, dengan cepat, melalui JavaScript.

Elemen `<canvas>` hanya merupakan wadah untuk grafik. Anda harus menggunakan JavaScript untuk menggambar grafik.

Kanvas memiliki beberapa metode untuk menggambar jalur, kotak, lingkaran, teks, dan menambahkan gambar.

## Dukungan Browser

Angka-angka pada tabel menentukan versi browser pertama yang sepenuhnya mendukung elemen `<canvas>`.

![canvas1](https://github.com/uin-unit/docs-html/blob/main/images/audio1.png)

Contoh Kanvas

Kanvas adalah area persegi panjang pada halaman HTML. Secara default, kanvas tidak memiliki batas dan konten.

Markupnya terlihat seperti ini:

`<canvas id="myCanvas" width="200" height="100"></canvas>`

Catatan: Selalu tentukan atribut id (untuk dirujuk dalam skrip), dan atribut lebar dan tinggi untuk menentukan ukuran kanvas. Untuk menambahkan 

batas, gunakan atribut style.

Berikut ini adalah contoh kanvas dasar yang kosong:

![canvas2](https://github.com/uin-unit/docs-html/blob/main/images/canvas2.png)

Contoh :

```sh
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;">
</canvas>
```

## Menambahkan JavaScript

Setelah membuat area kanvas persegi panjang, Anda harus menambahkan JavaScript untuk menggambar.

Berikut ini beberapa contohnya:

**Menggambar Sebuah Garis**

![canvas3](https://github.com/uin-unit/docs-html/blob/main/images/canvas3.png)

contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.moveTo(0, 0);
ctx.lineTo(200, 100);
ctx.stroke();
</script>
```

**Menggambar sebuah lingkaran**

![canvas4](https://github.com/uin-unit/docs-html/blob/main/images/canvas4.png)

contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(95, 50, 40, 0, 2 * Math.PI);
ctx.stroke();
</script>
```

**Menggambar Teks**

![canvas5](https://github.com/uin-unit/docs-html/blob/main/images/canvas5.png)

Contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World", 10, 50);
</script>
```

**Teks Stroke**

![canvas6](https://github.com/uin-unit/docs-html/blob/main/images/canvas6.png)

Contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.strokeText("Hello World", 10, 50);
</script>
```

**Menggambar Gradien Linier**

![canvas7](https://github.com/uin-unit/docs-html/blob/main/images/canvas7.png)

Contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createLinearGradient(0, 0, 200, 0);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
</script>
```

**Menggambar Gradien Melingkar**

![canvas8](https://github.com/uin-unit/docs-html/blob/main/images/canvas8.png)

Contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
</script>
```

**Menggambar Gambar**

Contoh : 
```sh
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var img = document.getElementById("scream");
ctx.drawImage(img, 10, 10);
</script>
```
