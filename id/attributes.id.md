# ATRIBUT HTML
Atribut HTML memberikan informasi tambahan tentang elemen HTML.

## Atribut HTML

- Semua elemen HTML dapat memiliki atribut
- Atribut memberikan informasi tambahan tentang elemen
- Atribut selalu ditentukan dalam tag awal
- Atribut biasanya datang dalam pasangan nama/nilai seperti: name="value"

## Atribut href

Tag <a> mendefinisikan hyperlink. Atribut href menentukan URL halaman yang dituju link tersebut:
Contoh : 
```sh
<a href="https://www.w3schools.com">Visit W3Schools</a>
```
## The src Attribute
Tag <img> digunakan untuk menyematkan gambar dalam halaman HTML. Atribut src menentukan jalur ke gambar yang akan ditampilkan:
Contoh : 
```sh
<img src="img_girl.jpg">
```
Ada dua cara untuk menentukan URL di atribut src:
1. URL Absolut - Tautan ke gambar eksternal yang dihosting di situs web lain. Contoh: src="https://www.w3schools.com/images/img_girl.jpg".
Catatan: Gambar eksternal mungkin dilindungi hak cipta. Jika Anda tidak mendapatkan izin untuk menggunakannya, Anda mungkin melanggar undang-undang hak cipta. Selain itu, Anda tidak dapat mengontrol gambar eksternal; itu bisa tiba-tiba dihapus atau diubah.

2. URL Relatif - Tautan ke gambar yang dihosting di dalam situs web. Di sini, URL tidak menyertakan nama domain. Jika URL diawali tanpa garis miring, URL tersebut akan relatif terhadap halaman saat ini. Contoh: src="img_girl.jpg". Jika URL dimulai dengan garis miring, itu akan berhubungan dengan domain. Contoh: src="/images/img_girl.jpg".
Tip: Hampir selalu yang terbaik adalah menggunakan URL relatif. Mereka tidak akan rusak jika Anda mengubah domain.

## Atribut lebar dan tinggi
Tag <img> juga harus berisi atribut lebar dan tinggi, yang menentukan lebar dan tinggi gambar (dalam piksel):\

Contoh : 

```sh
<img src="img_girl.jpg" width="500" height="600">
```

## Atribut alt

Atribut alt yang diperlukan untuk tag <img> menentukan teks alternatif untuk gambar, jika gambar karena alasan tertentu tidak dapat ditampilkan. Hal ini dapat disebabkan oleh koneksi yang lambat, atau kesalahan pada atribut src, atau jika pengguna menggunakan pembaca layar.

Contoh : 
```sh
<img src="img_girl.jpg" alt="Girl with a jacket">
```

Contoh : 

See what happens if we try to display an image that does not exist:
```sh
<img src="img_typo.jpg" alt="Girl with a jacket">
```
## Atribut gaya
Atribut style digunakan untuk menambahkan gaya pada suatu elemen, seperti warna, font, ukuran, dan lainnya.
Contoh : 
```sh
<p style="color:red;">This is a red paragraph.</p>
```
## Atribut lang

Anda harus selalu menyertakan atribut lang di dalam tag <html>, untuk mendeklarasikan bahasa halaman Web. Ini dimaksudkan untuk membantu mesin pencari dan browser.
Contoh berikut menetapkan bahasa Inggris sebagai bahasanya:
```sh
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```

Kode negara juga dapat ditambahkan ke kode bahasa di atribut lang. Jadi, dua karakter pertama menentukan bahasa halaman HTML, dan dua karakter terakhir menentukan negara.

Contoh berikut menetapkan bahasa Inggris sebagai bahasanya dan Amerika Serikat sebagai negaranya:

```sh
<!DOCTYPE html>
<html lang="en-US">
<body>
...
</body>
</html>
```

## Judul Atribut
Atribut title mendefinisikan beberapa informasi tambahan tentang suatu elemen.

Nilai atribut title akan ditampilkan sebagai tooltip ketika Anda mengarahkan mouse ke elemen:

Contoh : 
```sh
<p title="I'm a tooltip">This is a paragraph.</p>
```
Saran Kami: Selalu Gunakan Atribut Huruf Kecil
Standar HTML tidak memerlukan nama atribut huruf kecil.
Atribut judul (dan seluruh atribut lainnya) dapat ditulis dengan huruf besar atau huruf kecil seperti judul atau TITLE.
Namun, W3C merekomendasikan atribut huruf kecil dalam HTML, dan meminta atribut huruf kecil untuk jenis dokumen yang lebih ketat seperti XHTML.

Saran Kami: Selalu Mengutip Nilai Atribut
Standar HTML tidak memerlukan tanda kutip di sekitar nilai atribut.
Namun, W3C merekomendasikan kutipan dalam HTML, dan meminta kutipan untuk jenis dokumen yang lebih ketat seperti XHTML.

**Good:**
```sh
<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
```
**Bad:**
```sh
<a href=https://www.w3schools.com/html/>Visit our HTML tutorial</a>
```
Terkadang Anda harus menggunakan tanda kutip. Contoh ini tidak akan menampilkan atribut title dengan benar, karena mengandung spasi:

Contoh : 

```sh
<p title=About W3Schools>
```

## Kutipan Tunggal atau Ganda?

Tanda kutip ganda di sekitar nilai atribut adalah yang paling umum dalam HTML, namun tanda kutip tunggal juga dapat digunakan.

Dalam beberapa situasi, ketika nilai atribut itu sendiri berisi tanda kutip ganda, maka perlu menggunakan tanda kutip tunggal:

`<p title='John "ShotGun" Nelson'>`
Atau sebaliknya:
`<p title="John 'ShotGun' Nelson">`

## Ringkasan Bab

Semua elemen HTML dapat memiliki atribut

- Atribut href dari <a> menentukan URL halaman yang dituju link tersebut

- Atribut src dari <img> menentukan jalur ke gambar yang akan ditampilkan

- Atribut lebar dan tinggi <img> memberikan informasi ukuran gambar

- Atribut alt <img> menyediakan teks alternatif untuk gambar

- Atribut style digunakan untuk menambahkan gaya pada suatu elemen, seperti warna, font, ukuran, dan lainnya

- Atribut lang dari tag <html> mendeklarasikan bahasa halaman Web

- Atribut title mendefinisikan beberapa informasi tambahan tentang suatu elemen
