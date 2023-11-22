# HTML SSE API
Peristiwa Terkirim Server/Server Sent Event (SSE) memungkinkan halaman web mendapatkan pembaruan dari server.
# Server-Sent Events - Pesan Satu Arah
Peristiwa terkirim server adalah ketika halaman web secara otomatis mendapat pembaruan dari server.
Ini juga mungkin terjadi sebelumnya, tetapi halaman web harus menanyakan apakah ada pembaruan yang tersedia. Dengan acara yang dikirim server, pembaruan datang secara otomatis.
Contoh: Update Facebook/Twitter, update harga saham, feed berita, hasil olahraga, dll.
# Peramban Pendukung
![alt text](https://github.com/uin-unit/docs-html/blob/main/images/sse%20api.png)
# Terima Pemberitahuan Acara yang Dikirim Server
Contoh : 
```sh
var source = new EventSource("demo_sse.php");
source.onmessage = function(event) {
  document.getElementById("result").innerHTML += event.data + "<br>";
};
```
Penjelasan Contoh : 
- Buat objek EventSource baru, dan tentukan URL halaman yang mengirimkan pembaruan (dalam contoh ini "demo_sse.php")
- Setiap kali pembaruan diterima, peristiwa onmessage terjadi
- Ketika peristiwa onmessage terjadi, masukkan data yang diterima ke dalam elemen dengan id="result"
# Periksa Dukungan Acara Terkirim Server
Dalam contoh percobaan di atas ada beberapa baris kode tambahan untuk memeriksa dukungan browser untuk peristiwa yang dikirim server:
Contoh : 
```sh
if(typeof(EventSource) !== "undefined") {
  // Yes! Server-sent events support!
  // Some code.....
} else {
  // Sorry! No server-sent events support..
}


```
# Contoh Kode Sisi Server
Agar contoh di atas dapat berfungsi, Anda memerlukan server yang mampu mengirimkan pembaruan data (seperti PHP atau ASP).
Sintaks aliran peristiwa sisi server sederhana. Setel tajuk "Jenis Konten" ke "aliran teks/acara". Sekarang Anda dapat mulai mengirimkan aliran acara.
Kode dalam PHP (demo_sse.php):
Contoh : 
```sh
<?php
header('Content-Type: text/event-stream');
header('Cache-Control: no-cache');
$time = date('r');
echo "data: The server time is: {$time}\n\n";
flush();
?>
```
Code in ASP (VB) (demo_sse.asp):
Contoh : 
```sh
<%
Response.ContentType = "text/event-stream"
Response.Expires = -1
Response.Write("data: The server time is: " & now())
Response.Flush()
%>
```
Penjelasan Kode 
- Setel tajuk "Jenis Konten" ke "aliran teks/acara"
- Tentukan bahwa halaman tersebut tidak boleh di-cache
- Keluarkan data yang akan dikirim (Selalu dimulai dengan "data:")
- Siram data keluaran kembali ke halaman web
# Objek Sumber Peristiwa
Pada contoh di atas kita menggunakan event onmessage untuk menerima pesan. Namun acara lain juga tersedia:
![alt text](https://github.com/uin-unit/docs-html/blob/main/images/sse%20api%202.png)

