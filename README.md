# Dirb - Alat Pemindaian Direktori dan File

Dirb adalah alat open source yang digunakan untuk melakukan pemindaian direktori dan file pada aplikasi web. Alat ini membantu dalam mengidentifikasi direktori dan file yang mungkin tersembunyi atau tidak diakses secara langsung.

## Instalasi

1. Pastikan Anda telah menginstal Kali Linux di sistem Anda.

2. Buka terminal di Kali Linux.

3. Untuk menginstal Dirb, jalankan perintah berikut:

```
sudo apt-get install dirb
```

4. Dirb telah diinstal dan siap digunakan.

## Penggunaan

1. Buka terminal di Kali Linux.

2. Untuk memulai pemindaian direktori dan file, jalankan perintah berikut:

```
dirb <URL> <wordlist>
```

Ganti `<URL>` dengan URL target yang ingin Anda pindai, dan `<wordlist>` dengan jalur ke file daftar kata-kata yang akan digunakan oleh Dirb untuk melakukan pemindaian. Misalnya:

```
dirb http://example.com /usr/share/dirb/wordlists/common.txt
```


3. Dirb akan memulai pemindaian pada URL target yang diberikan dengan menggunakan daftar kata-kata yang ditentukan. Proses ini dapat memakan waktu tergantung pada kompleksitas target dan kecepatan koneksi internet.

4. Setelah Dirb selesai melakukan pemindaian, Anda akan melihat hasilnya di terminal. Dirb akan menampilkan daftar direktori dan file yang ditemukan bersama dengan kode respons HTTP yang terkait.

5. Anda juga dapat menggunakan opsi tambahan dengan perintah Dirb untuk mengatur pemindaian yang lebih spesifik. Beberapa opsi yang berguna adalah:

- Opsi `-r` untuk menampilkan hasil dengan format rekursif.
- Opsi `-o` untuk menyimpan hasil pemindaian ke file.
- Opsi `-X` untuk mengatur ekstensi file yang akan dipindai.
- Opsi `-S` untuk mengatur ukuran maksimum file yang akan dipindai.

Misalnya:

```
dirb http://example.com /usr/share/dirb/wordlists/common.txt -r -o scan_result.txt -X .php -S 500KB
```

6. Penting untuk diingat bahwa penggunaan alat pemindaian seperti Dirb harus dilakukan dengan izin dan pada sistem yang Anda memiliki otoritas. Pastikan Anda menggunakan alat ini dengan bijak dan sesuai dengan aturan yang berlaku.
