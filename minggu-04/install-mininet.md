## Install Mininet

Untuk menginstall mininet ini saya menggunakan virtualisasi container menggunakan docker

#### 1. Download Docker Hub

<div align="left">
<img src="./img/Screenshot_1.jpg" width="600px">
</div>

Untuk menggunakan docker ini pastikan memiliki akun dan download docker hub di situs resminya di hub.docker.com

#### 2. Install

<div align="left">
<img src="./img/Screenshot_2.jpg" width="600px">
</div>

Kemudian buka installer tersebut dan jalankan sampai proses install selesai.

<div align="left">
<img src="./img/Screenshot_3.jpg" width="600px">
</div>

Setelah selesai jangan lupa untuk merestart.

#### 3. Jalankan Docker

Setelah selesai langsung saja jalankan docker.

<div align="left">
<img src="./img/Screenshot_4.jpg" width="600px">
</div>

Nah, disini saya sudah memilki container untuk operating system ubuntu jadi saya tinggal masuk ke tab remote repositories dan saya pull container ubuntu supaya dapat dijalankan dilocal.

<div align="left">
<img src="./img/Screenshot_5.jpg" width="600px">
</div>

Tunggu proses pull sampai selesai & tinggal jalankan dengan klik Run.

<div align="left">
<img src="./img/Screenshot_6.jpg" width="600px">
</div>

#### 4. Install Wireshark

Setelah berhasil masuk ke terminal ubuntu langsung saja install wireshark untuk keperluan mininet.

<div align="left">
<img src="./img/mininet/Screenshot_1.jpg" width="600px">
</div>

#### 5. Clone Mininet atau Install Mininet

Selanjutna install mininet melalui repo yang disediakan ubuntu atau bisa juga dengan clone project yang ada di github.

<div align="left">
<img src="./img/mininet/Screenshot_2.jpg" width="600px">
</div>

Nah, seperti ini tampilan jika kita melakukan clone project mininet dari github.

<div align="left">
<img src="./img/mininet/Screenshot_4.jpg" width="600px">
</div>

#### 6. Jalankan Wireshark & Mininet

Setelah semua library yang dibutuhkan sudah terinstall langsung saja kita coba untuk menjalankan wireshark dan mininet.

Untuk menjalankan wrapper wireshark tinggal jalankan perintah sudo wireshark &

<div align="left">
<img src="./img/mininet/Screenshot_3.jpg" width="600px">
</div>

Kemudian jalankan mininet dengan perintah sudo mn

<div align="left">
<img src="./img/mininet/Screenshot_5.jpg" width="600px">
</div>

Nah selanjutnya tinggal konfigurasi menyesuaikan kebutuhan yang ada.

