---
title: "list"
date : 2023-10-22
draft: true
---
# DAFTAR HTML

Daftar HTML memungkinkan pengembang web mengelompokkan sekumpulan item terkait dalam daftar.
Contoh : 

An unordered HTML list:

- Item
- Item
- Item
- Item

An ordered HTML list:

1. First item
2. Second item
3. Third item
4. Fourth item

## Daftar HTML tidak berurutan

Daftar tidak berurutan dimulai dengan `<ul>`tag. Setiap item daftar dimulai dengan `<li>`tag.
Item daftar akan ditandai dengan poi`<ul>`


```sh
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

n (lingkaran hitam kecil) secara default:

Contoh :

## Daftar HTML yang dipesan

Daftar yang diurutkan dimulai dengan `<ol>`tag. Setiap item daftar dimulai dengan `<li>`tag.
Item daftar akan ditandai dengan angka secara default:

Contoh : 

```sh
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
## Daftar Deskripsi HTML

HTML juga mendukung daftar deskripsi.

Daftar deskripsi adalah daftar istilah, dengan deskripsi setiap istilah.
Tag `<dl>`mendefinisikan daftar deskripsi, `<dt>`tag mendefinisikan istilah (nama), dan `<dd>` tag menjelaskan setiap istilah:

Contoh : 

```sh
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
![list-html](https://github.com/uin-unit/docs-html/blob/main/images/list-html.png)
## Daftar Tidak Berurutan HTML

Tag HTML `<ul>` mendefinisikan daftar tidak berurutan (berpoin).

Daftar tidak berurutan dimulai dengan tag `<ul>`. Setiap item daftar dimulai dengan tag `<li>`.
Item daftar akan ditandai dengan poin (lingkaran hitam kecil) secara default:

contoh :

```sh
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
## Daftar HTML Tidak Berurutan - Pilih Penanda Item Daftar

Properti tipe gaya daftar CSS digunakan untuk menentukan gaya penanda item daftar. Itu dapat memiliki salah satu dari nilai berikut:

Deskripsi Nilai

disc Menyetel penanda item daftar ke poin (default)
lingkaran Menyetel penanda item daftar ke lingkaran
square Menyetel penanda item daftar menjadi persegi
none Item daftar tidak akan ditandai

Contoh :  - Disc

```sh
<ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
Contoh :  - Circle
```sh
<ul style="list-style-type:circle;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
Contoh :  - Square
```sh
<ul style="list-style-type:square;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
Contoh :  - None
```sh<ul style="list-style-type:none;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

## Daftar HTML Bersarang

Daftar dapat disarangkan (daftar di dalam daftar):
Contoh : 
```sh
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```
Catatan: Item daftar (`<li>`) dapat berisi daftar baru, dan elemen HTML lainnya, seperti gambar dan tautan, dll.

## Daftar Horisontal dengan CSS

Daftar HTML dapat ditata dengan berbagai cara dengan CSS.
Salah satu cara yang populer adalah menata daftar secara horizontal, untuk membuat menu navigasi:

Contoh : 
```sh
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #111111;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
Ringkasan Bab

- Gunakan elemen HTML `<ul>` untuk mendefinisikan daftar tidak berurutan
- Gunakan properti tipe gaya daftar CSS untuk menentukan penanda item daftar
- Gunakan elemen HTML `<li>` untuk mendefinisikan item daftar
- Daftar dapat disarangkan
- Item daftar dapat berisi elemen HTML lainnya
- Gunakan properti CSS float:left untuk menampilkan daftar secara horizontal

![list-html2](https://github.com/uin-unit/docs-html/blob/main/images/list-html2.png)

# Daftar Urutan HTML

Tag HTML <ol> mendefinisikan daftar yang diurutkan. Daftar yang diurutkan dapat berupa angka atau abjad.

## Daftar HTML yang dipesan

Daftar yang diurutkan dimulai dengan tag <ol>. Setiap item daftar dimulai dengan tag <li>.
Item daftar akan ditandai dengan angka secara default:
Contoh : 
```sh
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
## Daftar HTML yang Diurutkan - Atribut Tipe

Atribut type dari tag `<ol>`, mendefinisikan tipe penanda item daftar:
![list-html3](https://github.com/uin-unit/docs-html/blob/main/images/list-html3.png)

Numbers:
```sh
<ol type="1">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
Uppercase Letters:
```sh
<ol type="A">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
Lowercase Letters:
```sh
<ol type="a">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
Uppercase Roman Numbers:
```sh
<ol type="I">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
```
Lowercase Roman Numbers:
```sh
<ol type="i">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
## Penghitungan Daftar Kontrol

Secara default, daftar yang diurutkan akan mulai menghitung dari 1. Jika Anda ingin mulai menghitung dari angka tertentu, Anda dapat menggunakan atribut start:
Contoh : 
```sh
<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
## Daftar HTML Bersarang

Daftar dapat disarangkan (daftar di dalam daftar):
Contoh : 
```sh
<ol>
  <li>Coffee</li>
  <li>Tea
    <ol>
      <li>Black tea</li>
      <li>Green tea</li>
    </ol>
  </li>
  <li>Milk</li>
</ol>
```
