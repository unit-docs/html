# Plugin HTML
Plug-in adalah program komputer yang memperluas fungsionalitas standar browser.
## Plug-in
Plug-in dirancang untuk digunakan untuk berbagai tujuan berbeda:

- Untuk menjalankan applet Java

- Untuk menjalankan kontrol Microsoft ActiveX

- Untuk menampilkan film Flash

- Untuk menampilkan peta

- Untuk memindai virus

- Untuk memverifikasi id bank

Peringatan !

Kebanyakan browser tidak lagi mendukung Java Applet dan Plug-in.
Kontrol ActiveX tidak lagi didukung di browser mana pun.
Dukungan untuk Shockwave Flash juga telah dimatikan di browser modern

## Elemen `<objek>`
Elemen ini `<object>` didukung oleh semua browser.
Elemen `<object>` mendefinisikan objek yang tertanam dalam dokumen HTML.
Itu dirancang untuk menyematkan plug-in (seperti applet Java, pembaca PDF, dan Pemutar Flash) di halaman web, tetapi juga dapat digunakan untuk memasukkan HTML ke dalam HTML:
Contoh
``` sh
<object width="100%" height="500px" data="snippet.html"></object>
```
Atau gambar jika Anda suka:
Contoh
``` sh
<object data="audi.jpeg"></object>
```
## Elemen `<sematkan>`
Elemen ini `<embed>` didukung di semua browser utama.
Elemen ini `<embed>` juga mendefinisikan objek yang tertanam dalam dokumen HTML.
Browser web telah mendukung elemen `<embed>` sejak lama. Namun, ini belum menjadi bagian dari spesifikasi HTML sebelum HTML5.
Contoh
``` sh
<embed src="audi.jpeg">
```
Perhatikan bahwa elemen `<embed>` tidak memiliki tag penutup. Itu tidak boleh berisi teks alternatif.
Elemen ini `<embed>` juga dapat digunakan untuk memasukkan HTML ke dalam HTML:
Contoh
``` sh
<embed width="100%" height="500px" src="snippet.html">
```
