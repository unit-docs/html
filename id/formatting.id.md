---
title: "formatting"
date : 2023-11-22
draft: true
---

# Pemformatan Teks HTML

HTML berisi beberapa elemen untuk mendefinisikan teks dengan arti khusus.

Contoh : 

**This text is bold**

*This text is italic*

this is `<sub>` subscript `</sub>` and `<sup>` superscript `</sup>`
     

### Elemen Pemformatan HTML

Elemen pemformatan dirancang untuk menampilkan jenis teks khusus:

| tag | deskripsi |
| ----------- | ----------- |
| `<b>` | Teks tebal |
| `<strong>` | Teks penting |
| `<i>` | Teks miring |
| `<em>` | Teks yang ditekankan |
| `<mark>` | Teks yang ditandai |
| `<small>` | Teks lebih kecil |
| `<del>` | Teks yang dihapus |
| `<ins>` | Teks yang disisipkan |
| `<sub>` | Teks subskrip |
| `<sup>` | Teks superskrip |



### Elemen HTML `<b>` dan `<strong>`

Elemen HTML `<b>` mendefinisikan teks tebal, tanpa hal penting apa pun.

Contoh : 
```sh 
<b>This text is bold</b>
```


Elemen HTML `<strong>` mendefinisikan teks dengan sangat penting. Konten di dalamnya biasanya ditampilkan dalam huruf tebal.

Contoh : 

```sh 
<strong>This text is important!</strong>
```

### Elemen HTML `<i>` dan `<em>`

Elemen HTML `<i>` mendefinisikan bagian teks dalam suara atau suasana hati alternatif. Konten di dalamnya biasanya ditampilkan dalam huruf miring.

Tip: Tag `<i>` sering digunakan untuk menunjukkan istilah teknis, frasa dari bahasa lain, pemikiran, nama kapal, dll.

Contoh : 
```sh 
<i>This text is italic</i>
```



Elemen HTML `<em>` mendefinisikan teks yang ditekankan. Konten di dalamnya biasanya ditampilkan dalam huruf miring.

Tips: Pembaca layar akan mengucapkan kata dalam `<em>` dengan penekanan, menggunakan tekanan verbal.

Contoh : 
```sh 
<em>This text is emphasized</em>
```


### Elemen HTML `<small>`

Elemen HTML `<small>` mendefinisikan teks yang lebih kecil:

Contoh : 
```sh 
<small>This is some smaller text.</small>
```


### Elemen `<mark>` HTML

Elemen HTML `<mark>` mendefinisikan teks yang harus ditandai atau disorot:

Contoh : 
```sh 
<p>Do not forget to buy <mark>milk</mark> today.</p>
```


### Elemen HTML `<del>`

Elemen HTML `<del>` mendefinisikan teks yang telah dihapus dari dokumen. Browser biasanya akan membuat garis pada teks yang dihapus:

Contoh : 
```sh 
<p>My favorite color is <del>blue</del> red.</p>
```


### Elemen HTML `<ins>`

Elemen HTML `<ins>` mendefinisikan teks yang telah dimasukkan ke dalam dokumen. Browser biasanya akan menggarisbawahi teks yang disisipkan:

Contoh : 
```sh 
<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
```

### Elemen `<sub>` HTML

Elemen HTML `<sub>` mendefinisikan teks subskrip. Teks subskrip muncul setengah karakter di bawah garis normal, dan terkadang ditampilkan dalam font yang lebih kecil. Teks subskrip dapat digunakan untuk rumus kimia, seperti H2O:

Contoh : 
```sh 
<p>This is <sub>subscripted</sub> text.</p>
```


### Elemen `<sup>` HTML

Elemen HTML <sup> mendefinisikan teks superskrip. Teks superskrip muncul setengah karakter di atas garis normal, dan terkadang ditampilkan dalam font yang lebih kecil. Teks superskrip dapat digunakan untuk catatan kaki, seperti WWW[1]:
Contoh : 
```sh 
<p>This is <sup>superscripted</sup> text.</p>
```


