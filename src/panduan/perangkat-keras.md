---
title: Perangkat Keras
type: panduan
order: 111
---

## Pembatasan Beberapa Driver

### Mengapa beberapa driver dibatasi?

Pembatasan Driver (Restricted Driver) adalah keterbatasan driver untuk sebuah perangkat hardware karena tidak tersedia secara bebas atau open source.

Kebanyakan device (hardware) yang terpasang di komputer anda bisa berfungsi secara normal di TeaLinuxOS. Device ini cenderung tidak memiliki keterbatasan driver, yang artinya driver dapat dimodifikasi dan masalah dengan device dapat dibetulkan.

Ketika beberapa hardware tidak dapat berjalan lancar di TeaLinuxOS bisa dikarenakan device tersebut memiliki Restricted Driver (Pembatasan Driver). Biasanya pembuat hardware belum merilis detail dari hardware itu sendiri yang memungkinkan untuk developer membuat semacam driver sendiri. Device yang seperti ini mempunyai fungsi yang terbatas atau mungkin tidak bisa berkerja sama sekali.

### Mengaktifkan Pembatasan Driver

Jika Pembatasan Driver tersedia untuk beberapa device, anda dapat menginstalnya untuk memungkinkan perangkat anda berfungsi dengan baik.

Jika beberapa driver tersedia untuk perangkat anda dapat diinstal dari Software Source dialog:

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
   `→ Settings Manager → Software & Updates`
-    Driver yang tersedia akan muncul di tab Additional Drivers, pilih dan Apply Changes
-    Anda akan, jika perlu, memasukan password administration
-    Anda mungkin akan diminta untuk reboot komputer anda setelah proses instalasi selesai

### Menonaktifkan Pembatasan Driver

Jika Pembatasan Driver menyebabkan masalah, anda bisa menonaktifkan, ikuti langkah berikut

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
   `→ Settings Manager → Software & Updates`
-    Klik Additional Drivers
-    Cari driver yang akan dinonaktifkan dan tekan tombol Deactivate
-    Anda akan diminta memasukan password administration



## Disk dan Partition


### Memeriksa berapa ruang disk yang tersisa

Cara mudah untuk memeriksa ruang disk yang tersedia adalah menggunakan File Manager. Berikut beberapa langkah yang harus dilakukan

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
   `→ Accessories → File Manager`
-    Double-click di File System atau icon Home di Desktop
-    Klik folder home di Lancher Panel

Status bar di bagian bawah jendela memperlihatkan ruang tersedia dari drive atau disk yang terpilih. Jika anda memiliki lebih dari satu drive tepasang atau terhubung, anda dapat click di side pane dan anda akan melihat ruang kosong pada drive atau disk tersebut.

### Menambah ruang disk

Beberapa cara mudah untuk meberikan ruang kosong lebih:

-    Kosongkan trash dengan cara klik kanan di Trash icon pada Desktop atau Launcher Panel dan pilih Empty Trash
-    Hapus software package yang tidak digunakan lagi.
-    Hapus file yang tidak dibutuhkan.

### Mempartisi Perangkat

