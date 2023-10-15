# Modul 4 - Basic Routing dan Migration

## GET

- ### Langkah 1

  > Membuka file web.php pada folder routes dan menambahkan kode seperti pada gambar. Kemudian menjalankan aplikasi dengan command `php -S localhost:8000 -t public` pada terminal VSCODE
  > ![img1](1-1.png)

- ### Langkah 2

  > Membuka browser dan mengakses path seperti pada gambar
  > ![img1](1-2.png)

## POST, PUT, PATCH, DELETE, dan OPTIONS

- ### Langkah 3

  > Menambahkan methode POST, PUT, PATCH, DELETE, dan OPTIONS pada file web.php dengan code seperti pada gambar
  > ![img1](2.png)

- ### Langkah 4

  > Melakukan instalasi ekstensi Thunder Client
  > ![img1](3.png)

- ### Langkah 5

  > Mengklik logo petir yang terletak di bar sebelah kiri. Kemudian membuat request baru dengan "New Request"
  > ![img1](4.png)

- ### Langkah 6

  > Memasukkan method dan url sesuai tujuan (path)

  A. GET

  > ![img1](5-1.png)

  B. POST

  > ![img1](5-2.png)

  C. PUT

  > ![img1](5-3.png)

  D. DELETE

  > ![img1](5-4.png)

  E. PATCH

  > ![img1](5-5.png)

  F. OPTIONS

  > ![img1](5-6.png)

## Migrasi Database

- ### Langkah 7

  > Mengakses server database dan membuat database `lumenapi` > ![img1](6.png)

- ### Langkah 8

  > Mengubah konfigurasi database pada file .enf sesuai server yang digunakan. Pada percobaan ini, database menggunakan port 3007 dan tidak memerlukan password
  > ![img1](7.png)

- ### Langkah 9

  > Menghidupkan (menghapus tanda comment) library bawaan lumen pada file app.php di folder bootstrap
  > ![img1](8.png)

- ### Langkah 10

  > Menjalankan command `php artisan make:migration create_users_table` untuk membuat migrasi tabel users dan command `php artisan make:migration create_products_table` untuk membuat migrasi tabel produts
  > ![img1](9.png)

- ### Langkah 11

  > Merubah fungsi up pada file migrasi create_users_table
  > ![img1](10.png)

- ### Langkah 12

  > Merubah fungsi up pada file migrasi create_products_table
  > ![img1](11.png)

- ### Langkah 13

  > Menjalankan command `php artisan migrate` untuk melakukan migrasi tabel yang telah dibuat
  > ![img1](12.png)
