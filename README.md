## Memecahkan file zip yang dilindungi kata sandi menggunakan alat zip2john

Berikut ini adalah langkah-langkah untuk memecahkan file zip yang dilindungi kata sandi menggunakan alat zip2john:

Pertama, kita perlu mengakses hash dari kata sandi yang akan kita pecahkan. Catat nama file zip Anda karena Anda akan diminta untuk menyebutkannya dalam perintah selanjutnya.

Untuk mengakses hash kata sandi, arahkan ke lokasi file zip Anda yang dilindungi kata sandi dan jalankan perintah di bawah ini di terminal:

```
zip2john nama_file.zip
```

![img_1]()

Anda dapat mengekspor hasilnya ke dokumen teks untuk menyimpan hash kata sandi karena kita akan menggunakannya nanti.

```
zip2john nama_file.zip > hash txt
```
![img_2]()


Untuk memulai serangan pada file zip Anda, jalankan perintah di bawah ini:

```
john --format=PKZIP hash.txt
```

![img_3]()

Pada perintah di atas, kita sudah menentukan format file target.

Proses pemecahan kata sandi dimulai. Di sinilah kekuatan kata sandi berperan. Semakin kuat kata sandi, semakin banyak waktu yang dibutuhkan untuk melakukan serangan.

Setelah serangan berhasil, kata sandi akan ditampilkan pada terminal.
