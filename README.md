
<div align="center"><img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/logo.PNG?raw=true" width="290" height="110"></div>

<br/>


[Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Maintenance](#maintenance) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:


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

- *install* npm
dalam root directory yang telah di clone :
```
npm install
```

- *install* npm
dalam folder mininote-frontend, install lagi npm
```
npm install
```

- config.js
dalam config.js atur kembali jika diperlukan, seperti web server port di set menjadi di atas 5000

- npm run
Pada folder mininote-frontend run npm
```
npm run build
```

- npm start
Pada folder root start npm
```
npm start
```

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