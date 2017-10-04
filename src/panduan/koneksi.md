---
title: Koneksi Jaringan dan Internet
type: panduan
order: 107
---

## Menyambung dan Memutuskan jaringan

 ![menu](https://cloud.githubusercontent.com/assets/26142091/23577576/a90a1a1c-00f5-11e7-86ec-d4bc4d831a13.png)
 `→ Settings → Network Connection`
atau klik icon ![networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager` yang berada di panel `→ Edit.`
Koneksi jaringan di TealinuxOS Pappermint menggunakan network connection untuk mengatur jaringan menggunakan kabel, jaringan wireless, mobile broadband, VPN dan koneksi DSL. Network connection akan menghubungkan komputer anda secara otomatis dengan jaringan, namun jika penyambungan pertama kali biasanya memerlukan informasi keamanan untuk terhubung ke jaringan.

Untuk memutuskan (disconnect) jaringan klik pada icon ![networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager` yang berada di panel lalu klik `disconnect.` 

## Konfigurasi koneksi
 
 Jika anda menginginkan untuk mengkonfigurasi jaringan anda, Pada kotak dialog Netwok Connection anda akan melihat koneksi-koneksi jaringan yang ada. Pilih salah satu untuk mengatur konfigurasi atau anda dapat menambahkan koneksi jaringan baru dengan memilih `Add.`

## Berbagi koneksi ke komputer lain

Anda dapat berbagi koneksi ke komputer lain dengan menggunakan kabel Ethernet. Untuk pengaturannya klik icon ![networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager → Edit` lalu pilih `Add` pada kotak dialog pilih jenis koneksi yang anda inginkan, Setelah mengklik tombol create pada bagian tab `IPv4 Setting` pilih metode yang digunakan.

## Troubleshooting pada jaringan

Jika koneksi jaringan anda tidak bekerja secara sempurna anda dapat menggunakan beberapa cara untuk menemukan kesalahan koneksi anda.

### Mengecek informasi koneksi

- Menggunakan icon NetworkManager
   ![networkmanager](https://cloud.githubusercontent.com/assets/26142091/23577859/8c296144-00fc-11e7-9884-b770de64ba36.png)
 `NetworkManager → Information`. Jika information di disable ini kemungkinan karena komputer anda tidak terkoneksi dengan  jaringan.
-    Menggunakan ifconfig
    buka terminal (short cut terminal guake : F12)
    ketikkan perintah ifconfig lalu enter.
    ifconfig ini akan menunjukkan informasi koneksi anda meliputi nama koneksi, IP address di inet addr , dan MAC address di Hwaddr.


### Mengecek koneksi bekerja

Untuk mengecek apakah koksi anda bekerja atau tidak anda dapat mengetesnya melalui ping.

-    Buka terminal
-    ketikkan perintah 
           
           ping tealinuxos.org

-   lalu enter.

Jika koneksi berhasil anda akan menerima pesan berupa jumlah statistik paket yang di transmisikan. Jika anda mendapat pasan `ping: unknown host tealinuxos.org` maka komputer anda mungkin tidak terhubung ke internet dan tidak dapat menjangkau Domain Name System (DNS) server.

