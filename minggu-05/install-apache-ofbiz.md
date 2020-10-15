## Install Apache OFBiz

Untuk menginstall apache ofbiz kita memerlukan beberapa library yang harus diinstall

#### 1. Install OpenJDL Binaries

<div align="left">
<img src="./img/awal.jpg" width="600px">
</div>

Untuk mendownload file tersebut langsung saja kunjungi situs resminya dan lakukan install setelah file sudah terdownload.

#### 2. Install Apache OFBiz

Kemudian untuk menginstall apache ofbiz kita perlu mendownload file installer disitus resimnya.

<div align="left">
<img src="./img/Screenshot_1.jpg" width="600px">
</div>

Kemudian pilih menu Download and Install

<div align="left">
<img src="./img/Screenshot_2.jpg" width="600px">
</div>

Bentuk filenya adalah sebuah zip, jadi kita perlu mengekstract dan menjalankan installer tersebut.

<div align="left">
<img src="./img/Screenshot_3.jpg" width="600px">
</div>

Kemudian ikuti panduan yang ada pada file INSTALL

<div align="left">
<img src="./img/Screenshot_4.jpg" width="600px">
</div>


##### A. Install Gradle

Langkah pertama pastikan kita sudah memiliki software gradle. Jika belum bisa langsung download file installernya di situs resimnya gradle. Bentuk filenya pun juga zip jadi kita perlu mengekstrak.

<div align="left">
<img src="./img/Screenshot_5.jpg" width="600px">
</div>

Setelah sudah terektrak kita perlu menambahkan path command gradle di environment windows.

<div align="left">
<img src="./img/Screenshot_6.jpg" width="600px">
</div>

Setelah itu kita cek versi dari gradle yang kita pakai dengan menjalankan perintah gradle -v

<div align="left">
<img src="./img/Screenshot_7.jpg" width="600px">
</div>

#### 4. Eksekusi Installer

Setelah semua persiapan sudah selesai maka tinggal kita jalankan installer gradle. Pastikan kita sudah berada difolder dimana hasil ekstrak aplikasi apache ofbiz.

<div align="left">
<img src="./img/cmd-1.jpg" width="600px">
</div>

Jalankan perintah gradle wrapper untuk memjalankan aplikasi apache ofbiz.

<div align="left">
<img src="./img/cmd-2.jpg" width="600px">
</div>

Tunggu proses gradle wrapper sampai selesai.

<div align="left">
<img src="./img/cmd-3.jpg" width="600px">
</div>

Kemudian jalankan perintah gradle/gradlew cleanAll loadAll

<div align="left">
<img src="./img/Screenshot_9-salah.jpg" width="600px">
</div>

Tunggu proses sampai selesai

<div align="left">
<img src="./img/Screenshot_10.jpg" width="600px">
</div>

Setelah proses build selesai langsung saja jalankan perintah gradle/gradlew ofbiz

<div align="left">
<img src="./img/Screenshot_11.jpg" width="600px">
</div>

Maka ketika menjalankan aplikasi tersebut memerlukn allow access ke administrator.

<div align="left">
<img src="./img/Screenshot_12.jpg" width="600px">
</div>

Proses gradle apache ofbiz memakan banyak waktu, tapi tidak perlu menunggu sampai selesai.

Langsung saja akses halaman dashboard aplikasi tersebut dengan url http://localhost:8443/webtools

<div align="left">
<img src="./img/cmd-4.jpg" width="600px">
</div>

Berikut ini tampilan awal dari aplikasi apache ofbiz.

<div align="left">
<img src="./img/cmd-5.jpg" width="600px">
</div>

Setelah itu terdapat halaman login untuk aplikasi apache ofbiz. Gunakan saja default untuk login username: admin, password: ofbiz.

<div align="left">
<img src="./img/cmd-6.jpg" width="600px">
</div>

Nah, seperti ini tampilan awal apache ofbiz.

<div align="left">
<img src="./img/cmd-7.jpg" width="600px">
</div>


