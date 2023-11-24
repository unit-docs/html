# HTML Quotation and Citation Elements
Dalam bab ini kita akan membahas elemen HTML `<blockquote>`,`<q>`, `<abbr>`, `<address>`, `<cite>`, dan `<bdo>`.
Contoh : 

Here is a quote from WWF's website:
For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
#### HTML `<blockquote>` untuk Kutipan
Elemen HTML `<blockquote>` mendefinisikan bagian yang dikutip dari sumber lain.
Browser biasanya membuat indentasi elemen 

Contoh : 
```sh
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
</blockquote>
```
#### HTML `<q>` untuk Kutipan Singkat
Tag HTML `<q>` mendefinisikan kutipan singkat.
Browser biasanya menyisipkan tanda kutip di sekitar kutipan.

Contoh : 
```sh
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
```
#### HTML `<abbr>` untuk Singkatan
Tag HTML `<abbr>` mendefinisikan singkatan atau akronim, seperti "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".
Menandai singkatan dapat memberikan informasi berguna bagi browser, sistem terjemahan, dan mesin pencari.
Tip: Gunakan atribut judul global untuk menampilkan deskripsi singkatan/akronim saat Anda mengarahkan mouse ke elemen.

Contoh : 
```sh
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```
#### HTML `<address>` untuk Informasi Kontak
Tag HTML `<address>` mendefinisikan informasi kontak penulis/pemilik dokumen atau artikel.
Informasi kontak dapat berupa alamat email, URL, alamat fisik, nomor telepon, alamat media sosial, dll.
Teks dalam elemen `<address>` biasanya ditampilkan dalam huruf miring, dan browser akan selalu menambahkan baris baru sebelum dan sesudah elemen `<address>`.

Contoh : 
```sh
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```
#### HTML `<cite>` untuk Judul Karya
Tag HTML `<cite>` mendefinisikan judul karya kreatif (misalnya buku, puisi, lagu, film, lukisan, patung, dll.).
Catatan : Nama seseorang bukanlah judul suatu karya.
Teks dalam elemen `<cite>` biasanya ditampilkan dalam huruf miring.

Contoh : 
```sh
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```
#### HTML `<bdo>` untuk Penggantian Dua Arah
BDO adalah singkatan dari Bi-Directional Override.
Tag HTML `<bdo>` digunakan untuk mengganti arah teks saat ini:

Contoh : 
```sh
<bdo dir="rtl">This text will be written from right to left</bdo>
```
![radhi](https://github.com/uin-unit/docs-html/blob/main/images/img%20quotation.png)
