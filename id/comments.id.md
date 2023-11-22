---
title: "comments"
date : 2023-11-22
draft: true
---

# HTML Comments
Komentar HTML tidak ditampilkan di browser, namun dapat membantu mendokumentasikan kode sumber HTML Anda.
## Tag Komentar HTML
Anda dapat menambahkan komentar ke sumber HTML Anda dengan menggunakan sintaks berikut:
``` sh
<!-- Write your comments here -->
```
Perhatikan bahwa ada tanda seru (!) di tag awal, tetapi tidak di tag akhir.
## Tambahkan Komentar
Dengan komentar Anda dapat menempatkan pemberitahuan dan pengingat dalam kode HTML Anda:
Contoh : 
``` sh
<!-- This is a comment -->

<p>This is a paragraph.</p>

<!-- Remember to add more information here -->
```
## Sembunyikan Konten
Komentar dapat digunakan untuk menyembunyikan konten.
Ini dapat berguna jika Anda menyembunyikan konten untuk sementara:
Contoh : 
``` sh
<p>This is a paragraph.</p>

<!-- <p>This is another paragraph </p> -->

<p>This is a paragraph too.</p>
```
Anda juga dapat menyembunyikan lebih dari satu baris. Segala sesuatu di antara <!-- dan --> akan disembunyikan dari tampilan.
Contoh : 
Menyembunyikan bagian dari kode HTML:
``` sh
<p>This is a paragraph.</p>
<!--
<p>Look at this cool image:</p>
<img border="0" src="pic_trulli.jpg" alt="Trulli">
-->
<p>This is a paragraph too.</p>
```
## Sembunyikan Konten Sebaris
Komentar dapat digunakan untuk menyembunyikan bagian tengah kode HTML.
Contoh : 
Menyembunyikan bagian dari paragraf:
``` sh
<p>This <!-- great text --> is a paragraph.</p>
```
