### Penjelasan htop dan nmon
1. htop:

htop adalah alat baris perintah yang membantu memantau sumber daya dan kinerja sistem pada Linux.
Lebih baik daripada top dan sering tersedia secara default.

Fitur Utama:

- Tampilan Interaktif: htop memungkinkan untuk memfilter dan mengurutkan proses agar lebih mudah dipahami.
- Tampilan Pohon: Melihat proses dalam bentuk pohon.
- Menghentikan Proses: Menghentikan proses yang bermasalah.

Kelebihan:

- `Tampilan yang Lebih Menarik: htop menampilkan informasi dengan kode warna sehingga lebih terorganisir.
Interaksi dengan Mouse: dapat menggunakan mouse untuk berinteraksi dengan htop.`

Kekurangan:

- `Tidak Ada Output yang Cantik: Jika menginginkan tampilan yang lebih cantik, ada alternatif lain.`

Cara Menginstal htop (Ubuntu/Debian):

```sh
sudo apt install htop
```

2. nmon:

nmon adalah alat yang memberikan informasi rinci tentang proses yang berjalan di sistem.
Cocok untuk administrator sistem yang memerlukan data historis untuk analisis jangka panjang.

Kelebihan:

- `Informasi Lengkap: nmon memberikan semua data yang butuhkan untuk memahami proses di sistem.
Pemantauan Historis: Membuat log penggunaan sumber daya untuk analisis jangka panjang.`

Kekurangan:

- `Tampilan Kurang Menarik: Tidak memberikan tampilan yang cantik.`

Cara Menginstal nmon (Ubuntu/Debian):

```sh
sudo apt install nmon
```

Keduanya memiliki kegunaan yang berbeda, tergantung pada kebutuhan.

### Penjelasan Text Manipulation step by step

1. Grep digunakan mencari kata pada file yang dicari

`Contoh Grep`
![image/04.png](image/04.png)

2. Echo digunakan untuk mencetak string / pesan dari hasil perintah lain

`Contoh Echo`

![image/05.png](image/05.png)

### Penjelasan Install Nginx
Nginx adalah salah satu server web terpopuler di dunia dan berperan sebagai hos dari sebagian situs terbesar dan situs yang memiliki lalu lintas tertinggi di jagad internet. Ini adalah pilihan ringan yang dapat digunakan baik sebagai server web atau proksi balik.

```sh
sudo apt install nginx
```
