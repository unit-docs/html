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

![tabel html (14)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(14).png)

![tabel html(15)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(15).png)

## Tajuk Tabel HTML

Header tabel ditentukan dengan elemen ke-. Setiap elemen mewakili sel tabel.

Contoh : 
```sh
<table>
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

## Tajuk Tabel Vertikal

Untuk menggunakan kolom pertama sebagai header tabel, tentukan sel pertama di setiap baris sebagai elemen `<th>`:

Contoh :
```sh
<table>
  <tr>
    <th>Firstname</th>
    <td>Jill</td>
    <td>Eve</td>
  </tr>
  <tr>
    <th>Lastname</th>
    <td>Smith</td>
    <td>Jackson</td>
</tr>
  <tr>
    <th>Age</th>
    <td>94</td>
    <td>50</td>
  </tr>
</table>
```

## Sejajarkan Tajuk Tabel
Secara default, header tabel dicetak tebal dan berada di tengah:

![tabel html(16)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(16).png)

Untuk meratakan header tabel ke kiri, gunakan properti perataan teks CSS:

Contoh : 
```sh
th {
  text-align: left;
}
```

## Tajuk untuk Beberapa Kolom

Anda dapat memiliki header yang mencakup dua kolom atau lebih.

![tabel html(17)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(17).png)

Untuk melakukannya, gunakan atribut colspan pada elemen `<th>`:

Contoh : 
```sh
<table>
  <tr>
    <th colspan="2">Name</th>
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

## Keterangan Tabel

Anda dapat menambahkan keterangan yang berfungsi sebagai judul seluruh tabel.

![tabel html(18)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(18).png)

Untuk menambahkan keterangan pada tabel, gunakan tag `<caption>`:

Contoh : 
```sh
<table style="width:100%">
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$50</td>
  </tr>
</table>
```

# Lapisan & Spasi Tabel HTML
Tabel HTML dapat menyesuaikan lapisan di dalam sel, dan juga jarak antar sel.

![tabel html(19)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(19).png)

## Tabel HTML - Bantalan Sel

Cell lapisan adalah jarak antara tepi sel dan isi sel.

Secara default lapisan diatur ke 0.

Untuk menambahkan lapisan pada sel tabel, gunakan properti lapisan CSS:

Contoh : 
```sh
th, td {
  padding: 15px;
}
```
Untuk menambahkan padding hanya di atas konten, gunakan properti padding-top.

Dan yang lainnya berpihak pada properti padding-bottom, padding-left, dan padding-right:

Contoh : 
```sh
th, td {
  padding-top: 10px;
  padding-bottom: 20px;
  padding-left: 30px;
  padding-right: 40px;
}
```
## Tabel HTML - Spasi Sel

Jarak sel adalah jarak antar sel.

Secara default, spasi diatur ke 2 piksel.

Untuk mengubah spasi antar sel tabel, gunakan properti CSS border-spacing pada elemen tabel:

Contoh : 
```sh
table {
  border-spacing: 30px;
}
```

# Tabel HTML Colspan & Rowspan

Tabel HTML dapat memiliki sel yang mencakup beberapa baris dan/atau kolom.

![tabel html(20)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(20).png)

![tabel html(21)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(21).png)

## Tabel HTML - Colspan

Untuk membuat rentang sel pada beberapa kolom, gunakan atribut colspan:

Contoh : 
```sh
<table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>43</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>57</td>
  </tr>
</table>
```
## Tabel HTML - Rentang Baris
Untuk membuat rentang sel pada beberapa baris, gunakan atribut rowpan:

Example :
```sh
<table>
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>555-1234</td>
  </tr>
  <tr>
    <td>555-8745</td>
</tr>
</table>
```

# Penataan Tabel HTML
Gunakan CSS untuk membuat tabel Anda terlihat lebih baik.

## Tabel HTML - Garis Zebra
Jika Anda menambahkan warna latar belakang pada setiap baris tabel lainnya, Anda akan mendapatkan efek garis zebra yang bagus.

![tabel html(22)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(22).png)

