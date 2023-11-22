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





