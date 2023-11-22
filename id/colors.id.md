---
title: "colors"
date : 2023-11-22
draft: true
---
# Warna HTML
Warna HTML ditentukan dengan nama warna yang telah ditentukan sebelumnya, atau dengan nilai RGB, HEX, HSL, RGBA, atau HSLA.
## Nama Warna
Dalam HTML, suatu warna dapat ditentukan dengan menggunakan nama warna:

![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors.png)

## Warna latar belakang
Anda dapat mengatur warna latar belakang untuk elemen HTML:
## Hello World
### Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.
Contoh : 
``` sh
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p>
```
## Warna teks
Anda dapat mengatur warna teks:
## Hello World
Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.
Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.
Contoh : 
``` sh
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p>
```
## Warna Perbatasan
Anda dapat mengatur warna batas:
Hello World
Hello World
Hello World
Contoh : 
``` sh
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1>
```
Nilai Warna
Dalam HTML, warna juga dapat ditentukan menggunakan nilai RGB, nilai HEX, nilai HSL, nilai RGBA, dan nilai HSLA.
Tiga elemen <div> berikut memiliki warna latar belakang yang diatur dengan nilai RGB, HEX, dan HSL:
rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)

Dua elemen `<div>` berikut memiliki warna latar belakangnya yang diatur dengan nilai RGBA dan HSLA, yang menambahkan saluran Alpha ke warnanya (di sini kita memiliki transparansi 50%):
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%202.png)

Contoh : 
``` sh
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>
```
## RGB
Nilai warna RGB mewakili sumber cahaya MERAH, HIJAU, dan BIRU.
Nilai warna RGBA merupakan perpanjangan dari RGB dengan saluran Alpha (opacity).

## Nilai Warna RGB
Dalam HTML, suatu warna dapat ditentukan sebagai nilai RGB, menggunakan rumus ini:
rgb (merah, hijau, biru)
Setiap parameter (merah, hijau, dan biru) menentukan intensitas warna dengan nilai antara 0 dan 255.
Artinya ada 256 x 256 x 256 = 16777216 kemungkinan warna!
Misalnya, rgb(255, 0, 0) ditampilkan dengan warna merah, karena merah disetel ke nilai tertingginya (255), dan dua lainnya (hijau dan biru) disetel ke 0.
Contoh lainnya, rgb(0, 255, 0) ditampilkan dengan warna hijau, karena hijau disetel ke nilai tertingginya (255), dan dua lainnya (merah dan biru) disetel ke 0.
Untuk menampilkan warna hitam, atur semua parameter warna ke 0, seperti ini: rgb(0, 0, 0).
Untuk menampilkan warna putih, atur semua parameter warna ke 255, seperti ini: rgb(255, 255, 255).
Bereksperimenlah dengan mencampurkan nilai RGB di bawah ini:

![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%203.png)
Contoh : 
rgb(255, 0, 0)
rgb(0, 0, 255)
rgb(60, 179, 113)
rgb(238, 130, 238)
rgb(255, 165, 0)
rgb(106, 90, 205)
## Bayangan abu-abu
Nuansa abu-abu sering kali ditentukan menggunakan nilai yang sama untuk ketiga parameter:
Contoh : 
rgb(60, 60, 60)
rgb(100, 100, 100)
rgb(140, 140, 140)
rgb(180, 180, 180)
rgb(200, 200, 200)
rgb(240, 240, 240)


## Nilai Warna RGBA
Nilai warna RGBA merupakan perpanjangan dari nilai warna RGB dengan saluran Alpha - yang menentukan opasitas suatu warna.
Nilai warna RGBA ditentukan dengan:
rgba(merah, hijau, biru, alfa)
Parameter alpha adalah angka antara 0,0 (sepenuhnya transparan) dan 1,0 (tidak transparan sama sekali):
Bereksperimenlah dengan mencampurkan nilai RGBA di bawah ini:
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%204.png)
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%205.png)
## HEX
Warna heksadesimal ditentukan dengan: #RRGGBB, dimana bilangan bulat heksadesimal RR (merah), GG (hijau) dan BB (biru) menentukan komponen warna.


