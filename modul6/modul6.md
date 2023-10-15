# Modul 6 - Model, Controller dan Request-Response Handler

## Model

- ### Langkah 1

  > Mengganti baris kode pada file app/Models/User.php seperti pada gambar
  > ![img1](1.png)

## Controller

- ### Langkah 2

  > Menyalin file ExampleController.php dan mengubah nama file tersebut menjadi HomeController.php beserta baris kode seperti pada gambar
  > ![img1](2.png)

- ### Langkah 3

  > Menngubah route `/` pada file routes/web.php seperti pada gambar
  > ![img1](3.png)

- ### Langkah 4

  > Mengakses halaman web localhost
  > ![img1](4.png)

## Request Handler

- ### Langkah 5

  > Melakukan import library Request dengan menambahkan baris kode seperti pada gambar
  > ![img1](5.png)

- ### Langkah 6

  > Mengubah baris kode pada fungsi index seperti pada gambar
  > ![img1](6.png)

- ### Langkah 7

  > Mengakses halaman web localhost
  > ![img1](7.png)

## Response Handler

- ### Langkah 8

  > Melakukan import library Response dengan menambahkan baris kode seperti pada gambar
  > ![img1](8.png)

- ### Langkah 9

  > Membuat fungsi hello() dan menambahkan baris kode seperti pada gambar
  > ![img1](9.png)

- ### Langkah 10

  > Menambahkan route /hello pada file routes/web.php
  > ![img1](10.png)

- ### Langkah 11

  > Mengakses halaman web localhost dengan endpoint hello
  > ![img1](11.png)

## Penerapan

- ### Langkah 12

  > Melakukan import model User dengan menambahkan baris kode seperti pada gambar
  > ![img1](12.png)

- ### Langkah 13

  > Menambah route middleware dengan baris kode seperti pada gambar
  > ![img1](13.png)

- ### Langkah 14

  > Menambahkan fungsi defaultUser(), createUser(), dan getUser() pada HomeController.php
  > ![img1](14.png)

- ### Langkah 15

  > Menjalankan aplikasi pada postman sesuai endpoint

  A. /default

  > ![img1](15-1.png)

  B. /all

  > ![img1](15-2.png)

  C. /new

  > ![img1](15-3.png)
