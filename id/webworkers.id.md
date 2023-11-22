---
title: Web Workers
date : 2023-11-22
draft: true
---

# Pekerja Web HTML API

Pekerja web adalah JavaScript yang berjalan di latar belakang, tanpa memengaruhi kinerja laman.

## Apa itu pekerja Web ?
Saat menjalankan skrip di halaman HTML, halaman tersebut menjadi tidak responsif hingga skrip selesai.

Pekerja web adalah JavaScript yang berjalan di latar belakang, terlepas dari skrip lain, tanpa memengaruhi kinerja laman. Anda dapat terus melakukan 

apa pun yang Anda inginkan: mengklik, memilih sesuatu, dll., saat pekerja web berjalan di latar belakang.

## Peramban pendukung 

![webworkers1](https://github.com/uin-unit/docs-html/blob/main/images/webworkers1.png)

## Contoh HTML Pekerja Web 

Contoh di bawah ini membuat pekerja web sederhana yang menghitung angka di latar belakang:

Contoh :

![webworkers2](https://github.com/uin-unit/docs-html/blob/main/images/webworkers2.png)

## Periksa Dukungan Pekerja Web

Sebelum membuat pekerja web, periksa apakah browser pengguna mendukungnya:

Contoh : 
```sh
if (typeof(Worker) !== "undefined") {
  // Yes! Web worker support!
  // Some code.....
} else {
  // Sorry! No Web Worker support..
}
```

## Buat File Pekerja Web 

Sekarang, mari buat pekerja web kita dalam JavaScript eksternal.

Di sini, kami membuat skrip yang penting. Skrip disimpan dalam file "demo_workers.js":

Contoh : 
```sh
var i = 0;
function timedCount() {
  i = i + 1;
  postMessage(i);
  setTimeout("timedCount()",500);
}
timedCount();
```

Bagian penting dari kode di atas adalah metode posting Pesan() - yang digunakan untuk mengirim pesan kembali ke halaman HTML.

Catatan: Biasanya pekerja web tidak digunakan untuk skrip sederhana seperti itu, tetapi untuk tugas-tugas yang lebih intensif CPU.

## Buat Objek Pekerja Web

Sekarang kita memiliki file pekerja web, kita perlu memanggilnya dari halaman HTML.

Baris berikut memeriksa apakah pekerja sudah ada, jika belum - baris ini akan membuat objek pekerja web baru dan menjalankan kode di "demo_workers.js":

Contoh : 
```sh
if (typeof(w) == "undefined") {
  w = new Worker("demo_workers.js");
}
```

Kemudian kita dapat mengirim dan menerima pesan dari pekerja web.

Tambahkan pendengar acara "onmessage" ke pekerja web.

Contoh : 
```sh
w.onmessage = function(event){
  document.getElementById("result").innerHTML = event.data;
};
```

Saat pekerja web memposting pesan, kode dalam pendengar acara akan dieksekusi. Data dari pekerja web disimpan di event.data.

## Hentikan Pekerja Web

Saat objek pekerja web dibuat, objek tersebut akan terus mendengarkan pesan (bahkan setelah skrip eksternal selesai) hingga dihentikan.

Untuk menghentikan pekerja web, dan membebaskan sumber daya browser/komputer, gunakan metode penghentian():

Contoh : 
```sh
w.terminate();
```

## Gunakan kembali Pekerja Web

Jika Anda menyetel variabel pekerja ke tidak terdefinisi, setelah variabel tersebut dihentikan, Anda dapat menggunakan kembali kode:

Contoh : 
```sh
w = undefined;
```

## Contoh Kode Pekerja Web Lengkap

Kita telah melihat kode Pekerja di file .js. Di bawah ini adalah kode untuk halaman HTML:

Contoh :
```sh
<!DOCTYPE html>
<html>
<body>
<p>Count numbers: <output id="result"></output></p>
<button onclick="startWorker()">Start Worker</button>
<button onclick="stopWorker()">Stop Worker</button>
<script>
var w;
function startWorker() {
  if (typeof(Worker) !== "undefined") {
    if (typeof(w) == "undefined") {
  	w = new Worker("demo_workers.js");
	}
    w.onmessage = function(event) {
  	document.getElementById("result").innerHTML = event.data;
    };
  } else {
	document.getElementById("result").innerHTML = "Sorry! No Web Worker support.";
  }
}
function stopWorker() {
  w.terminate();
  w = undefined;
}
</script>
</body>
</html>
```

## Pekerja Web dan DOM

Karena pekerja web berada dalam file eksternal, mereka tidak memiliki akses ke objek JavaScript berikut:
- Objek jendela
- Objek dokumen
- Objek induk
