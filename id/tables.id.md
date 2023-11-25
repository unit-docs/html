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

# Batas Tabel HTML

Tabel HTML dapat memiliki batas gaya dan bentuk yang berbeda.

Cara Menambahkan Perbatasan

Untuk menambahkan border, gunakan properti border CSS pada elemen tabel, th, dan td:

![tabel html](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html.png)

Contoh : 
```sh
table, th, td {
  border: 1px solid black;
}
```

## Batas Tabel Runtuh
Untuk menghindari batas ganda seperti pada contoh di atas, setel properti CSS border-collapse menjadi ciutkan.

Hal ini akan membuat perbatasan tersebut runtuh menjadi satu perbatasan:

![tabel html(3)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(3).png)

Contoh : 
```sh
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
```
## Batas Tabel Gaya

Jika Anda mengatur warna latar belakang setiap sel, dan memberi warna putih pada tepinya (sama dengan latar belakang dokumen), Anda mendapatkan kesan tepi yang tidak terlihat:

![tabel html(4)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(4).png)

Contoh : 
```sh
table, th, td {
  border: 1px solid white;
  border-collapse: collapse;
}
th, td {
  background-color: #96D4D4;
}
```

## Perbatasan Meja Bundar

Dengan properti border-radius, batasnya berbentuk sudut membulat:

![tabel html(5)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(5).png)

Contoh : 
```sh
table, th, td {
  border: 1px solid black;
  border-radius: 10px;
}
```
Lewati batas di sekitar tabel dengan meninggalkan tabel dari pemilih css:

![tabel html(6)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(6).png)

Contoh : 
```sh
th, td {
  border: 1px solid black;
  border-radius: 10px;
}
```

## Batas Tabel Bertitik

Dengan properti border-style, Anda dapat mengatur tampilan perbatasan.

![tabel html(7)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(7).png)

Nilai-nilai berikut diperbolehkan:

burik

putus-putus

padat

dobel

alur

punggung bukit

sisipan

awal

tidak ada

tersembunyi

Contoh : 
```sh
 th, td {
  border-style: dotted;
}
```

## Warna Perbatasan
Dengan properti border-color, Anda dapat mengatur warna border.

![tabel html(8)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(8).png)

Contoh : 
```sh
 th, td {
  border-color: #96D4D4;
}
```

# Ukuran Tabel HTML
Tabel HTML dapat memiliki ukuran berbeda untuk setiap kolom, baris, atau keseluruhan tabel.

![tabel html(9)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(9).png)

![tabel html(10)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(10).png)

![tabel html(11)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(11).png)

Gunakan atribut style dengan properti lebar atau tinggi untuk menentukan ukuran tabel, baris, atau kolom.

## Lebar Tabel HTML

Untuk mengatur lebar tabel, tambahkan atribut style ke elemen `<table>`:
Contoh : 

Atur lebar tabel ke 100%:

```sh
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```

## Lebar Kolom Tabel HTML

![tabel html(12)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(12).png)

Untuk mengatur ukuran kolom tertentu, tambahkan atribut style pada elemen <th> atau <td>:

Contoh : 
```sh
Tetapkan lebar kolom pertama ke 70%:
<table style="width:100%">
  <tr>
    <th style="width:70%">Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```
## Tinggi Baris Tabel HTML

![tabel html(13)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(13).png)

Untuk mengatur tinggi baris tertentu, tambahkan atribut style pada elemen baris tabel:

Contoh : 

Tetapkan tinggi baris kedua ke 200 piksel:
```sh
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr style="height:200px">
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```

## Tajuk Tabel HTML
Tabel HTML dapat memiliki header untuk setiap kolom atau baris, atau untuk banyak kolom/baris.



