---
title: "JavaScript"
date : 2023-10-22
draft: true
---

# HTMLJavaScript

JavaScript membuat halaman HTML lebih dinamis dan interaktif.

## Tag `<script>` HTML

Tag HTML `<script>`digunakan untuk mendefinisikan skrip sisi klien (JavaScript).
Elemen tersebut `<script>`berisi pernyataan skrip, atau menunjuk ke file skrip eksternal melalui atribut src.
Kegunaan umum JavaScript adalah manipulasi gambar, validasi formulir, dan perubahan konten dinamis.
Untuk memilih elemen HTML, JavaScript paling sering menggunakan `document.getElementById()`metode ini.
Contoh JavaScript ini menulis "Halo JavaScript!" menjadi elemen HTML dengan id="demo":

Contoh : 
```sh
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```
## Rasa JavaScript

Berikut adalah beberapa contoh apa yang dapat dilakukan JavaScript

Contoh : 
JavaScript dapat mengubah konten:
```sh
document.getElementById("demo").innerHTML = "Hello JavaScript!";
```
Contoh : 
JavaScript dapat mengubah gaya:
```sh
document.getElementById("demo").style.fontSize = "25px";
document.getElementById("demo").style.color = "red";
document.getElementById("demo").style.backgroundColor = "yellow";
```
Contoh : 
JavaScript dapat mengubah atribut:
```sh
document.getElementById("image").src = "picture.gif";
```
## Tag HTML `<noscript>`

Tag HTML `<noscript>`mendefinisikan konten alternatif untuk ditampilkan kepada pengguna yang menonaktifkan skrip di browsernya atau memiliki browser yang tidak mendukung skrip:

Contoh : 
```sh<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript>
```
![JavaScript](https://github.com/uin-unit/docs-html/blob/main/images/javascript.png)

