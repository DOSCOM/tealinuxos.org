---
title: Instalasi TealinuxOS
type: panduan
order: 102
---


## Panduan Instalasi TealinuxOS
Ada 2 cara yang bisa Anda lakukan untuk instalisasi TealinuxOS pada perangkat Anda,yaitu:
Untuk menginstall TealinuxOS pada perangkat anda dapat mengikuti 2 cara yaitu :
- Melalui _bootable_ flashdisk
- Melalui _bootable_ CD
Jika Anda menggunakan CD, Anda dapat melewatkan bagian **Unduh ISO TealinuxOS** dan **Membuat bootable ISO TealinuxOS ke Flashdisk**.

### Unduh TealinuxOS
ISO tealinux dapat diunduh [di sini](http://pinguin.dinus.ac.id/iso/tealinuxos/).

### Membuat Bootable ISO TealinuxOS ke Flashdisk
Untuk membuat bootable ke flashdisk anda dapat menggunakan software _Third Party_ seperti [Universal USB Installer](https://universal-usb-installer.en.uptodown.com), [Unetbootin](http://unetbootin.github.io) atau [Rufus](https://rufus.akeo.ie/). Berikut adalah langkah-langkah untuk membuat bootable ISO TealinuxOS ke flashdisk menggunakan Universal USB Installer.
![Bootable_1](https://cloud.githubusercontent.com/assets/22718275/23578142/c4eae682-0102-11e7-9d76-69cd286a4406.png)

![Bootable_2](https://cloud.githubusercontent.com/assets/22718275/23578146/d6ebc932-0102-11e7-94c9-993dee8bcbe2.png)
Mengenai cara penggunaan, instalasi dan keterangan lainya dapat Anda lihat di Website resmi dari masing-masing software tersebut.

### Membuat partisi hardisk untuk TealinuxOS
Untuk membuat partisi hardisk Anda dapat menggunakan `Create and format hard disk partition` milik Windows, `GParted` milik Linux, atau _tools_ lain yang biasa Anda gunakan untuk membuat partisi.
Ada 2 Macam partisi yang dibutuhkan oleh TealinuxOS yaitu :
- Partisi dengan format `ext4`. Partisi ini berfungsi sebagai tempat setiap file system TealinuxOS.
  Sebagai contoh kami membuat partisi sebesar 50GB atau 50000Mb. Klik kanan pada disk yang ingin di _shrink_ (dipecah). Kenapa harus 50GB ?, karena ukuran 50GB itu ukuran yang ideal untuk sistem operasi linux. ukuran minimalnya untuk linux ialah 20GB.
  ![Partition_1](https://cloud.githubusercontent.com/assets/22718275/23578147/e2c49112-0102-11e7-868e-611db63be0a2.png)

  ![Partition_2](https://cloud.githubusercontent.com/assets/22718275/23578150/f11bd6d0-0102-11e7-815c-b4648866def9.png)

- Partisi dengan format `linux-swap`. Partisi ini berfungsi untuk membantu kerja RAM dalam memanajemen memori.
  Untuk ukuran partisi `linux-swap` kami merekomendasikan 2GB.


### Proses Instalasi TealinuxOS
1. Setelah Anda memiliki _bootable_ TealinuxOS, pastikan Anda menghubungkan _bootable_ tersebut ke perangkat anda.
2. Restart perangkat Anda untuk memulai proses instalasi TealinuxOS.
3. Arahkan _booting option_ ke perangkat _bootable_. Anda dapat masuk ke BIOS kemudian ubah mode BIOS ke `Legacy` (jika sebelumnya menggunakan mode `UEFI/EFI`).
4. Selanjutnya ubah boot priority USB HDD(): ke urutan pertama jika anda menggunakan flashdisk atau ubah boot priority CD(): ke urutan pertama jika Anda menggunakan CD.
5. Simpan pengaturan pada BIOS Anda kemudian restart.
6. Tunggu beberapa saat sampai muncul menu seperti berikut :
   ![menu-install](https://cloud.githubusercontent.com/assets/22718275/23685947/5be6f430-03d9-11e7-89c0-d55cfb593f9e.png)
7. Pilih `Try TealinuxOS` untuk mencoba atau `Install TealinuxOS` untuk langsung menginstall. Apabila Anda memilih Install TealinuxOS Anda dapat melewati langkah ke 6 dan 7.
8. Tunggu beberapa saat sampai muncul desktop TealinuxOS seperti berikut :
   ![try-install](https://cloud.githubusercontent.com/assets/22718275/23685964/736151be-03d9-11e7-9b11-23af4063ab3b.png)
   Anda dapat mencoba terlebih dahulu fitur-fitur yang terdapat pada TealinuxOS sebelum menginstallnya. Tetapi jika Anda langsung ingin memasang TealinuxOS, klik icon _Install TealinuxOS_ pada desktop.
9. Selanjutnya akan muncul antarmuka sebagai berikut.
   ![language](https://cloud.githubusercontent.com/assets/22718275/23685988/96e996fa-03d9-11e7-9cc0-b5664ed27a17.png)
   Anda diminta untuk memilih bahasa yang akan digunakan dalam TealinuxOS. Klik ok untuk lanjut.
11. Selanjutnya Anda diminta untuk memilih untuk mendownload _software third party_ atau tidak. Klik ok untuk lanjut.
    ![preparing](https://cloud.githubusercontent.com/assets/22718275/23685998/a811ae18-03d9-11e7-8c6f-1900f9a85b7d.png)
12. Selanjutnya anda diminta untuk memilih prosedur penginstalan sebagai berikut :
    - _Install TeaLinuxOS Alongside Them_
      Pilihan ini dapat menyimpan berkas anda seperti dokumen, dll.
    - _Erase disk and Install TeaLinuxOS_
      Pilihan ini menghapus semua Disk Anda. Pilihan ini dikhususkan bagi Anda yang tidak ingin dualboot, karena pilihan ini akan menghapus semua OS dan data yang ada.
    - _Something else_
      Pilihan ini dikhususkan bagi anda yang ingin dualboot. Karena didalam pilihan ini Anda dapat mengatur partisi yang telah kita buat diawal tadi.
    ![instalaltion](https://cloud.githubusercontent.com/assets/22718275/23686028/cd308aac-03d9-11e7-9fa7-217fd1f7ac08.png)
    Pilih something else lalu klik ok.
13. Anda akan mendapatkan antarmuka seperti berikut :
    ![partiton_1](https://cloud.githubusercontent.com/assets/22718275/23686041/e39d8f38-03d9-11e7-8836-e749fb8b0794.png)
    Seperti yang anda lihat pada antarmuka tersebut, terdapat 2 buah partisi yang anda telah buat pada langkah sebelumnya yaitu `/dev/sda1` yang berukuran 50GB dan `/dev/sda5` yang berukuran 2GB. Sebagai informasi nama partisi dapat berbeda antara tutorial ini dan perangkat anda.
14. Selanjutnya ubah tipe partisi `/dev/sda1` dengan cara klik tombol change. Atur menjadi `ext4`, format partisi dan juga arahkan mount point ke `/`. Klik OK untuk lanjut.
    ![Partition_2](https://cloud.githubusercontent.com/assets/22718275/23686049/f5030230-03d9-11e7-8834-7ecac4b9b6bb.png)
    ![partition_3](https://cloud.githubusercontent.com/assets/22718275/23686061/03f969f0-03da-11e7-8bda-eb56c7c8cf04.png)
15. Selanjutnya ubah tipe partisi `/dev/sda5` dengan cara klik tombol change. Atur menjadi `swap area`. Klik OK untuk lanjut.
    ![Partition_4](https://cloud.githubusercontent.com/assets/22718275/23686081/1fbf6266-03da-11e7-8daa-4a60c06703e5.png)
    ![partition_5](https://cloud.githubusercontent.com/assets/22718275/23686146/6dbf052a-03da-11e7-85e3-e844b273f694.png)
16. Selanjutnya akan tampil persetujuan sebagai berikut :
    ![Partition_6](https://cloud.githubusercontent.com/assets/22718275/23686161/857a51e2-03da-11e7-8011-a9fb063761b4.png)
    Klik continue untuk lanjut.
17. Selanjutnya Anda diminta untuk memilih waktu dan tempat.
    ![time-and-region](https://cloud.githubusercontent.com/assets/22718275/23686187/a58ca03e-03da-11e7-827a-01f86abe8ec3.png)
18. Selanjutnya Anda diminta untuk memilih tipe keyboard.
    ![keyboard](https://cloud.githubusercontent.com/assets/22718275/23686208/b682f4ce-03da-11e7-8dcb-85c8ef2cbbad.png)
19. Selanjutnya Anda diminta untuk mengisi data diri.
    ![whoru](https://cloud.githubusercontent.com/assets/22718275/23686238/d5fdd5e4-03da-11e7-8387-626587c4ede8.png)
20. Tunggu beberapa saat proses sampai proses instalasi tealinuxos selesai.
    ![installaltion](https://cloud.githubusercontent.com/assets/22718275/23686286/31ab73ec-03db-11e7-8292-173401c6851a.png)
21. Restart dan nikmati tealinuxos.
    ![success](https://cloud.githubusercontent.com/assets/22718275/23686381/df3fda20-03db-11e7-9ee1-a811f1646f36.png)
