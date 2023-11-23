---
title: "Insert Title"
date : 2023-09-22T10:28:51+07:00
draft: true
---

# Tabel HTML

Tabel HTML memungkinkan pengembang web untuk mengatur data ke dalam baris dan kolom.

![tabel html(1)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(1).png)

## Tentukan Tabel HTML
terdiri dari sel-sel tabel di dalam baris dan kolom.

Contoh : 

Tabel HTML

Tabel dalam HTML sederhana:
```sh
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>
```

## Sel Tabel
Setiap sel tabel ditentukan oleh tag `<td>` dan `</td>`.
td adalah singkatan dari data tabel.
Segala sesuatu di antara `<td>` dan `</td>` adalah isi sel tabel.
Contoh : 
```sh
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```
## Baris Tabel
Setiap baris tabel dimulai dengan tag `<tr>` dan diakhiri dengan tag `</tr>`.
tr singkatan dari baris tabel.
Contoh : 
```sh
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>
```
Anda dapat memiliki baris sebanyak yang Anda suka dalam sebuah tabel; pastikan saja jumlah sel di setiap baris sama.

Catatan: Ada kalanya sebuah baris dapat memiliki sel lebih sedikit atau lebih banyak dibandingkan baris lainnya. Anda akan mempelajarinya di bab selanjutnya.

## Header Tabel
Terkadang Anda ingin sel Anda menjadi sel header tabel. Dalam kasus tersebut gunakan tag `<th>` alih-alih tag `<td>`:

th singkatan dari header tabel.

Contoh : 

Biarkan baris pertama menjadi sel header tabel:
```sh
<table>
  <tr>
    <th>Person 1</th>
    <th>Person 2</th>
    <th>Person 3</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>
```
Secara default, teks dalam elemen <th> dicetak tebal dan berada di tengah, namun Anda dapat mengubahnya dengan CSS.

## Tag Tabel HTML
Deskripsi Tag

`<tabel>` Mendefinisikan sebuah tabel

`<th>` Mendefinisikan sel header dalam sebuah tabel

`<tr>` Mendefinisikan baris dalam tabel

`<td>` Mendefinisikan sel dalam tabel

`<caption>` Mendefinisikan keterangan tabel

`<colgroup>` Menentukan grup yang terdiri dari satu atau lebih kolom dalam tabel untuk diformat

`<col>` Menentukan properti kolom untuk setiap kolom dalam elemen <colgroup>

`<thead>` Mengelompokkan konten header dalam sebuah tabel

`<tbody>` Mengelompokkan konten isi dalam tabel

`<tfoot>` Mengelompokkan konten footer dalam sebuah tabel

