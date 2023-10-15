# Modul 3 - Integrasi MongoDB dan Express

## Instalasi NodeJS

- ### Langkah 1

  Membuka halaman https://nodejs.org/en/ untuk mendownload dan menjalanan node setup

- ### Langkah 2

  Menjalankan command node -v untuk memeriksa apakah NodeJS sudah terinstall
  ![img1](1.1.png)

## Inisiasi project Express dan Pemasangan Package

- ### Langkah 1

  Membuat folder baru dengan nama express-mongodb dan membuka nya melalui terminal/cmd

- ### Langkah 2

  Melakukan npm init untuk mengenerate file package.json dengan menggunakan command `npm init -y` ` `
  ![img1](2.1.png)

- ### Langkah 3

  Melakukan instalasi express, mongoose, dan dotenv dengan menggunakan command `npm i express mongoose dotenv`
  ![img1](2.2.png)

## Koneksi Express ke MongoDB

- ### Langkah 1

  Membuat file baru dengan nama index.js pada root folder dan memasukkan kode seperti perintah di modul, serta menjalankan aplikasi menggunakan command `node index.js`
  ![img1](3.1.png)

- ### Langkah 2

  Melakukan pembuatan file .env dan memasukkan value PORT. Setelah itu mengubah kode pada listening port (index.js) dan menjalankan aplikasi lagi
  ![img1](3.2.png)

- ### Langkah 3

  Meng-copy connection string pada compas atau atlas dan paste pada file .env
  ![img1](3.3.png)

- ### Langkah 4

  Menambahkan baris kode seperti perintah di modul dan menjalankan aplikasi lagi
  ![img1](3.4.png)

## Pembuatan Routing

- ### Langkah 1

  Membuat direktori routes di tingkat yang sama dengan index.js dan membuat file book.route.js di dalamnya
  ![img1](4.1.png)

- ### Langkah 2

  Menambahkan baris kode seperti perintah di modul untuk fungsi getAllBooks
  ![img1](4.3.png)

- ### Langkah 3

  Menambahkan baris kode untuk getOneBook, createBook, updateBook, dan deleteBook
  ![img1](4.4.png)

- ### Langkah 4

  Melakukan import book.route.js pada file index.js dan tambahkan baris kode seperti pada modul
  ![img1](4.5.png)

- ### Langkah 5

  Menguji salah satu endpoint melalui POSTMAN
  ![img1](4.6.png)

## Pembuatan Controller

- ### Langkah 1

  Membuat direktori controllers di tingkat yang sama dengan index.js dan membuat file book.controller.js di dalamnya
  ![img1](5.2.png)

- ### Langkah 2

  Meng-copy baris kode dari routes untuk fungsi getAllBooks, getOneBook, createBook, updateBook, dan deleteBook. Setelah itu, melakukan import book.controller.js pada file book.route.js
  ![img1](5.3.png)

- ### Langkah 3

  Melakukan perubahan pada fungsi agar dapat memanggil fungsi dari book.controller.js
  ![img1](5.6.png)

- ### Langkah 4

  Melakukan pengujian lagi dan pastikan response tetap sama
  ![img1](5.7.png)

## Pembuatan Model

- ### Langkah 1

  Membuat direktori models di tingkat yang sama dengan index.js dan membuat file book.model.js di dalamnya
  ![img1](6.2.png)

- ### Langkah 2

  Menambahkan baris kode seperti pada modul sesuai dengan tabel di modul
  ![img1](6.3.png)

  ## Operasi CRUD

- ### Langkah 1

  Menghapus semua data pada collection books
  ![img1](7.1.png)

- ### Langkah 2

  Melakukan import book.model.js pada file book.controller.js
  ![img1](7.2.png)

- ### Langkah 3

  Melakukan perubahan pada fungsi createBook
  ![img1](7.3.png)

- ### Langkah 4

  Membuat buku baru "Dilan 1990" seperti pada modul melalui Postman
  ![img1](7.4.1.png)

- ### Langkah 5

  Membuat buku baru "Dilan 1991" seperti pada modul melalui Postman
  ![img1](7.4.2.png)

- ### Langkah 6

  Melakukan perubahan pada fungsi getAllBooks
  ![img1](7.5.png)

- ### Langkah 7

  Melakukan perubahan pada fungsi getOneBook
  ![img1](7.6.png)

- ### Langkah 8

  Menampilkan semua buku melalui Postman
  ![img1](7.7.png)

- ### Langkah 9

  Mampilkan buku Dilan 1990 melalui POSTMAN
  ![img1](7.8.png)

- ### Langkah 10

  Melakukan perubahan pada fungsi updateBook
  ![img1](7.9.png)

- ### Langkah 11

  Mengubah judul buku Dilan 1991 menjadi “<NAMA PANGGILAN> 1991” melalui Postman
  ![img1](7.10.png)

- ### Langkah 12

  Melakukan perubahan pada fungsi deleteBook
  ![img1](7.11.png)

- ### Langkah 13

  Menghapus buku Dilan 1990 melalui POSTMAN
  ![img1](7.12.png)
