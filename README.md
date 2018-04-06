
<div align="center"><img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/logo.PNG?raw=true" width="290" height="110"></div>

<br/>


[Instalasi dan konfigurasi](#instalasi)| [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:


***MiniNote*** merupakan suatu web apps yang berguna untuk menyimpan catatan kecil untuk siapa saja. Catatan tersebut aman karena dilengkapi dengan fitur password. User dapat membuat catatan berbasis markdown sehingga lebih interaktif.


# Instalasi dan Konfigurasi

**Kebutuhan Sistem :**
- `NodeJS >= 6.x`


**Proses Instalasi :**
- *Update* sistem dengan versi yang terbaru
```
$ sudo apt-get update -y
```

- *Install* ssh
```
$ sudo apt update
$ sudo apt install ssh
```

- *Install* nodejs
```
$ sudo apt-get update
$ sudo apt-get install nodejs
```

- clone source code mininote
```
git clone https://github.com/n1try/mininote
```

- *install* npm <br>
dalam root directory yang telah di clone :
```
npm install
```

- *install* npm <br>
dalam folder mininote-frontend, install lagi npm
```
npm install
```

- config.js <br>
dalam config.js atur kembali jika diperlukan, seperti web server port di set menjadi di atas 5000

- npm run <br>
Pada folder mininote-frontend run npm
```
npm run build
```

- npm start <br>
Pada folder root start npm
```
npm start
```

# Cara Pemakaian
[`^ kembali ke atas ^`](#)  
1. Akses MiniNote melalui [http://localhost:8888](http://localhost:8888)
2. Ketik judul notebook baik yang pernah disimpan ataupun yang baru 
<img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/home.PNG?raw=true"></img>
3. Ketik password dari notebook jika membuka memasukkan judul yang pernah dibuat sebelumnya ( jika baru buat password baru )  
<img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/home_password.PNG?raw=true"></img>
4. Jika berhasil akan masuk pada halaman berikut :  
<img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/home_logged.PNG?raw=true"></img>
5. Masukkan nama Note pada field "add note" lalu click tombol plus hijau, jika berhasil maka tampilan akan menjadi seperti ini :   
<img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/new_note.PNG?raw=true"></img>
6. Selanjutnya isi catatan lalu clik icon save pada pojok kanan atas
<img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/fill_note.PNG?raw=true"></img>
7. Setelah catatan di save akan muncul pilihan untuk membuka note di kiri
<img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/success_note.PNG?raw=true"></img>

# Pembahasan
[`^ kembali ke atas ^`](#)  
**MiniNote** merupakan salah satu aplikasi *website open source* yang membantu user dalam menulis catatan. MiniNote dikembangkan dalam bahasa Javascript dengan framework VueJS untuk tampilan dan NodeJS untuk backend. MiniNote dapat diinstall secara manual. 

**Kelebihan**
- Catatan Aman
- Catatan Terjamin
- Simple (*Easy to use*)
- Ringan
- Mendukung Markdown

**Kekurangan**
- Ada batasan jumlah karakter
- Catatan yang sudah di ada, tidak ditampilkan saat *Landing Page*
- Tidak ada fitur lupa password dan lupa judul catatan

**Perbandingan dengan Aplikasi Sejenis**  
Dibandingkan dengan aplikasi sejenis seperti Notes.io, Notes.io dapat login menggunakan akun Facebook dan Twitter. Namun, tidak ada fitur password maka catatan terbuka dan tidak aman. Catatan disimpan dalam bentuk *link string random* sehingga tidak bisa terganti, sehingga user harus mengingat link tersebut.

# Referensi
1. [Mininote](https://github.com/n1try/mininote) - Source code and Installation mininote