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
