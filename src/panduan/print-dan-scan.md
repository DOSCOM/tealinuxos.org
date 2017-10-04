---
title: Print dan Scan
type: panduan
order: 108
---

## Penggunaan Printer

 Kebanyakan printer secara otomatis didukung oleh TeaLinuxOS Pappermint. Aplikasi Konfigurasi Printer memungkinkan Anda untuk menambahkan printer, serta mengubah pengaturan mereka. Anda juga dapat menggunakan aplikasi ini untuk berbagi printer dengan komputer lain di jaringan, menonaktifkan printer atau restart.

### Print Lokal

-    Dapatkan nama model printer Anda
-    Pastikan printer sudah hidup
-    ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Setting → Setting Manager → Printers`
-    Klik `→ Server → New → Printer`
-    Printer Anda harus secara otomatis terdeteksi dan ditampilkan dalam jendela Devices
-    Pilih printer Anda dan klik Forward
-    Komputer Anda akan mencari dan menginstal driver untuk printer Anda
-    Anda dapat memasukkan deskripsi dan lokasi untuk printer Anda
-    Tekan `Apply`
-    Printer Anda harus dikonfigurasi dengan benar pada saat ini dan Anda akan diminta jika Anda ingin mencetak halaman uji
-    Jika Anda menekan tombol Print Test Page, halaman uji akan mencetak dan Anda dapat memverifikasi apakah itu dicetak dengan benar, atau Anda dapat menekan Batal.
-    Jika Anda masih mengalami masalah, cobalah menggunakan antarmuka berbasis browser CUPS. Hal ini dapat diakses di http: // localhost: 631 /.

### Print menggunakan jaringan

-    Dapatkan nama model printer Anda
-    Pastikan printer sudah hidup
-   ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Setting → Setting Manager → Printers`
-    Klik `→ Server → New → Printer`
-    Klik pada Network Printer di jendela Devices
-    Jika printer Anda terhubung langsung ke mesin Windows di jaringan Anda, pilih Windows Printer via SAMBA. Jika tidak, pilih protokol printer Anda menggunakan untuk berkomunikasi.
-    Masukkan rincian printer jaringan dan tekan Teruskan
-    Pilih produsen printer dan kemudian tekan Teruskan
-    Pilih model printer dan driver kemudian tekan Teruskan
-    nda dapat memasukkan deskripsi dan lokasi untuk printer Anda di bidang yang sesuai
-    Tekan `Apply`
-    Printer Anda dikonfigurasi dengan benar pada saat ini dan Anda akan diminta untuk mencetak halaman uji, tekan Batal atau Print Test Page tergantung pada preferensi Anda

## Penggunaan Scanner

 Banyak scanner telah didukung oleh TeaLinuxOS Pappermint, sehingga mudah dalam penginstallan dan pengoperasiannya.
 
Scan dokumen

-    Tempatkan dokumen yang ingin di scan ke scanner
-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
  `→ Graphics → Simple Scan`
-    Klik `Document → Scan`
-    Pilih media yang ingin anda scan: Single Page, All Pages From Feeder, Text or Photo. Bergantian, tekan tombol Scan pada pemindai cara ini seharusnya bisa berhasil.









