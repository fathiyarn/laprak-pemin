# Modul 3 - Integrasi MongoDB dan Express

## Instalasi NodeJS

- ### Langkah 1

  > Membuka halaman https://nodejs.org/en/ untuk mendownload dan menjalanan node setup

- ### Langkah 2

  > Menjalankan command node -v untuk memeriksa apakah NodeJS sudah terinstall
  > ![img1](1.1.png)

## Inisiasi project Express dan Pemasangan Package

- ### Langkah 1

  > Membuat folder baru dengan nama express-mongodb dan membuka nya melalui terminal/cmd

- ### Langkah 2

  > Melakukan npm init untuk mengenerate file package.json dengan menggunakan command `npm init -y` ` ` > ![img1](2.1.png)

- ### Langkah 3

  > Melakukan instalasi express, mongoose, dan dotenv dengan menggunakan command `npm i express mongoose dotenv` > ![img1](2.2.png)

## Koneksi Express ke MongoDB

- ### Langkah 1

  > Membuat file baru dengan nama index.js pada root folder dan memasukkan kode seperti perintah di modul, serta menjalankan aplikasi menggunakan command `node index.js` > ![img1](3.1.png)

- ### Langkah 2

  > Melakukan pembuatan file .env dan memasukkan value PORT. Setelah itu mengubah kode pada listening port (index.js) dan menjalankan aplikasi lagi
  > ![img1](3.2.png)

- ### Langkah 3

  > Meng-copy connection string pada compas atau atlas dan paste pada file .env
  > ![img1](3.3.png)

- ### Langkah 4

  > Menambahkan baris kode seperti perintah di modul dan menjalankan aplikasi lagi
  > ![img1](3.4.png)

## Pembuatan Routing

- ### Langkah 1

  > Membuat direktori routes di tingkat yang sama dengan index.js dan membuat file book.route.js di dalamnya
  > ![img1](4.1.png)

- ### Langkah 2

  > Menambahkan baris kode seperti perintah di modul untuk fungsi getAllBooks
  > ![img1](4.2.png)

- ### Langkah 3

  > Menambahkan baris kode untuk getOneBook, createBook, updateBook, dan deleteBook
  > ![img1](4.3.png)

- ### Langkah 4

  > Melakukan insert buku “The Setting Sun” dan “Hujan” dengan command `db.books.insertMany(<data kalian>)` > ![img1](4.4.png)

- ### Langkah 5

  > MeLakukan pencarian semua buku dengan menggunakan command `db.books.find() ` > ![img1](15.png)

- ### Langkah 6

  > Menampilkan seluruh buku author “Osamu Dazai” dengan mengisi argument pada find()
  > ![img1](16.png)

- ### Langkah 9

  > Melakukan perubahan summary pada buku “Hujan” menjadi “Buku yang bagus (NAMA, NIM)”
  > ![img1](17.png)

- ### Langkah 10

  > Melakukan perubahan publisher menjadi “Yen Press” pada semua buku “Osamu Dazai”
  > ![img1](19.png)

- ### Langkah 11

  > Melakukan penghapusan pada buku “Overlord I” dengan menggunakan command `db.books.deleteOne({<argument>})` > ![img1](20.png)

- ### Langkah 12
  > Melakukan penghapusan pada semua buku “Osamu Dazai dengan menggunakan command `db.books.deleteMany({<argument>})` > ![img1](21.png)
