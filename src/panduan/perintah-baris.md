---
title: Perintah Baris
type: panduan
order: 113
---

## Daftar Perintah Umum ##
Untuk menjelajah atau beraktivitas di TealinuxOS atau distro linux lainya selain menggunakan Graphical User Interface (GUI) anda juga dapat menggunakan Command Line Interface(CLI). Berikut ini merupakan beberapa perintah yang umum digunakan dalam CLI.

- Melihat direktori kita berada

  Perintah `pwd` atau print working directory digunakan untuk mengetahui posisi direktori dimana kita berada.
  ```
    $ pwd
  ```

- Pindah Direktori

  Perintah `cd` digunakan untuk mengubah direktori dimana kita berada. cd [nama_direktori] Untuk kembali kedirekroti satu level sebelumnya perintah yang digunakan sebagai berikut.
  ```
    $ cd .
  ```
  Untuk kembali kedirektori root perintahnya sebagai berikut.
  ```
    $ cd ..
  ```

- List

  Perintah `ls` digunakan untuk menampilkan daftar file yang ada di direktori. ls Untuk menampilkan list file yang ada didirektori tertentu
  ```
    $ ls [nama_direktori]
  ```

- Menyalin File

  Perintah `cp` digunakan untuk mengopi file atau direktori ke direktori lain.
  ```
    $ cp [nama_file] [nama_direktori]
  ```

- Memindah File

  Perintah `mv` digunakan untuk memindah file atau direktori ke direktori lain.
  ```
    $ mv [nama_file] [nama_direktori]
  ```

- Menghapus File

  Perintah `rm` digunakan untuk menghapus file atau direktori ke direktori lain.
  ```
    $ rm [nama_file]
  ```

- Penggunaan perintah

  Perintah `man` digunakan untuk menampilkan cara penggunaan suatu perintah.
  ```
    $ man [nama_perintah] man rm
  ```


## Menjalankan Perintah dengan Hak Administrasi
Ketika anda bekerja dengan perintah-perintah baris, beberapa perintah tidak bisa dilakukan tanpa hak administrator, sehingga butuh perintah sudo di awal setiap perintah tersebut. Sesaat setelah anda memberi perintah sudo sistem akan meminta password lalu akan mengingatnya selama 15 menit. Dalam waktu 15 menit ini anda dapat menjalankan perintah sudo tanpa harus mengetik password setiap kali menjalankan perintahnya. ```
  $ sudo apt-get update
```
