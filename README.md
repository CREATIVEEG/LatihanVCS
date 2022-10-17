# Latihan1 : Tutorial Penggunaan GIT
Baik, disini saya akan menjelaskan tutorial mengenai, cara penggunaan GIT. Yang kita butuhkan adalah software git, dan tentunya akun github. Langsung saja saya mulai untuk tutorial penggunaan GIT.

## Menginstall software GIT
• Pertama kalian harus mendownload software GIT terlebih dahulu, kalian bisa mendownloadnya di **git-scm.com**
![images.png](https://user-images.githubusercontent.com/115677376/196108566-074d323f-72f3-4759-ae6a-c3df9ba9e101.png)
*Pilih sesuai dengan sistem yang kalian gunakan, jika memakai windows pilih juga sesuai dengan bit kalian (32bit atau 64bit) agar dapat berjalan.*<br /><br />
• Jika sudah terdownload, langsung saja klik install untuk melakukan penginstalan software GIT. ketika penginstalan terus klik next saja sampai ke step install. Tunggu proses install sampai selesai.<br />
![images.png](https://user-images.githubusercontent.com/115677376/196108583-0ec83f0e-058a-41ae-9fe0-767074cae182.png)<br /><br />

## Membuat Repository Local
• Setelah penginstalan selesai, kalian tinggal membuka cmd atau membuka software git langsung. Untuk test awal, apakah git sudah terinstall dengan benar, kita akan memasukan cmd untuk mengecek versi git. Caranya tinggal ketikan saja **git --version** . Disini saya memakai versi 2.38.0.windows.1.<br />
![images.png](https://user-images.githubusercontent.com/115677376/196109813-b6560a1b-4527-452d-9b79-2fb990e373c6.png)<br /><br />
• Setelah mengecek versi, sekarang saya akan membuat direktori untuk latihan ini. Dengan cara mengetikan cmd, **mkdir "Lab_Pemrograman"**, setelah berhasil langsung saja pindah direktori ke direktori yang sudah dibuat ini, dengan cara mengetik cmd, **cd Lab_Pemrograman** <br />
![images.png](https://user-images.githubusercontent.com/115677376/196112707-6f11e4d4-492d-44cc-a249-39bad0ac42be.png)<br /><br />
• Lalu, jika sudah masuk kedirektori yang dibuat, langsung saja buat lagi sub-direktori untuk latihan pertama sebagai contoh saya akan buat direktori Latihan1. Sama seperti cmd sebelumnya yaitu **mkdir "Latihan1"**, dan pindah direktori lagi dengan **cd Latihan1**<br />
![images.png](https://user-images.githubusercontent.com/115677376/196113812-f0ac8fb6-c4ed-4cfe-b476-11a83bc5cf67.png)<br /><br />
• Lalu masukan cmd untuk membuat repository local yaitu, **git init**<br />
![images.png](https://user-images.githubusercontent.com/115677376/196116397-f8fa4b77-2ca5-429d-a1f5-c6f48762b3ab.png)<br /><br />
• Jika sudah, pertama-tama kita harus meregister username dan email kita. Dengan contoh seperti ini.<br />
**git config --global user.name “nama_user”**<br />**git config --global user.email “user_email”**<br />
![images.png](https://user-images.githubusercontent.com/115677376/196117123-41bc4cc6-1942-4590-83f2-48d6dba8b608.png)<br /><br />
• Ketika sudah berhasil ter-register, kita akan membuat sebuah file yaitu **README.md**. Dengan mengetik cmd<br />
**echo "# Latihan1" >> README.md**<br />
![images.png](https://user-images.githubusercontent.com/115677376/196118496-e3dc4d0f-2e21-4c78-a0e5-3edf36e32d04.png)<br /><br />
• Untuk menambahkan file yang baru saja dibuat tersebut, gunakan cmd seperti ini<br />
**git add README.md**<br />
dan untuk menyimpan perubahan file gunakan cmd seperti ini<br />
**git commit -m “Latihan penggunaan GIT”**<br />
![images.png](https://user-images.githubusercontent.com/115677376/196119783-7e42ad3f-e7ef-456d-a98e-3a175e1689b6.png)<br /><br />

## Membuat Repository Server
• Setelah berhasil membuat Repository local, kita akan membuat servernya. Yaitu dengan cara membuat akun github, pada website **http://github.com**<br />
Masukan email, password baru, dan username. Lalu ikuti petunjuk yang diarahkan pada websitenya.<br />
![images.png](https://user-images.githubusercontent.com/115677376/196124948-985b02c0-3723-44bc-8a59-6c5ce0cbe7fa.png)<br /><br />
• Jika sudah berhasil maka tampilan akan seperti ini<br />
![images.png](https://user-images.githubusercontent.com/115677376/196126555-3338753c-b5e7-4bba-990f-af6830b45cfa.png)<br /><br />
• Dihalaman ini, klik icon tambah ( + ) diposisi kanan atas. Tujuannya adalah untuk membuat server repository yang baru<br />
![images.png](https://user-images.githubusercontent.com/115677376/196127730-e37c2f9c-ef85-4cb0-87a0-f9430196fb41.png)<br /><br />
• Setelah klik New Repository, akan muncul halaman seperti ini, isi bagian Repository Name nya. Saya mengisi dengan Latihan1 atau ikuti saja seperti pada gambar dibawah, lalu klik create repository<br />
![images.png](https://user-images.githubusercontent.com/115677376/196129011-af6728ee-032d-4bd0-90dc-de07cd856795.png)<br /><br />
• Jika sudah membuat reporistory baru, maka halaman akan dialihkan seperti ini, dan Repository Server berhasil dibuat<br />
![images.png](https://user-images.githubusercontent.com/115677376/196130082-df3e7913-a789-4ed2-a0b7-8f3fa56e1d38.png)<br /><br />

## Menambahkan Perubahan ke Repository Server
Remote Repository ini digunakan untuk menyimpan atau memasukan perubahan file yang dilakukan di Repository Local tadi yang sudah kita buat. Sehingga dapat diakses oleh semua pengguna github.<br />

• Untuk menambahkan remote repository, kita hanya perlu mengetik cmd yaitu<br />
**git remote add origin [URL]**<br />
Masukan URL github yang telah kita buat pada server repository tadi
![images.png](https://user-images.githubusercontent.com/115677376/196132324-12bd4da9-d07d-431e-803e-d1a00110449e.png)<br /><br />
• Untuk mengirim perubahan yang telah kita buat di Repository Local, masukan cmd yaitu<br />
**git push -u add origin master**<br />
![images.png](https://user-images.githubusercontent.com/115677376/196143195-fd7ef5e6-67a2-4d86-88b8-577b2312044a.png)<br /><br />
• Setelah itu, akan muncul sebuah pop up, untuk melanjutkan memasukan respository local kita ke server<br />
![images.png](https://user-images.githubusercontent.com/115677376/196143235-7ec79bc5-5826-4505-b56c-cbd58cf654a8.png)<br /><br />
• Masukkan Username dan password yang telah dibuat tadi, dan berikan akses ke respository server kita<br />
![images.png](https://user-images.githubusercontent.com/115677376/196143239-c13f4819-b8ee-483f-9040-4f1e43e56236.png)<br />
![images.png](https://user-images.githubusercontent.com/115677376/196143243-aaedcce5-ffab-4ff3-8bd8-f0f5c00b0ccb.png)<br /><br />
• Jika sudah refresh browser kalian, dan akhirnya... Kita sudah berhasil memasukan repository local kita kedalam server. Selanjutkan kalian bisa mengedit isi dari README.md, dengan menekan icon pensil
![images.png](https://user-images.githubusercontent.com/115677376/196143245-c12f6b58-414e-4a10-895e-266bfc4d3147.png)<br /><br />
Selesai... Baiklah, sekian tugas membuat tutorial dari saya. Jika ada kesalahan kata atau kekurangan dalam konten saya meminta maaf yang sebesar-besarnya.<br /> Terimakasih...<br />
**Nama  :** Rhendy Diki Nugraha<br />
**Kelas :** TI.22.A1<br />
**Dosen :** Agung Nugroho, S.Kom, M.Kom<br />
