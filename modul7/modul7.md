# Modul 7 - Relasi One-to-Many dan Many-to-Many

## Pembuatan Tabel

- ### Langkah 1

  Mengaktifkan server database dan membuat database dengan nama `lumenpost`
  ![img1](1.png)

- ### Langkah 2

  Mengubah konfigurasi database pada file .env seperti pada gambar
  ![img1](2.png)

- ### Langkah 3

  Menghidupkan beberapa library pada file app.php
  ![img1](3.png)

- ### Langkah 4

  Menjalankan command seperti pada gambar untuk membuat file migration
  ![img1](4.png)

- ### Langkah 5

  Mengubah fungsi `up()` pada file `create_posts_table`
  ![img1](5.png)

- ### Langkah 6

  Mengubah fungsi `up()` pada file `create_comments_table`
  ![img1](6.png)

- ### Langkah 7

  Mengubah fungsi `up()` pada file `create_tags_table`
  ![img1](7.png)

- ### Langkah 8

  Mengubah fungsi `up()` pada file `create_post_tag_table`
  ![img1](8.png)

- ### Langkah 9

  Menjalankan migrasi dengan command seperti pada gambar
  ![img1](9.png)

## Pembuatan Model

- ### Langkah 10

  Membuat file dengan nama Post.php dan menginputkan baris kode seperti pada gambar
  ![img1](10.png)

- ### Langkah 11

  Membuat file dengan nama Comment.php dan menginputkan baris kode seperti pada gambar
  ![img1](12.png)

- ### Langkah 12

  Membuat file dengan nama Tag.php dan menginputkan baris kode seperti pada gambar
  ![img1](11.png)

## Relasi One-to-Many

- ### Langkah 13

  Menambah fungsi comments() pada file Post.php
  ![img1](13.png)

- ### Langkah 14

  Menambahkan fungsi post() dan atribut postId pada `$fillable` di dalam file Comment.php
  ![img1](14.png)

- ### Langkah 15

  Membuat file PostController.php dan menginputkan baris kode seperti pada gambar
  ![img1](15.png)

- ### Langkah 16

  Membuat file CommentController.php dan menginputkan baris kode seperti pada gambar
  ![img1](16.png)

- ### Langkah 17

  Menambahkan baris kode pada router/web.php
  ![img1](17.png)

- ### Langkah 18

  Membuat satu post menggunakan postman
  ![img1](18.png)

- ### Langkah 19

  Membuat satu comment menggunakan postman
  ![img1](19.png)

- ### Langkah 20

  Menampilkan post menggunakan postman
  ![img1](20.png)

## Relasi Many-to-Many

- ### Langkah 21

  Menambah fungsi tags() pada file Post.php
  ![img1](21.png)

- ### Langkah 22

  Menambah fungsi posts() pada file Tag.php
  ![img1](22.png)

- ### Langkah 23

  Membuat file TagController.php dan memasukkan baris kode seperti pada gambar
  ![img1](23.png)

- ### Langkah 24

  Menambah fungsi addTag dan response tags pada PostController.php
  ![img1](24.png)

- ### Langkah 25

  Menambah baris kode pada file routes/web.php seperti pada gambar
  ![img1](25.png)

- ### Langkah 26

  Membuat tag baru menggunakan postman
  ![img1](26.png)

- ### Langkah 27

  Menambah tag "jadul" pada post "disana engkau berdua"
  ![img1](27.png)

- ### Langkah 28

  Menampilkan post "disana engkau berdua" menggunakan postman
  ![img1](28.png)

- ### Langkah 29

  Membuat post baru dengan value "tanpamu apa artinya" menggunakan postman
  ![img1](29.png)

- ### Langkah 30

  Menambah tag "jadul" pada postingan "tanpamu apa artinya"
  ![img1](30.png)

- ### Langkah 31

  Membuat tag "lagu" menggunakan postman
  ![img1](31.png)

- ### Langkah 32

  Menambah tag "lagu" pada post "tanpamu apa artinya"
  ![img1](32.png)

- ### Langkah 33

  Menampilkan post pertama
  ![img1](33.png)

- ### Langkah 34

  Menampilkan post kedua
  ![img1](34.png)
