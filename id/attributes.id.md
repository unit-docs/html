# Atribut ID HTML
Atribut HTML iddigunakan untuk menentukan id unik untuk elemen HTML.
Anda tidak boleh memiliki lebih dari satu elemen dengan id yang sama dalam dokumen HTML.
## Menggunakan Atribut id
Atribut idmenentukan id unik untuk elemen HTML. Nilai atribut id harus unik dalam dokumen HTML.
Atribut iddigunakan untuk menunjuk ke deklarasi gaya tertentu dalam style sheet. Itu juga digunakan oleh JavaScript untuk mengakses dan memanipulasi elemen dengan id tertentu.
Sintaks untuk id adalah: tulis karakter hash (#), diikuti dengan nama id. Lalu, definisikan properti CSS di dalam kurung kurawal {}.
Dalam contoh berikut kita memiliki `<h1>` elemen yang menunjuk ke nama id "myHeader". 
Elemen ini `<h1>` akan ditata sesuai dengan #myHeader definisi gaya di bagian kepala:
Contoh : 
```sh
<!DOCTYPE html>
<html>
<head>
<style>
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}
</style>
</head>
<body>

<h1 id="myHeader">My Header</h1>

</body>
</html>
```
Catatan: Nama id peka huruf besar-kecil!
Catatan: Nama id harus mengandung minimal satu karakter, tidak boleh diawali dengan angka, dan tidak boleh mengandung spasi (spasi, tab, dll).
## Perbedaan Antara Kelas dan ID
Nama kelas dapat digunakan oleh beberapa elemen HTML, sedangkan nama id hanya boleh digunakan oleh satu elemen HTML dalam halaman:
Contoh : 
```sh
<style>
/* Style the element with the id "myHeader" */
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}

/* Style all elements with the class name "city" */
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>

<!-- An element with a unique id -->
<h1 id="myHeader">My Cities</h1>

<!-- Multiple elements with same class -->
<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>
```
## Bookmark HTML dengan ID dan Tautan
Bookmark HTML digunakan untuk memungkinkan pembaca melompat ke bagian tertentu dari halaman web.
Bookmark dapat berguna jika halaman Anda sangat panjang.
Untuk menggunakan bookmark, Anda harus membuatnya terlebih dahulu, lalu menambahkan link ke bookmark tersebut.
Kemudian, ketika link tersebut diklik, halaman tersebut akan bergulir ke lokasi yang diberi bookmark.
Contoh
Pertama, buat bookmark dengan idatribut:
```sh
<  h2 id="C4"  >Chapter 4<  /h2  >
```
Atau, tambahkan link ke bookmark ("Lompat ke Bab 4"), dari halaman lain:
<a href="html_demo.html#C4">Jump to Chapter 4</a>
Menggunakan Atribut id dalam JavaScript
Atribut idjuga dapat digunakan oleh JavaScript untuk melakukan beberapa tugas untuk elemen tertentu.
JavaScript dapat mengakses elemen dengan id tertentu dengan getElementById()metode:
Contoh : 
### Gunakan atribut id untuk memanipulasi teks dengan JavaScript:
```sh
<script>
function displayResult() {
  document.getElementById("myHeader").innerHTML = "Have a nice day!";
}
</script>
```
## Ringkasan Bab
Atribut iddigunakan untuk menentukan id unik untuk elemen HTML
Nilai atribut id harus unik dalam dokumen HTML
Atribut ini id digunakan oleh CSS dan JavaScript untuk menata/memilih elemen tertentu
Nilai atribut id peka huruf besar-kecil
Atribut ini id juga digunakan untuk membuat bookmark HTML
JavaScript dapat mengakses elemen dengan id tertentu dengan getElementById() metode ini
