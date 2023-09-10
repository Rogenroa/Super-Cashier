# Super-Cashier
Pembuatan tugas Project Pyhton pada kurikulum Pacmaan Academy

# Latar Belakang
Roger adalah seorang pemilik supermarket besar di salah satu kota di Indonesia. Roger memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu Roger akan membuat sistem kasir yang dapat berjalan dengan self-service di supermarket miliknya. Sehingga customer bisa langsung memasukan item yang dibeli, jumlah item item yang dibeli, dan harga item yang dibeli serta tidak menutup kemungkinan adanya tambahan fitur lainnya.

Setelah Roger melakukan riset, nampaknya dia membutuhkan sebuah program yang memang diset sesuai dengan kebutuhan tersebut.

Program Super Cashier ini dirancang untuk bisa menjawab kebutuhan Roger tersebut.
Modul dibuat dengan menerapkan Object Oriented Programming, function, try-except, documentation, dan prinsip clean code.

# Objektif
Membuat sistem kasir self-service dengan alur belanja berikut:
1. Customer membuat ID transaksi customer

2. Customer memasukkan nama item, jumlah item, dan harga item yang ingin dibeli

3. Jika ternyata ada kesalahan dalam memasukkan nama item, jumlah item, atau harga item, customer bisa melakukan update item:
a. Update nama item
b. Update jumlah item
c. Update harga item

4. Jika batal membeli suatu item, customer bisa melakukan hapus item dengan 2 metode:
a. Hapus 1 item
b. Hapus seluruh item pada transaksi (reset transaksi)

5. Jika sudah selesai berbelanja, tetapi masih ada keraguan apakah nama item , jumlah item, dan harga item yang diinput sudah benar, customer bisa melakukan check order dengan output sebagai berikut:
a. Mengeluarkan pesan "Pemesanan sudah benar" jika tidak ada kesalahan input.
b. Mengeluarkan pesan "Terdapat kesalahan input jumlah/harga. Mohn cek ulang pesanan" jika terjadi kesalahan input.
c. Menampilkan tabel berisi seluruh data pesanan yang sudah diinput

6. Terakhir, customer bisa menampilkan total biaya belanja yang harus dibayarkan  dan diskon yang didapatkan sesuai dengan total biaya belanja.

# Flowchart & Code Related
![FlowChart](https://github.com/Rogenroa/Super-Cashier/assets/78997992/1f461c67-6b9b-4a79-9936-ef281aa9b5c6)

# Penjelasan dari Function

1. init()

Fungsi inisialisasi untuk class Transaction
dict_txn (dict) = dictionary untuk menyimpan data transaksi (dict)
txn_valid (boolean) = untuk menandai apakah data yang diinput ke dalam dictionary transaksi sudah valid. Nilai awal adalah True dan bisa berubah False setelah dicek validitasnya lewat fungsi.

2. add_item(nama, jumlah, harga)

Fungsi untuk menambahkan item ke dalam dictionary transaksi.
nama (String, key) = nama item yang dibeli, key dalam dictionary
jumlah (int) = jumlah item yang dibeli
harga (int) = harga per item

3. update_item_name(nama, nama_baru)

Fungsi untuk mengubah nama item dalam dictionary yang sudah diinput.
nama (String) = nama item sebelum diganti, key dari dictionary
nama_baru (String) = nama baru untuk item, menjadi key baru dari dictionary

4. update_item_qty(nama, jumlah_baru)

Fungsi untuk mengubah jumlah item dalam dictionary yang sudah diinput.
nama (String) = nama item yang ingin diubah jumlahnya, key dari dictionary
jumlah_baru (int) = jumlah baru dari nama item yang dibeli

5. update_item_price(nama, harga_baru)

Fungsi untuk mengubah harga item dalam dictionary yang sudah diinput.
nama (String) = nama item yang ingin diubah jumlahnya, key dari dictionary
harga_baru (int) = harga baru dari nama item yang dibeli

6. delete_item(nama)

Fungsi untuk menghapus data nama item beserta jumlah dan harganya dari dictionary.
nama (String) = nama item yang ingin dihapus

7. reset_transaction()

Fungsi untuk menghapus semua data pesanan dalam dictionary.

8. print_order()

Fungsi untuk menampilkan semua pesanan dalam dictionary.

9. check_order()

Fungsi untuk mengecek validitas dan menampilkan semua pesanan dalam dictionary.

10. total_price()

Fungsi untuk menampilkan semua pesanan dan total belanja.

# Hasil Test Case

Test Case 1. Menambahkan Item
![Test Case1](https://github.com/Rogenroa/Super-Cashier/assets/78997992/c4a712e9-f2fd-4128-ad84-6166c03007f7)

Test Case 2. Menghapus Item
![Test Case2](https://github.com/Rogenroa/Super-Cashier/assets/78997992/a9a6bcc3-9bd3-4f7b-91e8-35c0315b0581)

Test Case 3. Menghapus Seluruh Pesanan
![Test Case3](https://github.com/Rogenroa/Super-Cashier/assets/78997992/d5b03324-012c-409b-b2fe-7c38fb4d9bb6)

Test Case 4. Menghitung total belanja yang harus dibayarkan dan mencek jumlah diskon sesuai program
![Test Case4](https://github.com/Rogenroa/Super-Cashier/assets/78997992/9bc2e348-ef2c-412f-b29c-2f59f4d8a161)

Test Case 5. Mengupdate item name, jumlah item, harga item (tambahan)
![Test Case5](https://github.com/Rogenroa/Super-Cashier/assets/78997992/36f6882b-d393-4fb1-b3f6-9e42d52154f9)

# Kesimpulan
Program ini tentu masih jauh dari sempurna, masih banyak fitur yang mungkin bisa ditambahkan untuk menyempurnakan program self service cashier ini
Tapi ini bisa menjadi fundamental yang baik dalam proses pengembangan kedepannya karena secara overall seluruh requirement yang disampaikan didepan
sudah berhasil diselesaikan oleh program ini
