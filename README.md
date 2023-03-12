![lencana](https://img.shields.io/badge/Penulis-Rofi-blue)
![lencana](https://img.shields.io/badge/Ditulis%20pada-Minggu,%2012%20Maret%202023-blue)

## Memecahkan file zip yang dilindungi kata sandi menggunakan alat zip2john

Berikut ini adalah langkah-langkah untuk memecahkan file zip yang dilindungi kata sandi menggunakan alat zip2john:

Pertama, kita perlu mengakses hash dari kata sandi yang akan kita pecahkan. Catat nama file zip Anda karena Anda akan diminta untuk menyebutkannya dalam perintah selanjutnya.

Untuk mengakses hash kata sandi, arahkan ke lokasi file zip Anda yang dilindungi kata sandi dan jalankan perintah di bawah ini di terminal:

```
zip2john nama_file.zip
```

![img_1](https://github.com/FII14/CARA-MENGGUNAKAN-ALAT-ZIP2JOHN/blob/main/gambar/IMG_20230304_173920.jpg)

Anda dapat mengekspor hasilnya ke dokumen teks untuk menyimpan hash kata sandi karena kita akan menggunakannya nanti.

```
zip2john nama_file.zip > hash txt
```
![img_2](https://github.com/FII14/CARA-MENGGUNAKAN-ALAT-ZIP2JOHN/blob/main/gambar/IMG_20230304_173438.jpg)


Untuk memulai serangan pada file zip Anda, jalankan perintah di bawah ini:

```
john --format=PKZIP hash.txt
```

Pada perintah di atas, kita sudah menentukan format file target.

Proses pemecahan kata sandi dimulai. Di sinilah kekuatan kata sandi berperan. Semakin kuat kata sandi, semakin banyak waktu yang dibutuhkan untuk melakukan serangan.

Setelah serangan berhasil, kata sandi akan ditampilkan pada terminal.

![img_3](https://github.com/FII14/CARA-MENGGUNAKAN-ALAT-ZIP2JOHN/blob/main/gambar/IMG_20230304_173653.jpg)
