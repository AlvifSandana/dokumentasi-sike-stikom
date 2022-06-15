# Installation Guide

## Linux

1. Clone project dari repository [berikut](https://github.com/AlvifSandana/keuangan-stikom) :
```bash
cd /var/www/html
git clone https://github.com/AlvifSandana/keuangan-stikom.git
```
2. Install `composer`, keterangan lebih lanjut bisa diakses di laman resmi [Composer](https://getcomposer.org/).
3. Masuk ke dalam folder `keuangan-stikom`, lalu install `dependencies` menggunakan `composer` yang telah diinstall pada tahap sebelumnya.
```bash
cd keuangan-stikom
composer install
```
4. Copy file `env` dan ubah menjadi `.env`, lalu ubah konfigurasi sesuai kebutuhan menggunakan teks editor.
```bash
cp env .env
nano .env
```
5. Buat database baru dengan nama sesuai dengan konfigurasi yang Anda tulis pada file `.env` sebelumnya. 
6. Migrasi tabel database dengan `command` berikut :
```bash
php spark migrate
```
7. `Seed` tabel dengan `dummy data` dengan perintah berikut :
```bash
php spark db:seed TestSeeder
```
8. Atur VirtualHost (Apache) atau Server Blocks (Nginx) sesuai kebutuhan.
9. Login dengan `username = admin@example.com` dan `password = 12345678` (credential ini dapat diubah pada file `app/Database/Seeds/UserSeeder.php`)

## Windows (XAMPP)

1. Install `XAMPP`.
2. Install `Composer`.
3. Buka `Explorer`, lalu arahkan ke `C:\xampp\htdocs`.
4. Tekan dan tahan tombol `Shift` lalu klik kanan, pilih `Open Command Window here`.
5. Setelah `cmd` atau `Poweline` terbuka, clone project dari [repositori](https://github.com/AlvifSandana/keuangan-stikom) berikut.
6. Masuk ke dalam folder `keuangan-stikom`, lalu install `dependencies` menggunakan `composer` yang telah diinstall pada tahap sebelumnya.
```bash
cd keuangan-stikom
composer install
```
7. Copy file `env` dan ubah menjadi `.env`, lalu ubah konfigurasi sesuai kebutuhan menggunakan teks editor.
```bash
cp env .env
nano .env
```
8. Buat database baru dengan nama sesuai dengan konfigurasi yang Anda tulis pada file `.env` sebelumnya.
9. Migrasi tabel database dengan `command` berikut :
```bash
php spark migrate
```
10. `Seed` tabel dengan `dummy data` dengan perintah berikut :
```bash
php spark db:seed TestSeeder
```
11. Atur VirtualHost (Apache) atau Server Blocks (Nginx) sesuai kebutuhan.
12. Login dengan `username = admin@example.com` dan `password = 12345678` (credential ini dapat diubah pada file `app/Database/Seeds/UserSeeder.php`)