Anda dapat menggunakan GParted (GNOME Partition Editor) untuk mempartisi perangkat penyimpanan. Klik ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Settings Manager → GParted` untuk memulai editor partisi

### Membebaskan ruang untuk partisi baru

Untuk membuat partisi baru di perangkat yang sudah terpatisi, Anda harus mengubah ukuran partisi yang tersedia. Jika Anda sudah mempunyai ruang kosong, lewati langkah ini dan menuju kebagian Membuat partisi baru. Jika tidak, ikuti langkah dibawah:

-    Pilih perangkat yang akan dipartisi dari list drop-down yang terdapat di kanan-atas dari jendela utama
-    List partisi akan muncul di jendela utama. Pilih partisi yang akan anda rubah ukurannya dan dari menu pilih `Partition → Unmount`
-    Untuk merubah partisi pilih `Partition → Resize /Move.` Resize/Move dialog akan muncul. Anda dapat menggunakan Free Space Following (MiB) box untuk memilih berapa banyak ruang yang akan dikosongkan setelah partisi, atau Free Space Preceding (MiB) untuk mengosongkan ruang sebelum partisi ini.
-    Klik `Resize / Move`
-    Untuk menerapkan perubahan, klik `Edit → Apply All Operations`

### Membuat Partisi baru

Untuk membuat partisi baru:

-    Pilih perangkat yang akan dipartisi dari list drop-down di bagian kanan-atas dari jendela utama.
-    List dari partisi akan muncul. Pilih unallocated, klik kanan dan click New
-    Dari File system: pick list, pilih type dari filesystem yang akan digunakan.
-    Jika dibutuhkan, masukkan deskripsi partisi di Label : field
-    Click tombol Add
-    Untuk menerapkan perubahan, klik `Edit → Apply All Operation`

### Memformat Partisi

Untuk menghapus partisi, lakukan langkah berikut:

-    Pilih perangkat dari list drop-down di bagian kanan-atas dari jendela utama
-    List partisi akan muncul. Pilih partisi dan pilih `Partition → Unmount`
-    Pilih partisi yang akan diformat dan pilih `Partition → Format to` dan pilih tipe file system dari list untuk dirubah ke tipe tersebut
-    Untuk menerapkan perubahan, klik `Edit → Apply All Operations`

### Mount dan Unmount perangkat

Ketika anda memasang sebuah perangakat removable storage (ex : Flashdisk) ke komputer anda, harusnya perangkat tersebut akan tersambung (mounted) oleh operating system yang memperbolehkan anda untuk mengakses file di perangkat tersebut

Untuk mencari bagaimana cara mount dan unmount perangkat penyimpanan secara manual dan/atau otomatis, liat di halaman Ubuntu community wiki untuk [perintah mount](https://help.ubuntu.com/community/Mount).

Ketika anda mengcopy files dari perangkat penyimpanan removable, perangkat tersebut tidak selalu tertulis di perangkat secara langsung. Sebaliknya perangkat tersebut akan disimpan dalam antrian sehingga mereka semua dapat ditransfer ke perangkat pada saat yang sama (untuk alasan efisiensi).

## Laptop

### Pengaturan manajemen daya

Anda mungkin ingin mengubah pengaturan manajemen daya laptop Anda untuk membantu menghemat baterai.

-  ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
   `→ Settings Manager → Power Manager`
-    Mengubah pengaturan yang sesuai
-    Perubahan yang diterapkan dapat langsung dilihat

### Touchpads

Sebagian besar laptop terdapat touchpad, yang digunakan untuk mengontrol pointer mouse. Ada banyak cara untuk mengubah cara touchpad berkerja; pengaturan touchpad dasar dapat dikonfigurasi dengan cara berikut:

- ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
    `→ Settings Manager → Mouse dan Touchpad`
-    Pada tab  `Device` : pilih `touchpad`
-    Anda dapat mengubah pengaturan touchpad sesuai dengan keinginan Anda.

## Suspend dan Hibernate

Untuk menghemat daya, Anda dapat mengalihkan komputer ke salah satu dari sejumlah mode hemat daya ketika Anda tidak menggunakannya:

`Suspend` adalah perintah untuk membuat komputer anda seperti tertidur. Komputer masih akan diaktifkan dan semua pekerjaan akan dibiarkan terbuka, dengan menggunakan daya yang lebih sedikit. Anda dapat membangunkan komputer dengan menekan tombol atau mengklik mouse.

`Hibernate` adalah mematikan komputer sepenuhnya sambil menyimpan keadaan saat komputer (seperti menjaga semua dokumen yang terbuka). Ketika Anda menghidupkan kembali komputer setelah Hibernate, semua pekerjaan Anda harus dikembalikan seperti sebelum Hibernate. Tidak ada daya yang digunakan saat komputer hibernate.

`Shutting Down` adalah mematikan komputer sepenuhnya tanpa menyimpan keadaan saat komputer masih hidup. Tidak ada daya yang digunakan saat komputer dimatikan.

`Resumming` membawa komputer keluar dari mode hemat daya dan kembali ke operasi normal.

Anda dapat secara manual mengalihkan komputer ke mode hemat daya dengan menekan `Menu → logout` dan kemudian pilih tombol mode yang sesuai.

### Komputer saya tidak Suspend atau hibernasi dengan benar

Beberapa komputer tidak dapat Suspend atau hibernate denga benar di TeaLinuxOS. Anda mungkin melihat beberapa gejala seperti berikut:

-    Komputer tidak mati setelah Anda klik untuk hibernate itu.
-    Ketika Anda menghidupkan komputer setelah hibernate itu, program yang sebelumnya terbuka Anda tidak hidup.
-    Komputer tidak bangun setelah proses suspend.
-    Program tertentu atau perangkat keras berhenti bekerja dengan benar setelah melanjutkan dari hibernate atau suspend.

Jika Anda mengalami masalah ini, Anda harus [melaporkan bug](http://tealinuxos.org/dukungan/bug.tealinuxos.org). Masalah mudah-mudahan akan diperbaiki dalam versi berikutnya dari TeaLinuxOS. Jika hardware Anda tidak bekerja dengan benar setelah suspend atau hibernate komputer, restart komputer Anda. Jika program tidak bekerja dengan benar, cobalah menutup program dan kemudian mulai lagi.

## Mouse dan keyboard

Ketika Anda menginstal TeaLinuxOS Anda diberi pilihan untuk memilih jenis keyboard dan bahasa. Selama instalasi, perangkat penunjuk harus secara otomatis terdeteksi dan dikonfigurasi. Jika Anda ingin atau perlu mengubah pengaturan dari setiap perangkat ini setelah instalasi, Anda dapat melakukannya dengan klik ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
   `→ Settings Manager → Mouse dan Touchpad` atau ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Settings Manager → Keyboard.`

Pilihan untuk mouse dan touchpad meliputi:

-    Orientasi tombol
-    Kecepatan pointer dan sensitivitas
-    Sensitivitas double-click
-    Tema Kursor



Beberapa pilihan untuk mengkonfigurasi keyboard Anda meliputi:

-    State of the Num Lock key on startup
-    Key repeat speed and delay
-    Cursor blinking speed
-    Application keyboard shortcuts
-    Keyboard layout and language










