---
title: Basic
date : 2023-09-22T10:28:51+07:00
draft: true
---

# HTML BASIC

## Dokumen HTML

Semua dokumen HTML harus diawali dengan deklarasi tipe dokumen: `<!DOCTYPE html>`.

Dokumen HTML sendiri diawali dengan `<html>` dan diakhiri dengan `</html>`.

Bagian dokumen HTML yang terlihat berada di antara `<body>` dan `</body>`.

Contoh : 
```sh
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

## Deklarasi `<!DOCTYPE>`

Deklarasi `<!DOCTYPE>` mewakili tipe dokumen, dan membantu browser menampilkan halaman web dengan benar.

Itu hanya boleh muncul sekali, di bagian atas halaman (sebelum tag HTML apa pun).

Deklarasi `<!DOCTYPE>` tidak membedakan huruf besar-kecil.

Deklarasi `<!DOCTYPE>` untuk HTML5 adalah:

``` sh <!DOCTYPE html>```

## Judul HTML

Judul HTML didefinisikan dengan tag `<h1>` hingga `<h6>`.

`<h1>` mendefinisikan judul yang paling penting. `<h6>` mendefinisikan judul yang paling tidak penting:
Contoh : 
  
```sh
<h1>This is heading 1</h1>
```

```sh
<h2>This is heading 2</h2>
```

```sh
<h3>This is heading 3</h3>
```

## Paragraf HTML

Paragraf HTML didefinisikan dengan tag `<p>`:

Contoh : 
```sh
<p>This is a paragraph.</p>
```
```sh
<p>This is another paragraph.</p>
```

## Tautan HTML

Tautan HTML ditentukan dengan tag `<a>`:

Contoh : 
```sh
<a href="https://www.w3schools.com">This is a link</a>
```

Tujuan tautan ditentukan dalam atribut href

Atribut digunakan untuk memberikan informasi tambahan tentang elemen HTML.

## Gambar HTML

Gambar HTML didefinisikan dengan tag `<img>`.

File sumber (src), teks alternatif (alt), lebar, dan tinggi disediakan sebagai atribut:

Contoh
```sh
<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">
```

## Cara Melihat Sumber HTML

Pernahkah Anda melihat halaman Web dan bertanya-tanya, "Hei! Bagaimana mereka melakukan itu?"

Lihat Kode Sumber HTML:

Klik CTRL + U di halaman HTML, atau klik kanan pada halaman dan pilih "Lihat Sumber Halaman". Ini akan membuka tab baru yang berisi kode sumber HTML halaman tersebut.
Periksa Elemen HTML:

Klik kanan pada sebuah elemen (atau area kosong), dan pilih "Periksa" untuk melihat terdiri dari elemen apa (Anda akan melihat HTML dan CSS). Anda juga dapat mengedit HTML atau CSS dengan cepat di panel Elemen atau Gaya yang terbuka.


