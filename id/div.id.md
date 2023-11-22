---
title: "DIV"
date : 2023-11-22
draft: true
---

# Elemen Div HTML

Elemen `<div>` digunakan sebagai wadah untuk elemen HTML lainnya.

## Elemen `<div>`

Elemen `<div>` secara default merupakan elemen blok, yang berarti elemen ini mengambil semua lebar yang tersedia, dan dilengkapi dengan jeda baris sebelum dan sesudahnya.

Contoh :
Elemen <div> menggunakan semua lebar yang tersedia:

```sh
Lorem Ipsum <div>I am a div</div> dolor sit amet.
```

Elemen <div> tidak memiliki atribut yang diperlukan, tetapi style, kelas, dan id adalah hal yang umum.

## `<div>` sebagai sebuah wadah

Elemen `<div>` sering digunakan untuk mengelompokkan bagian dari halaman web.

Contoh :
Elemen `<div>` dengan elemen HTML:

```sh
<div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>
```

## Meratakan rata tengah sebuah elemen `<div>`

Jika Anda memiliki elemen <div> yang lebarnya tidak 100%, dan Anda ingin meratakannya di tengah, atur properti margin CSS ke otomatis.

Contoh :
```sh
<style>
div {
  width:300px;
  margin:auto;
}
</style>
```

## Beberapa elemen <div>

Anda dapat memiliki banyak wadah `<div>` pada halaman yang sama.

Contoh :
```sh
<div>
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>

<div>
  <h2>Oslo</h2>
  <p>Oslo is the capital city of Norway.</p>
  <p>Oslo has over 600.000 inhabitants.</p>
</div>

<div>
  <h2>Rome</h2>
  <p>Rome is the capital city of Italy.</p>
  <p>Rome has almost 3 million inhabitants.</p>
</div>
```
## Menyelaraskan elemen `<div>` secara berdampingan

Saat membuat halaman web, Anda sering kali ingin memiliki dua atau lebih elemen `<div>` yang berdampingan, seperti ini:

![div1](https://github.com/uin-unit/docs-html/blob/main/images/div1.png)

Ada beberapa metode berbeda untuk menyelaraskan elemen secara berdampingan, semuanya mencakup beberapa gaya CSS. Kita akan melihat metode yang paling umum:

## Float

Properti float CSS pada awalnya tidak dimaksudkan untuk menyelaraskan elemen `<div>` secara berdampingan, tetapi telah digunakan untuk tujuan ini selama bertahun-tahun.

Properti float CSS digunakan untuk memposisikan dan memformat konten dan memungkinkan elemen mengambang di samping satu sama lain, bukan di atas satu sama lain.

Contoh :
Cara menggunakan float untuk menyelaraskan elemen div secara berdampingan:

Contoh :
```sh
<style>
.mycontainer {
  width:100%;
  overflow:auto;
}
.mycontainer div {
  width:33%;
  float:left;
}
</style>
```

## Inline-block

Jika Anda mengubah properti tampilan elemen `<div>` dari blok menjadi blok sebaris, elemen `<div>` tidak akan lagi menambahkan jeda baris sebelum dan sesudahnya, dan akan ditampilkan secara berdampingan, bukan di atas satu sama lain.

Contoh :
Cara menggunakan tampilan: blok sebaris untuk menyelaraskan elemen div secara berdampingan:
```sh
<style>
div {
  width: 30%;
  display: inline-block;
}
</style>
```

## Flex

Modul Tata Letak CSS Flexbox diperkenalkan untuk mempermudah mendesain struktur tata letak responsif yang fleksibel tanpa menggunakan float atau pemosisian.

Untuk membuat metode flex CSS berfungsi, kelilingi elemen `<div>` dengan elemen `<div>` lain dan berikan status sebagai wadah flex.

Contoh :
Cara menggunakan flex untuk menyelaraskan elemen div secara berdampingan:
```sh
<style>
.mycontainer {
  display: flex;
}
.mycontainer > div {
  width:33%;
}
</style>
```

## Grid

Modul Tata Letak Grid CSS menawarkan sistem tata letak berbasis grid, dengan baris dan kolom, sehingga lebih mudah untuk mendesain halaman web tanpa harus menggunakan float dan pemosisian.

Kedengarannya hampir sama dengan flex, tetapi memiliki kemampuan untuk menentukan lebih dari satu baris dan memposisikan setiap baris satu per satu.

Metode grid CSS mengharuskan Anda mengelilingi elemen `<div>` dengan elemen `<div>` lain dan memberikan status sebagai wadah grid, dan Anda harus menentukan lebar setiap kolom.

Contoh : 
Cara menggunakan kisi untuk menyelaraskan elemen `<div>` secara berdampingan:
```sh
<style>
.grid-container {
  display: grid;
  grid-template-columns: 33% 33% 33%;
}
</style>
```

## Tag HTML

| Tag  | Deskripsi |
| ----------- | ----------- |
| `<div>` | Menentukan bagian dalam dokumen (tingkat blok) |

