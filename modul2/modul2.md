# Modul 2 - CRUD MongoDB Compass dan Shell

## MangoDB Compass

- ### Langkah 1

  > Melakukan koneksi ke MangoDB menggunakan connection string secara local
  > ![img1](modul2/1.png)

- ### Langkah 2

  > Membuat database baru dengan mengklik "Create Database"
  > ![img1](modul2/2.png)

- ### Langkah 3

  > Melakukan insert buku pertama dengan melakukan klik “Add Data”, pilih “Insert Document”, mengisi dengan data yang diinginkan dan klik “Insert”
  > ![img1](modul2/3.png)

- ### Langkah 4

  > Melakukan insert buku kedua dengan cara yang sama seperti langkah 3.
  > ![img1](modul2/4.png)

- ### Langkah 5

  > Melakukan pencarian buku dengan author “Osamu Dazai” dengan mengisi filter yang diinginkan dan klik “Find”
  > ![img1](modul2/5.png)

- ### Langkah 6

  > Melakukan perubahan summary pada buku “No Longer Human” menjadi “Buku yang bagus (<NAMA>,<NIM>) dengan melakukan klik “Edit Document” (berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik “Update”
  > ![img1](modul2/6.png)

- ### Langkah 7
  > Menghapus buku “I Am a Cat” dengan melakukan klik “Remove Document” (berlambang tong sampah) dan melakukan klik “Delete”
  > ![img1](modul2/8.png)

## MangoDB Shell

- ### Langkah 1

  > Melakukan koneksi ke MongoDB Server dengan menjalankan command `mongosh`
  > ![img1](modul2/9.png)

- ### Langkah 2

  > Melihat list database yang ada di server dengan menjalankan command `show dbs`
  > ![img1](modul2/10.png)

- ### Langkah 3

  > Berpindah ke database “bookstore” gunakan command `use bookstore`
  > ![img1](modul2/11.png)

- ### Langkah 4

  > Melihat collection yang ada pada database tersebut dengan menggunakan command `show collections`
  > ![img1](modul2/12.png)

- ### Langkah 5

  > Melakukan insert buku “Overlord I” dengan menggunakan command `db.books.insertOne(<data kalian>)`
  > ![img1](modul2/13.png)

- ### Langkah 6

  > Melakukan insert buku “The Setting Sun” dan “Hujan” dengan command `db.books.insertMany(<data kalian>)`
  > ![img1](modul2/14.png)

- ### Langkah 7

  > MeLakukan pencarian semua buku dengan menggunakan command `db.books.find() `
  > ![img1](modul2/15.png)

- ### Langkah 8

  > Menampilkan seluruh buku author “Osamu Dazai” dengan mengisi argument pada find()
  > ![img1](modul2/16.png)

- ### Langkah 9

  > Melakukan perubahan summary pada buku “Hujan” menjadi “Buku yang bagus (NAMA, NIM)”
  > ![img1](modul2/17.png)

- ### Langkah 10

  > Melakukan perubahan publisher menjadi “Yen Press” pada semua buku “Osamu Dazai”
  > ![img1](modul2/19.png)

- ### Langkah 11

  > Melakukan penghapusan pada buku “Overlord I” dengan menggunakan command `db.books.deleteOne({<argument>})`
  > ![img1](modul2/20.png)

- ### Langkah 12
  > Melakukan penghapusan pada semua buku “Osamu Dazai dengan menggunakan command `db.books.deleteMany({<argument>})`
  > ![img1](modul2/21.png)
