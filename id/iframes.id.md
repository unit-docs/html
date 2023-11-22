# Iframe HTML
Iframe HTML digunakan untuk menampilkan halaman web di dalam halaman web.
## Syntax Iframe HTML
Tag HTML <iframe>menentukan bingkai sebaris.
Bingkai sebaris digunakan untuk menyematkan dokumen lain ke dalam dokumen HTML saat ini.
## Syntax
```sh
<iframe src="url" title="description"></iframe>
```
## Iframe - Atur Tinggi dan Lebar
Gunakan atribut heightdan widthuntuk menentukan ukuran iframe.
Tinggi dan lebar ditentukan dalam piksel secara default:
Contoh : 
```sh
<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>
```
Atau Anda dapat menambahkan atribut gaya dan menggunakan properti tinggi dan lebar CSS:
Contoh : 
```sh
<iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe Example"></iframe>
```
## Iframe - Hapus Perbatasan
Secara default, iframe memiliki batas di sekelilingnya.
Untuk menghapus batas, tambahkan styleatribut dan gunakan properti CSS border
Contoh : 
```sh
<iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>
```
Dengan CSS, Anda juga dapat mengubah ukuran, gaya, dan warna batas iframe:
Contoh : 
```sh
<iframe src="demo_iframe.htm" style="border:2px solid red;" title="Iframe Example"></iframe>
## Iframe - Target untuk Tautan
Iframe dapat digunakan sebagai bingkai target untuk sebuah tautan.
Atribut targetlink harus mengacu pada nameatribut iframe:
Contoh :
```sh
<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>
<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
```
## Ringkasan Bab
Tag HTML <iframe>menentukan bingkai sebaris
Atribut src mendefinisikan URL halaman yang akan disematkan
Selalu sertakan titleatribut (untuk pembaca layar)
Atribut heightand widthmenentukan ukuran iframe
Gunakan border:none;untuk menghapus batas di sekitar iframe
Tag iframe HTML
Tag	Description
<iframe>	Defines an inline frame
