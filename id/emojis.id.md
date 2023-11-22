---
title: Emojis
date : 2023-09-22T10:28:51+07:00
draft: true
---

### Menggunakan Emoji dalam HTML


![emoji](https://github.com/uin-unit/docs-html/blob/main/images/emoji1.png)
![emoji](https://github.com/uin-unit/docs-html/blob/main/images/emoji2.png)
![emoji](https://github.com/uin-unit/docs-html/blob/main/images/emoji3.png)


### Apa itu Emoji?
Emoji terlihat seperti gambar, atau ikon, padahal sebenarnya tidak.
Itu adalah huruf (karakter) dari kumpulan karakter UTF-8 (Unicode).
### Atribut rangkaian karakter HTML
Untuk menampilkan halaman HTML dengan benar, browser web harus mengetahui kumpulan karakter yang digunakan di halaman tersebut.
Ini ditentukan dalam tag `<meta>`:
`<meta charset="UTF-8">`
### Karakter UTF-8
Banyak karakter UTF-8 yang tidak dapat diketik pada keyboard, namun selalu dapat ditampilkan menggunakan angka (disebut nomor entitas):
A adalah 65
B adalah 66
C adalah 67
Contoh : 
`<!DOCTYPE html>
<html>
<meta charset="UTF-8">
<body>

<p>I will display A B C</p>
<p>I will display &#65; &#66; &#67;</p>

</body>
</html>`
Contoh Dijelaskan
Elemen `<meta charset="UTF-8">` mendefinisikan kumpulan karakter.
Karakter A, B, dan C ditampilkan dengan angka 65, 66, dan 67.
