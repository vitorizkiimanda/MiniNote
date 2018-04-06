
<div align="center"><img src="https://github.com/vitorizkiimanda/MiniNote/blob/master/screenshoot/logo.PNG?raw=true" width="290" height="110"></div>

<br/>

[Sekilas Tentang](#sekilas-tentang) | [Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Maintenance](#maintenance) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:|:--:

[Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Maintenance](#maintenance) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)
:---:|:---:|:---:|:---:|:---:|:---:


***MiniNote*** merupakan suatu web apps yang berguna untuk menyimpan catatan kecil untuk siapa saja. Catatan tersebut aman karena dilengkapi dengan fitur password. User dapat membuat catatan berbasis markdown sehingga lebih interaktif.


# Instalasi
[`^ kembali ke atas ^`](#)

**Kebutuhan Sistem :**
- `Web Server (Apache, Nginx, etc.)`
- `PHP 5.5 or above`
- `Database (MySQL, Postgre, etc.)`


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

- *Install* apache, MySQL, dan PHP
```
$ sudo apt install apache2
$ sudo apt install mysql-server
$ sudo apt install php
$ sudo apt install libapache2-mod-php
$ sudo apt install php-mysql
$ sudo apt install php-gd php-mcrypt php-mbstring php-xml php-ssh2
$ sudo service apache2 restart
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
1. Akses dotclear melalui [http://localhost:888/dotclear](http://localhost:8888/dotclear)
2. Melakukan registrasi admin, menentukan nama database dan password database  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/cara%20pemakaian/1.png?raw=true"></img>
3. Mengisi informasi pengguna beserta password pengguna  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/cara%20pemakaian/2.png?raw=true"></img>
4. Sebelum menggunakan dotclear, login terlebih dahulu  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/cara%20pemakaian/login.JPG?raw=true"></img>
5. Setelah itu akan ditampilkan halaman dashboard, yang terdapat berbagai menu yaitu My favorites, Blog, System setting, Plugins  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/cara%20pemakaian/dashboard.JPG?raw=true"></img>
6. Selanjutnya kita membuat postingan blog, klik new entry dan tulis postingan  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/cara%20pemakaian/new%20entry.JPG?raw=true"></img>
7. Setelah postingan di save akan ada pilihan comment, jika kita ingin memberikan komentar maka klik comment  
<img src="https://github.com/haefa/dotclear/blob/master/screenshot/cara%20pemakaian/comment.JPG?raw=true"></img>

# Pembahasan
[`^ kembali ke atas ^`](#)  
**Dotclear** merupakan salah satu aplikasi *open source blog publishing* dan *Content Management System (CMS)* naungan *General Public License (GNU)*. Dotclear ditulis dalam bahasa pemrograman PHP. Dotclear dapat diinstal secara otomatis atau manual dan setelah proses selesai, itu memungkinkan pengguna mengelola aspek yang berbeda dari satu atau beberapa blog. Developer dapat membuat bebarapa blog dalam satu instalasi.

**Kelebihan**
- Publikasi mudah
- Tema yang dapat disesuaikan sepenuhnya
- *User-friendly administration*
- Sistem komentar yang fleksibel
- Dioptimalkan untuk skala besar, sehingga dapat berjalan lancar untuk seribu blog dan seratus ribu komentar
- Dilengkapi dengan *media built-in* sehingga lebih mudah dalam memasukkan file musik dan video

**Kekurangan**
- Fitur keamanan rudimeter
- Tidak cocok untuk proyek perusahaan besar
- Pengelola aset yang sangat terbatas

**Perbandingan dengan Blogging Platform lain**  
Dibandingkan dengan blogging platform lain seperti Wordpress atau Drupal, Dotclear tidak memiliki integrasi dengan sistem atau aplikasi lain. Namun, fitur yang ditawarkan oleh Dotclear lebih beragam jika dibandingkan dengan Wordpress atau Drupal. Dotclear juga tersedia dalam bahasa Inggris dan Prancis, sementara Wordpress dan Drupal hanya tersedia dalam bahasa Inggris.

# Referensi
1. [Dotclear](https://dotclear.org/) - dotclear
2. [ How To Install Dotclear In Ubuntu](https://www.linuxhelp.com/how-to-install-dotclear-in-ubuntu/) - linuxhelp
3. [ Compare Dotclear vs. WordPress](https://comparisons.financesonline.com/wordpress-vs-dotclear) - financesonline
3. [ Compare Dotclear vs. Drupal](https://comparisons.financesonline.com/dotclear-vs-drupal) - financesonline