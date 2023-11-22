---
title: "Block & Inline"
date : 2023-11-22
draft: true
---

# Blok HTML dan Elemen Sebaris

Setiap elemen HTML memiliki nilai tampilan default, bergantung pada jenis elemennya.

Ada dua nilai tampilan: blok dan sebaris.

## Elemen Tingkat Blok

Elemen tingkat blok selalu dimulai pada baris baru, dan browser secara otomatis menambahkan beberapa spasi (margin) sebelum dan sesudah elemen.

Elemen tingkat blok selalu menempati seluruh lebar yang tersedia (meregangkan ke kiri dan kanan sejauh mungkin).

Dua elemen blok yang umum digunakan adalah: `<p>` dan `<div>`.

Elemen `<p>` mendefinisikan paragraf dalam dokumen HTML.

Elemen `<div>` mendefinisikan divisi atau bagian dalam dokumen HTML.

Elemen `<p>` adalah elemen tingkat blok.

Elemen `<div>` adalah elemen tingkat blok.


Contoh : 

```sh
<p>Hello World</p>
<div>Hello World</div>
```

Berikut adalah elemen tingkat blok dalam HTML:

```sh
<address> <article> <aside> <aside> <blockquote> <canvas> <dd>
<div> <dl> <dt> <fieldset> <figcaption>  <figure> <footer>
<form> <h1> <h6> <header> <hr> <li> <main>
<nav> <noscript> <ol> <p> <pre> <section> <table>
<tfoot> <ul> <video>
```

## Elemen Sebaris

Elemen sebaris tidak dimulai pada baris baru.

Elemen sebaris hanya membutuhkan lebar sebanyak yang diperlukan.

Ini adalah elemen <span> di dalam paragraf.

Contoh : 

`<span>Hello World</span>`

Berikut adalah elemen inline dalam HTML:

```sh
<a> <abbr> <acronym> <b> <bdo> <big> <br>
<button> <cite> <code> <dfn> <em> <i> <img>
<input> <kbd> <label> <map> <object> <output> <q>
<samp> <script> <select> <small> <span> <strong> <sub>
<sup> <textarea> <time> <tt> <var>
```

Catatan: Elemen sebaris tidak boleh berisi elemen tingkat blok!


## Elemen `<div>`
Elemen tersebut `<div>` sering digunakan sebagai wadah untuk elemen HTML lainnya.

Elemen tersebut `<div>` tidak memiliki atribut yang diperlukan, tetapi style, class dan id bersifat umum.

Ketika digunakan bersama dengan CSS, `<div>` elemen tersebut dapat digunakan untuk menata blok konten:

Contoh : 

```sh
<div style="background-color:black;color:white;padding:20px;">
  <h2>London</h2>
  <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
</div>
```


## Elemen `<span>`

Elemen `<span>` adalah wadah sebaris yang digunakan untuk menandai bagian teks, atau bagian dokumen.

Elemen tersebut `<span>` tidak memiliki atribut yang diperlukan, tetapi style, classdan idbersifat umum.

Ketika digunakan bersama dengan CSS, <span>elemen tersebut dapat digunakan untuk menata bagian teks:


Contoh :
```sh
<p>My mother has <span style="color:blue;font-weight:bold;">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold;">dark green</span> eyes.</p>
```

## Ringkasan Bab

- Ada dua nilai tampilan: blok dan sebaris

- Elemen tingkat blok selalu dimulai pada baris baru dan menggunakan lebar penuh yang tersedia

- Elemen sebaris tidak dimulai pada baris baru dan hanya menggunakan lebar sebanyak yang diperlukan

- Elemen ini `<div>` merupakan level blok dan sering digunakan sebagai wadah untuk elemen HTML lainnya

- Elemen `<span>` adalah wadah sebaris yang digunakan untuk menandai bagian teks, atau bagian dokumen

## Tag HTML

| Tag | Deskripsi |
| ----------- | ----------- |
| `<div>` | Mendefinisikan bagian dalam blok (tingkat blok) |
| `<span>` | Mendefinisikan bagian dalam blok (sebaris) |


