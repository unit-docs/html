---
title: File Path
date : 2023-11-22
draft: true
---

# Jalur File HTML

Jalur file menjelaskan lokasi file dalam struktur folder situs web.

Contoh Jalur File

**Deskripsi Jalur**

`<img src="picture.jpg">` File "picture.jpg" terletak di folder yang sama dengan halaman saat ini

`<img src="images/picture.jpg">` File "picture.jpg" terletak di folder gambar di folder saat ini

`<img src="/images/picture.jpg">` File "picture.jpg" terletak di folder gambar di root web saat ini

`<img src="../picture.jpg">` File "picture.jpg" terletak di folder satu tingkat di atas folder saat ini

### Jalur File HTML

Jalur file menjelaskan lokasi file dalam struktur folder situs web.

Jalur file digunakan saat menautkan ke file eksternal, seperti:

- Halaman web

- Gambar-gambar

- Lembar gaya

- JavaScript

## Jalur File Absolut

Jalur file absolut adalah URL lengkap ke file:

Contoh : 

```sh
<img src="https://www.w3schools.com/images/picture.jpg" alt="Mountain">
```

## Jalur File Relatif

Jalur file relatif menunjuk ke file yang relatif terhadap halaman saat ini.

Dalam contoh berikut, jalur file menunjuk ke file di folder gambar yang terletak di akar web saat ini:

Contoh : 

```sh
<img src="/images/picture.jpg" alt="Mountain">
```

Dalam contoh berikut, jalur file menunjuk ke file di folder gambar yang terletak di folder saat ini:

Contoh : 

```sh
<img src="images/picture.jpg" alt="Mountain">
```

Dalam contoh berikut, jalur file menunjuk ke file di folder gambar yang terletak di folder yang satu tingkat lebih tinggi dari folder saat ini:

Contoh : 

```sh
<img src="../images/picture.jpg" alt="Mountain">
```

## Praktek terbaik

Praktik terbaiknya adalah menggunakan jalur file relatif (jika memungkinkan).


Saat menggunakan jalur file relatif, halaman web Anda tidak akan terikat ke URL dasar Anda saat ini. Semua tautan akan berfungsi di komputer Anda sendiri (localhost) serta di domain publik Anda saat ini dan domain publik Anda di masa mendatang.
