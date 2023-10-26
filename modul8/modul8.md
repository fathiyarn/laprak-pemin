# Modul 7 - Register, Authentication dan Authorization

## Register

- ### Langkah 1

  Memastikan terdapat tabel users yang dibuat menggunakan migration pada praktikum 4 Basic Routing dan Migration
  ![img1](1.png)

- ### Langkah 2

  Memastikan terdapat model User.php yang digunakan pada praktikum 6 Model, Controller dan Request-Response Handler
  ![img1](2.png)

- ### Langkah 3

  Membuat file AuthController.php dan menambahkan baris kode seperti pada gambar
  ![img1](3.png)

- ### Langkah 4

  Menambahkan baris kode rute baru pada routes/web.php
  ![img1](4.png)

- ### Langkah 5

  Menjalankan aplikasi dengan endpoint /auth/register dan method post
  ![img1](5.png)

## Authentication

- ### Langkah 6

  Membuat fungsi login(Request $request) pada file AuthController.php
  ![img1](6.png)

- ### Langkah 7

  Menambahkan baris kode rute baru pada routes/web.php
  ![img1](7.png)

- ### Langkah 8

  Menjalankan aplikasi pada endpoint /auth/login dengan method post

  A. Email & Password Benar
  ![img1](8.png)

  B. Email atau Password Salah
  ![img1](9.png)

## Token

- ### Langkah 9

  Menjalankan perintah `php artisan make:migration add_column_token_to_users` untuk membuat migrasi baru
  ![img1](10.png)

- ### Langkah 10

  Menambahkan baris kode seperti pada gambar di dalam file migrasi yang baru dibuat
  ![img1](11.png)

- ### Langkah 11

  Menambahkan baris kode seperti pada gambar di dalam file AuthController.php
  ![img1](12.png)

- ### Langkah 12

  Menjalankan perintah `php artisan migrate` untuk menjalankan migrasi terbaru
  ![img1](13.png)

- ### Langkah 13

  Menjalankan aplikasi pada endpoint /auth/login dengan method post
  ![img1](14.png)

## Authorization

- ### Langkah 14

  Membuat file Authorization.php pada folder App/Http/Middleware dan menambah baris kode seperti pada gambar
  ![img1](15.png)

- ### Langkah 15

  Menambahkan middleware Authorization pada bootstrap/app.php
  ![img1](16.png)

- ### Langkah 16

  Membuat fungsi home() pada HomeController.php
  ![img1](17.png)

- ### Langkah 17

  Menambahkan baris kode untuk rute middleware pada routes/web.php
  ![img1](18.png)

- ### Langkah 18

  Menjalankan aplikasi pada postman dengan endpoint /home dan menambahkan nilai token --yang didapat dari login sebelumnya-- pada header
  ![img1](19.png)