Contoh : 
```sh
tr:nth-child(even) {
  background-color: #D6EEEE;
}
```
## Tabel HTML - Garis Zebra Vertikal
Untuk membuat garis zebra vertikal, beri gaya pada setiap kolom lainnya, bukan setiap baris lainnya.

![tabel html(23)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(23).png)

Atur :nth-child(even) untuk elemen data tabel seperti ini:

Contoh : 
```sh
td:nth-child(even), th:nth-child(even) {
  background-color: #D6EEEE;
}
```
# Gabungkan Garis Zebra Vertikal dan Horisontal
Anda dapat menggabungkan gaya dari dua contoh di atas dan Anda akan memiliki garis-garis di setiap baris dan kolom lainnya.

Jika Anda menggunakan warna transparan, Anda akan mendapatkan efek yang tumpang tindih.

![tabel html(24)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(24).png)

Gunakan warna rgba() untuk menentukan transparansi warna:

Contoh : 
```sh
tr:nth-child(even) {
  background-color: rgba(150, 212, 212, 0.4);
}
```

```sh
th:nth-child(even),td:nth-child(even) {
  background-color: rgba(150, 212, 212, 0.4);
}
```
## Pembagi horizontal

Nama Depan Nama Belakang Tabungan

Peter Griffin $100

Lois Griffin $150

Joe Swanson $300

Jika Anda menentukan batas hanya di bagian bawah setiap baris tabel, Anda akan memiliki tabel dengan pembagi horizontal.

Tambahkan properti border-bottom ke semua elemen tr untuk mendapatkan pembagi horizontal:

Contoh : 
```sh
tr {
  border-bottom: 1px solid #ddd;
}
```
## Tabel Melayang

Gunakan pemilih :hover di tr untuk menyorot baris tabel dengan mengarahkan mouse:

Nama Depan Nama Belakang Tabungan

Peter Griffin $100

Lois Griffin $150

Joe Swanson $300

Contoh : 
```sh
tr:hover {background-color: #D6EEEE;}
```

# Grup Tabel HTML
Elemen `<colgroup>` digunakan untuk memberi gaya pada kolom tertentu pada tabel.

## Grup Tabel HTML
Jika Anda ingin memberi gaya pada dua kolom pertama tabel, gunakan elemen `<colgroup>` dan `<col>`.

![tabel html(25)](https://github.com/uin-unit/docs-html/blob/main/images/tabel%20html(25).png)

Elemen `<colgroup>` harus digunakan sebagai wadah untuk spesifikasi kolom.

Setiap grup ditentukan dengan elemen `<col>`.

Atribut span menentukan berapa banyak kolom yang mendapatkan gaya.

Atribut style menentukan gaya yang akan diberikan pada kolom.

Catatan: Pilihan properti CSS legal untuk colgroups sangat terbatas.

Contoh : 
```sh
<table>
  <colgroup>
    <col span="2" style="background-color: #D6EEEE">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
...
```
## Properti CSS Hukum

Hanya ada pilihan properti CSS yang sangat terbatas yang diperbolehkan untuk digunakan di colgroup:

properti lebar

properti visibilitas

properti latar belakang

properti perbatasan

Semua properti CSS lainnya tidak akan berpengaruh pada tabel Anda.

## Beberapa Elemen Kol
Jika Anda ingin menata lebih banyak kolom dengan gaya berbeda, gunakan lebih banyak elemen `<col>` di dalam `<colgroup>`:

Contoh : 
```sh
<table>
  <colgroup>
    <col span="2" style="background-color: #D6EEEE">
    <col span="3" style="background-color: pink">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
...
```
## Colgroup Kosong
Jika Anda ingin memberi gaya pada kolom di tengah tabel, sisipkan elemen <col> "kosong" (tanpa gaya) untuk kolom sebelumnya:

Contoh : 
```sh
<table>
  <colgroup>
    <col span="3">
    <col span="2" style="background-color: pink">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
...
```
## Sembunyikan Kolom
Anda dapat menyembunyikan kolom dengan properti visibilitas: runtuh:

Contoh : 
```sh
<table>
  <colgroup>
    <col span="2">
    <col span="3" style="visibility: collapse">
  </colgroup>
  <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
...
```



