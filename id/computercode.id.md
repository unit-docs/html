---
title: "computercode"
date : 2023-11-22
draft: true
---

# Elemen Kode Komputer HTML
HTML berisi beberapa elemen untuk mendefinisikan input pengguna dan kode komputer.
Contoh : 
``` sh
<code>
x = 5;
y = 6;
z = x + y;
</code>
```
# HTML `<kbd>` Untuk Masukan Keyboard
Elemen HTML `<kbd>` digunakan untuk mendefinisikan input keyboard. Konten di dalamnya ditampilkan dalam font monospace default browser.
Contoh : 
Menetapkan beberapa teks sebagai input keyboard dalam dokumen:
``` sh
<p>Save the document by pressing <kbd>Ctrl + S</kbd></p>
Result:
Simpan dokumen dengan menekan Ctrl + S
```

# HTML `<samp>` Untuk Keluaran Program
Elemen HTML <samp> digunakan untuk menentukan contoh keluaran dari program komputer. Konten di dalamnya ditampilkan dalam font monospace default browser.
Contoh : 
Tentukan beberapa teks sebagai contoh keluaran dari program komputer dalam dokumen:
``` sh
<p>Message from my computer:</p>
<p><samp>File not found.<br>Press F1 to continue</samp></p>
Result:
Pesan dari komputer saya:
File not found.
Press F1 to continue
```

# HTML `<code>` Untuk Kode Komputer
Elemen HTML `<code>` digunakan untuk mendefinisikan sepotong kode komputer. Konten di dalamnya ditampilkan dalam font monospace default browser.

Contoh : 
Menetapkan beberapa teks sebagai kode komputer dalam dokumen:
``` sh
<code>
x = 5;
y = 6;
z = x + y;
</code>
Result:
x = 5; y = 6; z = x + y;
```

Perhatikan bahwa elemen `<code>` tidak mempertahankan spasi tambahan dan jeda baris.
Untuk memperbaikinya, Anda bisa meletakkan elemen `<code>` di dalam elemen `<pre>`:

Contoh : 
``` sh
<pre>
<code>
x = 5;
y = 6;
z = x + y;
</code>
</pre>
Result:
x = 5;
y = 6;
z = x + y;
```

## HTML `<var>` Untuk Variabel
Elemen HTML `<var>` digunakan untuk mendefinisikan variabel dalam pemrograman atau ekspresi matematika. Konten di dalamnya biasanya ditampilkan dalam huruf miring.

Contoh : 
Mendefinisikan beberapa teks sebagai variabel dalam dokumen:
``` sh
<p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var>, where <var>b</var> is the base, and <var>h</var> is the vertical height.</p>
Result:
The area of a triangle is: 1/2 x b x h, where b is the base, and h is the vertical height.
```

# Ringkasan Bab

- Elemen `<kbd>` mendefinisikan input keyboard
- Elemen `<samp>` mendefinisikan contoh keluaran dari program komputer
- Elemen `<code>` mendefinisikan sepotong kode komputer
- Elemen `<var>` mendefinisikan variabel dalam pemrograman atau ekspresi matematika
- Elemen `<pre>` mendefinisikan teks yang telah diformat sebelumnya
