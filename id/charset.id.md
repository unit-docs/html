---
title: "charset"
date : 2023-11-22
draft: true
---

# Pengkodean HTML (Kumpulan Karakter)
## Atribut rangkaian karakter HTML
Kumpulan karakter ditentukan dalam tag `<meta>`:

Contoh : 
``` sh
<meta charset="UTF-8">
```
Spesifikasi HTML5 mendorong pengembang web untuk menggunakan rangkaian karakter UTF-8.
UTF-8 mencakup hampir semua karakter dan simbol di dunia!
Referensi UTF-8 Lengkap
## Kumpulan Karakter ASCII
ASCII adalah standar pengkodean karakter pertama untuk web. Ini mendefinisikan 128 karakter berbeda yang dapat digunakan di internet:
- Huruf bahasa Inggris (A-Z)
- Angka (0-9)
- Karakter khusus seperti ! $+-( )@< >.
## Kumpulan Karakter ANSI
ANSI (Windows-1252) adalah kumpulan karakter Windows asli:
- Identik dengan ASCII untuk 127 karakter pertama
- Karakter khusus dari 128 hingga 159
- Identik dengan UTF-8 dari 160 hingga 255
- 
``` sh
<meta charset="Windows-1252">
```
## Kumpulan Karakter ISO-8859-1
ISO-8859-1 adalah kumpulan karakter default untuk HTML 4. Kumpulan karakter ini mendukung 256 kode karakter berbeda. HTML 4 juga mendukung UTF-8.
- Identik dengan ASCII untuk 127 karakter pertama
- Tidak menggunakan karakter dari 128 hingga 159
- Identik dengan ANSI dan UTF-8 dari 160 hingga 255
HTML 4 Contoh : 
```sh
<meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1">
```
HTML 5 Contoh : 
``` sh
<meta charset="ISO-8859-1">
```
## Kumpulan Karakter UTF-8
- identik dengan ASCII untuk nilai dari 0 hingga 127
- Tidak menggunakan karakter dari 128 hingga 159
- Identik dengan ANSI dan 8859-1 dari 160 hingga 255
- Berlanjut dari nilai 256 hingga 10.000 karakter
- 
``` sh
<meta charset="UTF-8">
```
## Perbedaan Antara Kumpulan Karakter
Tabel berikut menampilkan perbedaan antara rangkaian karakter yang dijelaskan di atas:
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%201.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%202.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%203.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%204.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%205.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%206.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%207.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%208.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%209.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%2010.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%2011.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%2012.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%2013.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%2014.png)
![table](https://github.com/uin-unit/docs-html/blob/main/images/pengkodean%2015.png)
