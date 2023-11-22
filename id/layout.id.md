---
title: "Layout"
date : 2023-10-22
draft: true
---

# Elemen dan Teknik Tata Letak HTML

Situs web sering kali menampilkan konten dalam beberapa kolom (seperti majalah atau koran).
![layout](https://github.com/uin-unit/docs-html/blob/main/images/layout.png)

## Elemen Tata Letak HTML

HTML memiliki beberapa elemen semantik yang mendefinisikan berbagai bagian halaman web:

![layout2](https://github.com/uin-unit/docs-html/blob/main/images/layout2.gif)

- `header> -` Mendefinisikan header untuk dokumen atau bagian
- `<nav> -` Mendefinisikan sekumpulan tautan navigasi
- `<section> -` Mendefinisikan bagian dalam dokumen
- `<artikel> -` Mendefinisikan konten independen dan mandiri
- `<aside> -` Mendefinisikan konten selain konten (seperti sidebar)
- `<footer> -` Mendefinisikan footer untuk dokumen atau bagian
- `<details> -` Mendefinisikan detail tambahan yang dapat dibuka dan ditutup oleh pengguna sesuai permintaan
- `<ringkasan> -` Mendefinisikan judul untuk elemen `<details>`

Anda dapat membaca lebih lanjut tentang elemen semantik di bab Semantik HTML kami.

## Teknik Tata Letak HTML

Ada empat teknik berbeda untuk membuat tata letak multikolom. Setiap teknik memiliki kelebihan dan kekurangannya:

- kerangka CSS
- Properti mengambang CSS
- kotak fleksibel CSS
- kisi CSS

## Kerangka CSS

Jika Anda ingin membuat layout dengan cepat, Anda dapat menggunakan framework CSS, seperti W3.CSS atau Bootstrap.
Tata Letak Mengambang CSS
Merupakan hal yang umum untuk melakukan seluruh tata letak web menggunakan properti float CSS. Float mudah dipelajari - Anda hanya perlu mengingat cara kerja properti float dan clear. Kekurangan: Elemen mengambang terikat pada alur dokumen, sehingga dapat mengganggu fleksibilitas. Pelajari lebih lanjut tentang float di bab CSS Float dan Clear kami
![layout3](https://github.com/uin-unit/docs-html/blob/main/images/layout3.png)

## Tata Letak Kotak Fleksibel CSS

Penggunaan flexbox memastikan bahwa elemen berperilaku dapat diprediksi ketika tata letak halaman harus mengakomodasi ukuran layar yang berbeda dan perangkat tampilan yang berbeda.

![layout4](https://github.com/uin-unit/docs-html/blob/main/images/layout4.png)

## Tata Letak Kotak CSS

Modul Tata Letak Grid CSS menawarkan sistem tata letak berbasis grid, dengan baris dan kolom, sehingga memudahkan mendesain halaman web tanpa harus menggunakan float dan positioning.
