# Paragraf HTML
Sebuah paragraf selalu dimulai pada baris baru, dan biasanya berupa blok teks.
## Paragraf HTML
Elemen HTML `<p>` mendefinisikan sebuah paragraf.
Sebuah paragraf selalu dimulai pada baris baru, dan browser secara otomatis menambahkan spasi (margin) sebelum dan sesudah paragraf.

Contoh : 
```sh
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```
## Tampilan HTML
Anda tidak dapat memastikan bagaimana HTML akan ditampilkan.
Layar besar atau kecil, dan jendela yang diubah ukurannya akan memberikan hasil yang berbeda.
Dengan HTML, Anda tidak dapat mengubah tampilan dengan menambahkan spasi atau baris tambahan pada kode HTML Anda.
Browser akan secara otomatis menghapus spasi dan baris tambahan saat halaman ditampilkan:

Contoh : 
```sh
<p>
This paragraph
contains a lot of lines
in the source code,
but the browser
ignores it.
</p>

<p>
This paragraph
contains         a lot of spaces
in the source         code,
but the        browser
ignores it.
</p>
```
## Aturan Horisontal HTML
Tag `<hr>` mendefinisikan jeda tematik di halaman HTML, dan paling sering ditampilkan sebagai aturan horizontal.
Elemen `<hr>` digunakan untuk memisahkan konten (atau menentukan perubahan) di halaman HTML:

Contoh : 
```sh
<h1>This is heading 1</h1>
<p>This is some text.</p>
<hr>
<h2>This is heading 2</h2>
<p>This is some other text.</p>
<hr>
```
Tag `<hr>` merupakan tag kosong yang artinya tidak memiliki tag akhir.
## Jeda Baris HTML
Elemen HTML `<br>` mendefinisikan jeda baris.
Gunakan `<br>` jika Anda menginginkan jeda baris (baris baru) tanpa memulai paragraf baru:

Contoh : 
```sh
<p>This is<br>a paragraph<br>with line breaks.</p>
```
Tag `<br>` merupakan tag kosong yang artinya tidak memiliki tag akhir.
## Masalah Puisi
Puisi ini akan ditampilkan dalam satu baris:

Contoh : 
```sh
<p>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</p>
```
## Solusi - Elemen HTML `<pre>`
Elemen HTML `<pre>` mendefinisikan teks yang telah diformat sebelumnya.
Teks di dalam elemen `<pre>` ditampilkan dalam font dengan lebar tetap (biasanya Courier), dan mempertahankan spasi dan jeda baris:

Contoh :
```sh
<pre>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</pre>
```
