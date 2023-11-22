---
title: HTML versus XHTML
date : 2023-09-22T10:28:51+07:00
draft: true
---

# HTML versus XHTML

XHTML adalah versi HTML yang lebih ketat dan berbasis XML.

### Apa itu XHTML?

XHTML adalah singkatan dari EXtensible HyperText Markup Language

XHTML adalah versi HTML yang lebih ketat dan berbasis XML

XHTML adalah HTML yang didefinisikan sebagai aplikasi XML

XHTML didukung oleh semua browser utama

### Mengapa XHTML?
XML adalah bahasa markup di mana semua dokumen harus diberi markup dengan benar (berbentuk "baik").

XHTML dikembangkan untuk membuat HTML lebih dapat diperluas dan fleksibel untuk bekerja dengan format data lain (seperti XML). Selain itu, browser mengabaikan kesalahan pada halaman HTML, dan mencoba menampilkan situs web meskipun ada beberapa kesalahan dalam markupnya. Jadi XHTML hadir dengan penanganan kesalahan yang jauh lebih ketat.

Jika Anda ingin mempelajari XML, silakan baca Tutorial XML kami.

Perbedaan Paling Penting dari HTML

`<!DOCTYPE>` adalah wajib

Atribut xmlns di `<html>` bersifat wajib

`<html>`, `<head>`, `<title>`, dan `<body>` adalah wajib
  
Elemen harus selalu disarangkan dengan benar

Elemen harus selalu tertutup

Elemen harus selalu menggunakan huruf kecil

Nama atribut harus selalu menggunakan huruf kecil

Nilai atribut harus selalu dikutip

Minimalkan atribut dilarang

XHTML - `<!DOCTYPE ....>` Wajib

Dokumen XHTML harus memiliki deklarasi XHTML `<!DOCTYPE>`.

Elemen `<html>`, `<head>`, `<title>`, dan `<body>` juga harus ada, dan atribut xmlns di `<html>` harus menentukan namespace xml untuk dokumen tersebut.

Contoh : 

Berikut ini adalah dokumen XHTML dengan minimal tag yang diperlukan:
```sh 
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN"
"http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <title>Title of document</title>
</head>
<body>

  some content here...

</body>
</html>
```

Elemen XHTML harus disarangkan dengan benar

Dalam XHTML, elemen harus selalu disarangkan dengan benar satu sama lain, seperti ini:

Correct:

`<b><i>Some text</i></b>`

Wrong:

`<b><i>Some text</b></i>`

Elemen XHTML Harus Selalu Tertutup

Di XHTML, elemen harus selalu tertutup, seperti ini:

Correct:

`<p>This is a paragraph</p>`

`<p>This is another paragraph</p>`

Wrong:

`<p>This is a paragraph`

`<p>This is another paragraph`

  
Elemen Kosong XHTML Harus Selalu Tertutup

Di XHTML, elemen kosong harus selalu ditutup, seperti ini:

Correct:

A break: `<br />`

A horizontal rule: `<hr />`

An image: `<img src="happy.gif" alt="Happy face" />`

Wrong:

A break: `<br>`

A horizontal rule: `<hr>`

An image: `<img src="happy.gif" alt="Happy face">`

Elemen XHTML Harus dalam Huruf Kecil

Di XHTML, nama elemen harus selalu menggunakan huruf kecil, seperti ini:

Correct:
`
<body>
<p>This is a paragraph</p>
</body>
```

Wrong:
```sh 
<BODY>
<P>This is a paragraph</P>
</BODY>
```
Nama Atribut XHTML Harus dalam Huruf Kecil

Di XHTML, nama atribut harus selalu menggunakan huruf kecil, seperti ini:


Correct:

`<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>`

Wrong:

`<a HREF="https://www.w3schools.com/html/">Visit our HTML tutorial</a>`


Nilai Atribut XHTML Harus Dikutip

Dalam XHTML, nilai atribut harus selalu diberi tanda kutip, seperti ini:

Correct:

`<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>`

Wrong:

`<a href=https://www.w3schools.com/html/>Visit our HTML tutorial</a>`

Minimisasi Atribut XHTML Dilarang

Di XHTML, minimalisasi atribut dilarang:
```
Correct:

`<input type="checkbox" name="vehicle" value="car" checked="checked" />`
`<input type="text" name="lastname" disabled="disabled" />`

Wrong:

`<input type="checkbox" name="vehicle" value="car" checked />`
`<input type="text" name="lastname" disabled />`
```
