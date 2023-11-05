# Modul 8 - JSON Web Token (JWT)

## Penyesuaian Database

- ### Langkah 1

  Melakukan perubahan pada length kolom token dengan menghapus parameter 72 di belakangnya
  ![img1](1.png)

- ### Langkah 2

  Menjalankan perintah `php artisan migrate:fresh` untuk memperbaharui migrasi dan menghapus data yang lama
  ![img1](2.png)

- ### Langkah 3

  Menjalankan aplikasi pada endpoint /auth/register dengan body seperti pada gambar
  ![img1](3.png)

## JWT Manual

- ### Langkah 4

  Menambahkan ketiga fungsi berikut pada AuthController.php
  ![img1](4.png)

- ### Langkah 5

  Melakukan perubahan pada fungsi login
  ![img1](5.png)

- ### Langkah 6

  Menambahkan 4 fungsi baru (base64ur1_encode, base64ur1_decode, sign, dan verify) pada Middleware/Authorization.php
  ![img1](6.png)

- ### Langkah 7

  Melakukan perubahan pada fungsi handle
  ![img1](7.png)

- ### Langkah 8

  Menjalankan aplikasi pada endpoint /auth/login dengan body seperti pada gambar
  ![img1](8.png)

- ### Langkah 9

  Menjalankan aplikasi pada endpoint /home dengan melampirkan nilai token yang didapat pada login sebelumnya
  ![img1](9.png)

## JWT Library

- ### Langkah 10

  Melakukan generate jwt key secara online menggunakan website Djecrety ― Django Secret Key Generator
  ![img1](10.png)

- ### Langkah 11

  Memasukkan secret key tersebut pada file .env dengan membuat variable baru bernama `JWT_SECRET`
  ![img1](11.png)

- ### Langkah 12

  Melakukan instalasi package jwt firebase dengan menggunakan command seperti pada gambar
  ![img1](12.png)

- ### Langkah 13

  Menambahkan fungsi baru pada file AuthController
  ![img1](13.png)

- ### Langkah 14

  Melakukan perubahan pada fungsi login
  ![img1](14.png)

- ### Langkah 15

  Membuat file JwtMiddleware.php dan menambahkan baris kode seperti pada gambar
  ![img1](16.png)

- ### Langkah 16

  Mendaftarkan middleware yang telah dibuat pada bootstrap/app.php
  ![img1](17.png)

- ### Langkah 17

  Menambahkan baris kode untuk rute middleware home pada routes/web.php
  ![img1](18.png)

- ### Langkah 18

  Menjalankan aplikasi pada endpoint /auth/login dengan body seperti pada gambar
  ![img1](19.png)
