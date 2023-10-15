# Modul 5 - Dynamic Route dan Middleware

## Dynamic Route

- ### Langkah 1

  Menambahkan baris kode untuk dynamic routes seperti pada gambar
  ![img1](1-1.png)

- ### Langkah 2

  Mengakses halaman web dari route yang telah dibuat sebelumnya
  ![img1](1-2.png)
  ![img1](1-3.png)

- ### Langkah 3

  Menambahkan paramater pada routes dengan baris kode seperti pada gambar
  ![img1](2-1.png)

- ### Langkah 4

  Mengakses halaman web dari route dengan parameter variabel tambahan
  ![img1](2-2.png)

- ### Langkah 5

  Menambahkan optional routes dengan kode baris seperti pada gambar
  ![img1](3-1.png)

- ### Langkah 6

  Mengakses halaman web optional routes dengan parameter variabel dan tanpa parameter variabelnya
  ![img1](3-2.png)
  ![img1](3-3.png)

## Aliases Route

- ### Langkah 7

  Menambahkan aliases route dengan kode baris seperti pada gambar
  ![img1](4-1.png)

- ### Langkah 8

  Mengakses halaman web /auth/login dan /profile
  ![img1](4-3.png)
  ![img1](4-4.png)

## Group Route

- ### Langkah 9

  Menambahkan group route dengan kode baris seperti pada gambar
  ![img1](5-1.png)

- ### Langkah 10

  Mengakses halaman web /users yang menggunakan metode grouping
  ![img1](5-2.png)

## Middleware

- ### Langkah 11

  Menyalin file `ExampleMiddleware` pada `app/Http/Middleware` dan mengubah nama file tersebut menjadi `AgeMiddleware`, kemudian memasukkan baris kode seperti pada gambar
  ![img1](6-1.png)

- ### Langkah 12

  Mendaftarkan `AgeMiddleware` pada aplikasi di dalam file `bootstrap/app.php`
  ![img1](6-2.png)

- ### Langkah 13

  Menambah route middleware dengan baris kode seperti pada gambar
  ![img1](6-3.png)

- ### Langkah 14

  Mengakses halaman web /admin/home/ dan /fail. Halaman web /admin/home/ akan dialihkan menuju halaman web /fail karena tidak terdapat parameter umur pada route nya
  ![img1](6-4.png)
