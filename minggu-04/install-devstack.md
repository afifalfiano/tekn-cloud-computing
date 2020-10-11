## Install Devstack

Untuk menginstall devstack ini saya menggunakan virtualisasi container menggunakan docker

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

#### 4. Tambahkan User Stack

Setelah berhasil menjalankan ubuntu langsung saja buat user baru untuk stack

<div align="left">
<img src="./img/devstack/Screenshot_1.jpg" width="600px">
</div>

Kemudian jalankan perintah sudo su - stack untuk berpindah akses ke user stack.

<div align="left">
<img src="./img/devstack/Screenshot_2.jpg" width="600px">
</div>

Jika masih error maka bisa kita cek pada file /etc/sudoers yang mana bisa kita tambahkan secara manual ada User privilege specification

<div align="left">
<img src="./img/devstack/Screenshot_3.jpg" width="600px">
</div>

#### 5. Install Git

Selanjutnya install git dengan cara menjalankan sudo apt -y install git

<div align="left">
<img src="./img/devstack/Screenshot_4.jpg" width="600px">
</div>

Setelah itu clone project yang sudah ada digithub.

<div align="left">
<img src="./img/devstack/Screenshot_5.jpg" width="600px">
</div>

#### 6. Konfigurasi Devstack

Kemudian tambahkan file localhost.conf dan isi konfigurasinya seperti dibawah ini.

<div align="left">
<img src="./img/devstack/Screenshot_6.jpg" width="600px">
</div>

Kemudian untuk menjalankan project devstack tinggal masuk ke repository devstack dan jalankan perintah ./stack.sh

<div align="left">
<img src="./img/devstack/Screenshot_7.jpg" width="600px">
</div>

Tunggu sampai proses selesai

<div align="left">
<img src="./img/devstack/Screenshot_8.jpg" width="600px">
</div>

Tapi disini saya ada beberapa kendala seperti dibawah ini. Pada akhirnya jika berhasil nanti tinggal akses saja ip yang terdapat pada file localhost.conf


<div align="left">
<img src="./img/devstack/Screenshot_9.jpg" width="600px">
</div>

Sebelum melakukan install devstack saya juga menambahkan beberapa libary seperti python3, python3-dsutils, ip command dan iptables. Tapi masih saja terdapat kendala.