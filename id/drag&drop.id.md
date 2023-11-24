# API Seret dan Lepas HTML
Dalam HTML, elemen apa pun dapat diseret dan dilepas.
Contoh : 
Tarik gambar W3Schools ke dalam persegi panjang.

![ibnu](https://github.com/uin-unit/docs-html/blob/main/images/drag%20drop.png)
## Seret dan Jatuhkan
Seret dan lepas adalah fitur yang sangat umum. Itu adalah saat Anda "mengambil" suatu objek dan menyeretnya ke lokasi lain.

## Dukungan Peramban
Angka-angka pada tabel menunjukkan versi browser pertama yang sepenuhnya mendukung Drag and Drop.
API : Chrome, Microsoft Edge, Firefox, Safari, Opera 
Seret dan Jatuhkan : 4.0, 9.0, 3.5, 6.0, 12.0

## Contoh Seret dan Lepas HTML
Contoh di bawah ini adalah contoh drag and drop sederhana:


Contoh:
``` sh
<!DOCTYPE HTML>
<html>
<head>
<script>
function allowDrop(ev) {
  ev.preventDefault();
}


function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}


function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  ev.target.appendChild(document.getElementById(data));
}
</script>
</head>
<body>


<div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>


<img id="drag1" src="img_logo.gif" draggable="true" ondragstart="drag(event)" width="336" height="69">


</body>
</html>
```
Ini mungkin tampak rumit, tapi mari kita bahas semua bagian berbeda dari acara seret dan lepas.
## Jadikan Elemen Dapat Diseret
Pertama-tama: Untuk membuat elemen dapat diseret, setel atribut dapat diseret ke true:
``` sh
<img draggable="true">
```
## Apa yang Harus Diseret - ondragstart dan setData()
Lalu, tentukan apa yang akan terjadi saat elemen diseret.
Pada contoh di atas, atribut `ondragstart` memanggil fungsi, drag(event), yang menentukan data apa yang akan diseret.
Metode `dataTransfer.setData()` menyetel tipe data dan nilai data yang diseret:
Contoh : 
``` sh
function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}
```
Dalam hal ini, tipe datanya adalah "teks" dan nilainya adalah id elemen yang dapat diseret ("drag1").
## Tempat Menjatuhkan - ondragover
Peristiwa ondragover menentukan di mana data yang diseret dapat dibuang.


Secara default, data/elemen tidak dapat dihilangkan di elemen lain. Untuk mengizinkan penurunan, kita harus mencegah penanganan default elemen tersebut.
Hal ini dilakukan dengan memanggil metode `event.preventDefault()` untuk acara ondragover:
Contoh : 
``` sh
event.preventDefault()
```
## Lakukan Drop – ondrop
Ketika data yang diseret dibuang, peristiwa penurunan terjadi.
Pada contoh di atas, atribut ondrop memanggil fungsi drop(event):
``` sh
function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  ev.target.appendChild(document.getElementById(data));
}
```
Kode menjelaskan:
Panggil `preventDefault()` untuk mencegah penanganan data secara default oleh browser (defaultnya terbuka sebagai tautan yang dilepaskan)
Dapatkan data yang diseret dengan metode `dataTransfer.getData()`. Metode ini akan mengembalikan data apa pun yang disetel ke tipe yang sama dalam metode `setData()`
Data yang diseret adalah id elemen yang diseret ("drag1")
Tambahkan elemen yang diseret ke dalam elemen drop
## Contoh Lainnya
Contoh
Cara menarik (dan melepas) gambar bolak-balik antara dua elemen <div>:
![ibnu](https://github.com/uin-unit/docs-html/blob/main/images/drag%20drop.png)
