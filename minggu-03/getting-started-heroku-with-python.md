## Getting Started Heroku with Python

Berikut ini tutorial singkat menggunakan heroku dengan mendeploy project dari python.

#### 1. Login

Login akun heroku terlebih dahulu melalui cli baik dari windows ataupun linux/mac.

<div align="left">
<img src="./img/20.herokulogin.jpg" width="600px">
</div>

#### 2. Clone Project

Kemudian setelah berhasil login clone project python yang ada di github.

<div align="left">
<img src="./img/21.cloneproject.jpg" width="600px">
</div>

#### 3. Create Project

Kemudian kita buat project baru di heroku melalui cli

<div align="left">
<img src="./img/22.create-heroku.jpg" width="600px">
</div>

#### 4. Push Project

Setelah berhasil membuat project melalui cli maka langkah selanjutnya adalah mengunggah project python hasil clone tadi ke heroku.

<div align="left">
<img src="./img/23.heroku-push.jpg" width="600px">
</div>

#### 5. Open Project

Setelah proses push berhasil maka jalankan perintah heroku open untuk mengecek project kita di heroku.

<div align="left">
<img src="./img/25.web-view.jpg" width="600px">
</div>

.

<div align="left">
<img src="./img/26.log-project.jpg" width="600px">
</div>


#### 6. Scalling Project

Kita juga bisa melakukan scalling up untuk project kita di heroku.

<div align="left">
<img src="./img/24.heroku-scale.jpg" width="600px">
</div>

Kemudian untuk megecek status penggunakan sumber daya di heroku bisa jalankan perintah heroku ps

<div align="left">
<img src="./img/27.heroku-scale.jpg" width="600px">
</div>

Kemudian kita coba buat scallingnya menjadi 1

<div align="left">
<img src="./img/27.heroku-scale2.jpg" width="600px">
</div>

Selanjutnya kita kembalikan kembali scalling heroku menjadi 0

<div align="left">
<img src="./img/27.heroku-scale1.jpg" width="600px">
</div>

#### 7. Install Dependensi

Supaya kita bisa menggunakan paket atau library yang digunakan di project ini di localhost maka kita harus menginstall terlebih dahulu. Pada file requirements.txt sudah terdapat list dependensi yang digunakan jadi tinggal jalankan perintah pip install -r requirements.txt

<div align="left">
<img src="./img/28.installdepend.jpg" width="600px">
</div>

Kemudian kita cek dependensi apa saja yang sudah terinstall dengan menggunakan perintah pip list

<div align="left">
<img src="./img/29.piplist.jpg" width="600px">
</div>

Kemudian kita coba copi konfigurasi ke file static python.

<div align="left">
<img src="./img/30.copied.jpg" width="600px">
</div>

#### 8. Jalankan Localhost

Sebelum mendeploy ke heroku sebaiknya kita cek terlebih dahulu di localhost. Untuk windows jalankan perintah heroku local web -f Procfile.windows. Apa itu Procfile? Procfile adalah file konfigurasi untuk menjalankan project python di suatu operatin system.

<div align="left">
<img src="./img/31.local.jpg" width="600px">
</div>

Nah, berikut ini tampilan di localhost.

<div align="left">
<img src="./img/32.done.jpg" width="600px">
</div>

#### 7. Konsume API

Kemudian kita coba mengkonsusmi api dengan library requests. Install terlebih dahulu dengan cara pip install requests

<div align="left">
<img src="./img/33.requestinstall.jpg" width="600px">
</div>

Kemudian edit file view.py yang berada di folder hello. Edit seperti berikut ini.

<div align="left">
<img src="./img/34.editview.jpg" width="600px">
</div>

Kemudian kita jalankan lagi dan seperti berikut ini tampilannya.

<div align="left">
<img src="./img/35.done.jpg" width="600px">
</div>

Pastikan pada requirements.txt juga ditambahkan library requests supaya ketika project sudah terdeploy tidak terjadi error karena tidak menginstall library tersebut lantaran tidak terdaftar pada requirements.txt

<div align="left">
<img src="./img/37.janganlupa.jpg" width="600px">
</div>

Jika sudah tidak ada error maka tinggal melakukan git add, git commit dan git push ke heroku.

<div align="left">
<img src="./img/36.pushheroku.jpg" width="600px">
</div>

Nah, seperti ini tampilan terbaru project python setelah berhasil di push ke heroku.

<div align="left">
<img src="./img/38.berhasil.jpg" width="600px">
</div>

#### 8. Log

Untuk addons paprtrail ini saya lompati karena untuk mendapatkan addons ini harus mneggunakan kartu kredit

<div align="left">
<img src="./img/39.failedpapertrail.jpg" width="600px">
</div>

#### 9. Show Project on Terminal

Selain melihat project kita di browser kita juga bisa melihat melalui terminal yang kita gunakan. Caranya adalah jalankan perintah berikut ini heroku run python manage.py shell

Setelah itu masukkan perintah import requests

Kemudian masukan kembali print(requests.get('http://httpbin.org/status/418'))

<div align="left">
<img src="./img/40.show via terminal.jpg" width="600px">
</div>

Jika sudah selesai dan ingin keluar dari terminal tinggal jalankan perintah exit()

#### 10. Heroku Bash

Kita juga bisa melakukan remote bash pada project kita yang ada di heroku. Dengan cara menjalankan perintah berikut ini heroku run bash

<div align="left">
<img src="./img/41.bashheroku.jpg" width="600px">
</div>

#### 11. Dependensi OS

Selanjutnya kita mencoba menggunakan dependensi os. Pastikan pada file view.py yang ada di folder hello diedit menjadi seperti berikut ini.

<div align="left">
<img src="./img/44.changeview.jpg" width="600px">
</div>

Kemudian jalankan kembali project tersebut di localhost dengan menjalankan perintah heroku local web -f Procfile.windows

<div align="left">
<img src="./img/44.doneagain.jpg" width="600px">
</div>

Kita juga bisa mengkonfigurasi TIMES project kita pada heroku dengan menjalankan perintah heroku config:set TIMES=2

Untuk melihat config terbaru tinggal jalankan perintah heroku config

<div align="left">
<img src="./img/45.editconfig.jpg" width="600px">
</div>

Untuk melihat addons, config dan penggunaa sumber daya dari project kita bisa jalanka perintah berikut ini heroku addons untuk melihat addons, heroku config untuk melihat configuration dan heroku pg untuk melihat seberapa besar peggunaan sumber daya dari project kita.

#### 12. Migrasi Database

Untuk melakukan migrasi databse tinggal jalankan perintah heroku run python manage.py migrate

<div align="left">
<img src="./img/47.migrate.jpg" width="600px">
</div>

Seharusnya tinggal kita jalankan perintah heroku pg:psql dan kita bisa menggunakan database posgresql secara localhost. Tapi karena masih ada kendala maka saya tidak bisa melakukan langkah tersebut

<div align="left">
<img src="./img/50.psql.jpg" width="600px">
</div>