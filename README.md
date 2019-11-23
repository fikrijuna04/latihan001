# latihan001
# Cara penggunaan git
# Apa Itu Git ?
Git adalah salah satu sistem pengontrol versi(Version Control System) pada proyek perangkat lunak yang diciptakan Linus Torvalds.
Pengontrol versi bertugas memcatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.
Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.
# Instalasi Git
Download Git, Buka website resminya git-scm.com.
Kemudian unduh Git sesuai dengan arsitektur komputer kita, Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit
![1](https://user-images.githubusercontent.com/57304587/69478215-a0f04800-0e22-11ea-994b-1384efebcd2d.png)

Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka CMD atau PowerShell, kemudian ketik perintah git --version
![2](https://user-images.githubusercontent.com/57304587/69478288-515e4c00-0e23-11ea-98f7-432aea224f15.png)
Menambahkan Global Config
Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.

apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

Config Global Repository

![3](https://user-images.githubusercontent.com/57304587/69478306-7226a180-0e23-11ea-81c6-c89918c45879.png)
Perintah Dasar Git
git init , perintah untuk membuat repository local.
git add , perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
git commit , perintah untuk menyimpan perubahan kedalam database git.
git push -u origin master , perintah untuk mengirim perubahan pada repository local menuju server repository.
git clone [url], perintah untuk membuat working directory yang diambil dari repositry sever.
git remote add origin [url] , perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)
git pull , perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke local repository.
Membuat Reposiory Local
Buka direktory aktif, misal: d:\labs_pemrograman1 (bukamenggunakan Windows Explorer)

klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,sehingga muncul git bash commad

Buat direktory project praktikum pertama dengan nama latihan1
![4](https://user-images.githubusercontent.com/57304587/69478328-c9c50d00-0e23-11ea-86c6-1009c1f8137c.png)
Sehingga terbentuk satu direktori baru dibawahnya, selanjutnyamasuk kedalam direktori tersebut dengan perintah cd (changedirectory)

direktory aktif menjadi: d:\labs_pemrograman1\latihan1

Membuat Reposiory Local
Jalankan perintah git init, untuk membuat repository local.

Repository baru berhasil di inisialisasi, dengan terbentuknya satudirektori hidden dengan nama .git

Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

![5](https://user-images.githubusercontent.com/57304587/69478367-0f81d580-0e24-11ea-8051-8ad2b9ab1c4e.png)
Menambahkan File baru pada repository
Untuk membuat file dapat menggunakan text editor, lalu menyimpafilenya pada direktori aktif (repository)

disini kita akan coba buat satu file bernama README.md (text file) $ echo “#Latihan 1” >> README.md

![6](https://user-images.githubusercontent.com/57304587/69478377-2e806780-0e24-11ea-9960-b6a44de1bfca.png)
File README.md berhasil dibuat.

Menambahkan File baru pada repository
Untuk menambahkan file yang baru saja dibuat tersebut gunakanperintah git add.

File README.md berhasil ditambahkan. $ git add README.md
![7](https://user-images.githubusercontent.com/57304587/69478384-566fcb00-0e24-11ea-8047-d2ca05bfea75.png)
Commit (Menyimpan perubahan ke database)
Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah $ git commit -m “komentar commit”
![8](https://user-images.githubusercontent.com/57304587/69478396-7d2e0180-0e24-11ea-8149-f39e85761675.png)
Perubahan berhasil disimpan

Membuat repository server
Server reopsitory yang akan kita gunakan adalah github.com

Anda harus membuat akun terlebih dahulu.

Pada laman github, klik tombol start a project, atau Dari menu (icon +) klik New Repository

![9](https://user-images.githubusercontent.com/57304587/69478419-a2227480-0e24-11ea-9834-c18d79d36076.png)
Membuat repository server
Isi nama repositorynya, misal: labpy1.

lalu klik tombol Create repository

![10](https://user-images.githubusercontent.com/57304587/69478452-ffb6c100-0e24-11ea-80fc-a980a2d977dd.png)
Menambahkan Remote Repository
Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

![11](https://user-images.githubusercontent.com/57304587/69478464-207f1680-0e25-11ea-872d-2d7e4b6c0039.png)

Melihat hasilnya pada server repository
Buka laman github.com,arahkan pada repositori- nya.

Maka perubahan akan terlihat pada laman tersebut.
![12](https://user-images.githubusercontent.com/57304587/69478469-3ee51200-0e25-11ea-8e8f-fe8237421553.png)


