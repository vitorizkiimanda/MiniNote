
<div align="center"><img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/logo.PNG?raw=true" width="290" height="110"></div>

<br/>


[Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Maintenance](#maintenance) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:


***MiniNote*** merupakan suatu web apps yang berguna untuk menyimpan catatan kecil untuk siapa saja. Catatan tersebut aman karena dilengkapi dengan fitur password. User dapat membuat catatan berbasis markdown sehingga lebih interaktif.


# Instalasi

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

- Buat database untuk Dotclear
```
$ mysql -u root -p
```
```
	CREATE DATABASE dotclear;
	CREATE USER dotclear IDENTIFIED BY 'dotclear';
	GRANT ALL PRIVILEGES ON dotclear.* TO dotclear;"
 ```

- Pindah ke direktori web di localhost
```
$ cd /var/www/html/
```

- Mendownload packages terakhir dari situs dotclear.org
```
$ wget http://download.dotclear.org/latest.tar.gz
```

- Mengekstrak packages yang telah didownload
```
$ tar -xvzf latest.tar.gz
```

-  Mengatur hak akses
```
$ sudo chmod a+w cache/
$ sudo chmod a+w inc/
$ sudo chmod a+w public/
```

- Mengakses web `localhost:8888/dotclear/`

# Konfigurasi  
[`^ kembali ke atas ^`](#)  
Untuk mengakses konfigurasi, maka memilih menu System settings lalu memilih sub menu about:config.

- ***antispam*** : mencegah agar pengguna tidak melakukan spamming dalam pembuatan akun, tipe datanya adalah integer  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/1.JPG?raw=true"></img>
- ***breadcrumb*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/2.JPG?raw=true"></img>
- ***dcckeditor*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/3.JPG?raw=true"></img>
- ***dclegacyeditor*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/4.JPG?raw=true"></img>
- ***pings*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/5.JPG?raw=true"></img>
- ***system*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/6.JPG?raw=true"></img>
- ***themes*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/konfigurasi/7.JPG?raw=true"></img>


# Maintenance
[`^ kembali ke atas ^`](#)  

Untuk mengakses maintenance, maka memilih menu plugins lalu memilih sub menu maintenance.  

- ***servicing*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/1.JPG?raw=true"></img>  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/2.JPG?raw=true"></img>
- ***backup*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/3.JPG?raw=true"></img>
- ***alert settings*** :  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/4.JPG?raw=true"></img>  <img src="https://github.com/haefa/dotclear/blob/master/screenshot/maintenance/5.JPG?raw=true"></img>


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
1. [Dotclear](https://dotclear.org/) - dotclear
2. [ How To Install Dotclear In Ubuntu](https://www.linuxhelp.com/how-to-install-dotclear-in-ubuntu/) - linuxhelp
3. [ Compare Dotclear vs. WordPress](https://comparisons.financesonline.com/wordpress-vs-dotclear) - financesonline
3. [ Compare Dotclear vs. Drupal](https://comparisons.financesonline.com/dotclear-vs-drupal) - financesonline