## Nilai Warna HEX
Dalam HTML, suatu warna dapat ditentukan menggunakan nilai heksadesimal dalam bentuk:
#rrggbb
Dimana rr (merah), gg (hijau) dan bb (biru) merupakan nilai heksadesimal antara 00 dan ff (sama dengan desimal 0-255).
Misalnya, #ff0000 ditampilkan dengan warna merah, karena merah disetel ke nilai tertingginya (ff), dan dua lainnya (hijau dan biru) disetel ke 00.
Contoh lainnya, #00ff00 ditampilkan dengan warna hijau, karena hijau disetel ke nilai tertingginya (ff), dan dua lainnya (merah dan biru) disetel ke 00.
Untuk menampilkan warna hitam, atur semua parameter warna ke 00, seperti ini: #000000.
Untuk menampilkan warna putih, atur semua parameter warna ke ff, seperti ini: #ffffff.
Bereksperimenlah dengan mencampurkan nilai HEX di bawah ini:
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%206.png)
Contoh : 
#ff0000
#0000ff
#3cb371
#ee82ee
#ffa500
#6a5acd


## Bayangan abu-abu
Nuansa abu-abu sering kali ditentukan menggunakan nilai yang sama untuk ketiga parameter:
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%207.png)
## HSL
HSL adalah singkatan dari hue, saturation, dan lightness.
Nilai warna HSLA merupakan perpanjangan dari HSL dengan saluran Alpha (opacity).


## Nilai Warna HSL
Dalam HTML, suatu warna dapat ditentukan menggunakan hue, saturation, dan lightness (HSL) dalam bentuk:
hsl(rona, saturasi, kecerahan)
Hue adalah derajat pada roda warna dari 0 hingga 360. 0 berwarna merah, 120 berwarna hijau, dan 240 berwarna biru.
Saturasi adalah nilai persentase. 0% berarti warna abu-abu, dan 100% berarti warna penuh.
Ringan juga merupakan nilai persentase. 0% berwarna hitam, dan 100% berwarna putih.
Bereksperimenlah dengan mencampurkan nilai HSL di bawah ini:
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%208.png)
Example
hsl(0, 100%, 50%)
hsl(240, 100%, 50%)
hsl(147, 50%, 47%)
hsl(300, 76%, 72%)
hsl(39, 100%, 50%)
hsl(248, 53%, 58%)


## Kejenuhan
Saturasi dapat digambarkan sebagai intensitas suatu warna.
100% adalah warna murni, tidak ada corak abu-abu.
50% adalah 50% abu-abu, namun Anda masih dapat melihat warnanya.
0% seluruhnya berwarna abu-abu; kamu tidak dapat lagi melihat warnanya.
Contoh : 
hsl(0, 100%, 50%)
hsl(0, 80%, 50%)
hsl(0, 60%, 50%)
hsl(0, 40%, 50%)
hsl(0, 20%, 50%)
hsl(0, 0%, 50%)
## Kecerahan
Kecerahan suatu warna dapat digambarkan sebagai seberapa banyak cahaya yang ingin diberikan pada warna tersebut, dimana 0% berarti tidak ada cahaya (hitam), 50% berarti 50% terang (tidak gelap dan tidak terang), dan 100% berarti kecerahan penuh (putih). 

![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%209.png)
## Bayangan abu-abu
Nuansa abu-abu sering kali ditentukan dengan mengatur rona dan saturasi ke 0, dan menyesuaikan kecerahan dari 0% hingga 100% untuk mendapatkan nuansa yang lebih gelap/terang:
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%2010.png)
## Nilai Warna HSLA
Nilai warna HSLA merupakan perpanjangan dari nilai warna HSL, dengan saluran Alpha - yang menentukan opasitas suatu warna.
Nilai warna HSLA ditentukan dengan:
hsla(rona, saturasi, kecerahan, alfa)
Parameter alpha adalah angka antara 0,0 (sepenuhnya transparan) dan 1,0 (tidak transparan sama sekali):
Bereksperimenlah dengan mencampurkan nilai HSLA di bawah ini:
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%2011.png)
![arkan](https://github.com/uin-unit/docs-html/blob/main/images/colors%2012.png)
