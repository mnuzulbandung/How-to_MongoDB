# **Basic MongoDB Atlas Tutorial**

## A. Membuat Cluster baru
1.	Dalam homepage, klik `Create`.
2.	Di laman baru, klik `M0` untuk menggunakan Cluster versi gratis; pilih `Provider AWS`; masukkan dama Cluster; klik `Create Deployment`. (Ceklis `Automate security setup` dan `Preload sample dataset` jika dibutuhkan)
3.	Di laman baru, untuk membuat/mengatur user yang bakal mengakses Cluster, masukkan username dan passsword lalu kllik `Create Database User`. Jika sudah selesai, klik `Close`. Pembuatan/pengaturan user yang bisa mengakses Cluster juga bisa dilakukan dengan, pada bagian `Security`; klik `Quickstart`; pilih `Username and Password`.
4.	Pengaturan perangkat yang bisa mengakses Cluster dapat dilakukan dengan, pada bagian `Security`; klik `Quickstart`; pilih `My Local Environment`; masukkan `IP Address` dan `Description` atau klik `Add My Current IP Address`; lalu klik `Add Entry`.

## B. Memasukkan data ke dalam Cluster
1.	Di menu bar sebelah kiri, klik `Overview`. Di bagian tengah, pilih `Add Data` atau `Load Sample Data`.
2.	Untuk melihat data yang sudah masuk, pada bagian `Overview`, klik `Browse collections`.
3.	Di bagian `Collections`, `sample_mflix` adalah nama database, `comments` adalah nama collection.
4.	Untuk melihat informasi dari masing-masing Collection pada `sample_mflix`; klik `sample_mflix`.

## C. Membuat database
1.	Pada menu bar di bagian `DATABASE`; klik `Clusters`; pilih cluster yang akan dibuat database baru.
2.	Di laman baru, pilih bagian `Collections`; klik `Create Database`.
3.	Di laman baru, masukkan informasi nama database, nama collection.

## D. Membuat collection
1.	Pada menu bar di bagian `DATABASE`; klik `Clusters`; pilih cluster yang akan dibuat collection baru.
2.	Di laman baru, pilih bagian `Collections`; pilih database yang akan dibuat collection baru; klik `Create Collection`.
3.	Di laman baru, masukkan informasi nama collection.

## E. Menambahkan document
1.	Pada menu bar di bagian `DATABASE`; klik `Clusters`; pilih cluster tempat document baru.
2.	Di laman baru, pilih bagian `Collections`; pilih database tempat document baru, pilih collection yang akan dibuat document baru; klik `Insert Document`.
3.	Di laman baru, masukkan data dengan format JSON.
* Contoh:
    ```json
    "Name": "Adi",
    "Age_Group": "Teenager",
    "Purchase": ["Apple", "Berry", "Cherry"]}

    "Name": "Budi",
    "Age_Group": "Teenager",
    "Purchase": ["Date"]}
    ```

## F. Query
1.	Pada laman cellection, masukkan script tertentu di kolom `Filter`, lalu klik `apply`. Kunjungi laman [ini](https://github.com/mnuzulbandung/How-to_MongoDB/blob/main/MongoDB_Query.md) untuk tutorial query.

# **Basic MongoDB Compass Tutorial**

## Menghubungkan MongoDB Atlas dengan MongoDB Compass.
1.	Untuk mengetahui versi dari MongoDB Compass, pada MongoDB Compass, klik `Help`; klik `About`; lihat versi MongoDB Compass.
2.	Pada MongoDB Atlas, pada menu bar sbelah kiri, pada bagian `Database`, klik `Cluster`; di bagian tengah, pilih Cluster yang akan dihubungkan; pilih `Connect`.
3.	Di laman baru, pilih `Compass`.
4.	Di laman baru, pilih `I have MongoDB Compass Installed`; pilih versi MongoDB Compass sesuai apa yang dimiliki; copy link dan ubah db_password.
5.	Pada MongoDB Compass, klik `Add new connection`; masukkan link dari poin 4; klik `Save & Connect`.
