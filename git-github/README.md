# GIT & GITHUB FAST TRACK

Author: **Muhammad Rizqi Ariadi**

Linkedin: [Muhammad Rizqi Ariadi](https://www.linkedin.com/in/muhammad-rizqi-ariadi-bba168110/)

Facebook: [M Rizqi Ariadi](https://www.facebook.com/Muhammad.Rizqi.Ariadi)

Twitter : [M Rizqi Ariadi](https://twitter.com/MRizqiAriadi)

## Tujuan

Pada DevNotes kali ini, Anda akan mempelajari bagaimana cara membuat Repository pada GITHUB dan bagaimana menggunakan git dalam development aplikasi. Hasil dari DevNotes kali ini akan seperti ini:

## Tools yang dibutuhkan

* [GitHub Dekstop](https://desktop.github.com/) - GitHub Dekstop for Windows/Mac

* [Git](http://git-scm.com) - Git for All Platforms

Git distributions for Linux and POSIX systems are available on
the official Git SCM web site.

## Teori Version Control

Apa itu version control dan mengapa sebaiknya Anda peduli? Version control adalah sebuah sistem yang merekam perubahan-perubahan dari sebuah berkas atau sekumpulan berkas dari waktu ke waktu sehingga Anda dapat menilik kembali versi khusus suatu saat nanti. 

Jika Anda adalah seorang perancang grafis atau web dan ingin menyimpan setiap versi dari sebuah gambar atau layout (yang tentunya Anda ingin melakukannya), sebuah Version Control System (VCS) adalah hal yang bijak untuk digunakan. VCS memperbolehkan Anda untuk mengembalikan berkas-berkas ke keadaan sebelumnya, mengembalikan seluruh proyek kembali ke keadaan sebelumnya, membandingkan perubahan-perubahan di setiap waktu, melihat siapa yang terakhir mengubah sesuatu yang mungkin menimbulkan masalah, siapa dan kapan yang mengenalkan sebuah isu dan banyak lagi. Menggunakan VCS secara umum juga berarti bahwa jika Anda melakukan kesalahan atau menghilangkan berkas, Anda dapat dengan mudah memulihkannya.

### Sistem Version Control Tersebar
Di sinilah Distributed Version Control System (DVCS) masuk. Pada DVCS (seperti Git, Mercurial, Bazaar atau Darcs), para klien tidak hanya melakukan check out pada snapshot terakhir dari berkas: mereka mencerminkan sepenuhnya repository tersebut. Dan juga, jika ada salah satu server yang mati, dan sistem-sistem ini bekerja bersama melalui server itu, setiap repository milik klien dapat disalin kembali ke server untuk memulihkannya. Setiap check out benar-benar cadangan penuh dari semua data.

<img src="https://git-scm.com/book/en/v2/images/distributed.png" width="500" title="Centralized">

+ [Referensi](https://git-scm.com/book/id/v2/Memulai-Tentang-Version-Control) - Baca Tentang Version Control Selengkapnya.

## Sejarah GIT

Pada 2005, hubungan antara komunitas yang mengembangkan kernel Linux dan perusahaan komersil yang mengembangkan BitKeeper terputus, dan status bebas biaya dari alatnya dicabut. Hal ini mendesak komunitas pengembangan Linux (khususnya Linus Torvalds, pencipta Linux) untuk mengembangkan alat mereka sendiri berdasarkan beberapa pelajaran yang telah mereka pelajari ketika menggunakan BitKeeper. Beberapa sasaran dari sistem baru tersebut adalah sebagai berikut:

+ Kecepatan
+ Rancangan yang sederhana
+ Dukungan yang kuat untuk pengembangan non-linier (ribuan cabang paralel)
+ Benar-benar tersebar
+ Mampu menangani proyek besar seperti Linux secara efisien (kecepatan dan ukuran data)

Sejak kelahirannya pada 2005, Git telah berevolusi dan berkembang untuk dapat digunakan dengan mudah namun tetap memiliki kualitas awal tersebut. Git sangat cepat, sangat efisien dengan proyek-proyek besar, dan Git memiliki sistem percabangan yang hebat untuk pengembangan non-linear.
+ [Referensi](https://git-scm.com/book/id/v2/Memulai-Sejarah-Singkat-Git) - Baca Sejarah GIT Selengkapnya

## Join GITHUB
+ Membuka halaman [Join Github](https://github.com/join) → melakukan pendaftaran akun github → melakukan konfirmasi pada email anda.

  <img src="images/register_github.JPG" width="500" title="Join Github">

## DevNotes Buat Repositori dari GITHUB

1. Klik tombol → Tambah (__+__) → Memilih menu __new repository__.

    <img src="images/menu_create_github.JPG" width="350" title="Button +">

2. Buat *repository* baru di Github dengan kriteria sebagai berikut:

    | Perintah | Deskripsi |
    | --- | --- |
    | __Repository name__ | First-Repository |
    | __Description__ | Learning by doing |
    | __Public/Private__ | Public |
    | __Initialize this repository with a README__ | Check |

3. Klik tombol → *Create Repository* , maka akan membuat *repository* seperti ini:

    <img src="images/first_repository.JPG" width="800" title="First Repository">
    
   - [x] Selamat anda telah berhasil membuat _repository_ baru :+1:

## DevNotes _Clone Repository_ dari GITHUB

Pada materi sebelumnya anda sudah belajar membuat repositori baru. Kita dapat mengambil repositori tersebut dengan melakukan _clone_ dari github ke lokal komputer anda dengan cara sebagai berikut:

1. Klik tombol → __Clone or download__ → memilih tombol copy URL / blok link URL (Copy).

    <img src="images/clone_repository.JPG" width="300" title="Button Clone">
    
    <img src="images/copy_link_repository.JPG" width="300" title="Button Copy Link URL">
    
2. Buka Command Prompt(CMD) anda, sebelum kita melakukan *clone repository* pastikan anda melihat *folder/directory* __Documents__ dengan menggunakan perintah __dir__ untuk menampilkan isi dari *folder* C:\Users\~username_anda.

`Apabila anda sudah memahami perintah Command Prompt (CMD) silahkan letakkan pada folder/directory yang anda diinginkan.`

    ```
    Microsoft Windows [Version 6.3.9600]
    (c) 2013 Microsoft Corporation. All rights reserved.

    C:\Users\mhmmdrizqi>dir
     Volume in drive C has no label.
     Volume Serial Number is F6DF-BA88

     Directory of C:\Users\mhmmdrizqi

    01/12/2020  08:55 AM    <DIR>          .
    01/12/2020  08:55 AM    <DIR>          ..
    01/12/2020  08:55 AM               215 .gitconfig
    10/08/2019  07:03 PM    <DIR>          .LdVirtualBox
    07/13/2019  08:51 AM               186 .packettracer
    03/17/2019  11:41 PM    <DIR>          .ssh
    01/12/2020  07:37 AM               854 .viminfo
    02/17/2019  06:16 PM    <DIR>          .vscode
    07/13/2019  04:56 AM    <DIR>          Cisco Packet Tracer 7.2.1
    03/17/2019  04:03 PM    <DIR>          Contacts
    01/06/2020  10:18 PM    <DIR>          Desktop
    01/12/2020  08:01 AM    <DIR>          Documents
    01/12/2020  07:04 AM    <DIR>          Downloads
    03/17/2019  04:03 PM    <DIR>          Favorites
    03/17/2019  04:03 PM    <DIR>          Links
    04/06/2019  11:28 AM    <DIR>          Music
    01/12/2020  09:52 AM    <DIR>          Pictures
    03/17/2019  04:03 PM    <DIR>          Saved Games
    04/17/2019  09:36 AM    <DIR>          Searches
    03/17/2019  04:03 PM    <DIR>          Videos
                   3 File(s)          1,255 bytes
                  17 Dir(s)  29,433,196,544 bytes free
    ```

3. Menggunakan perintah __CD__ untuk dapat masuk ke *folder/directory* __Documents__.

    ```
    C:\Users\mhmmdrizqi>cd Documents
    C:\Users\mhmmdrizqi\Documents>
    ```

4. Selanjutnya, lakukan _clone_ dengan perintah __git clone YOUR-URL-REPOSITORY__ sebagai berikut:

    ```diff
    C:\Users\mhmmdrizqi\Documents>git clone https://github.com/<username>/First-Repository.git
    ```
5. Tunggu sampai proses download _repository_ selesai seperti ini:

     <img src="images/clone_cmd_github.JPG" width="500" title="Clone CMD">
     
6. Selamat anda sudah berhasil melakukan clone dari GITHUB ke lokal komputer.

     <img src="images/folder_first_repository.JPG" width="500" title="Result Clone">
     
     `Penting: ini merupakan salah satu cara untuk melakukan clone repositori anda, ada beberapa cara yang anda dapat gunakan untuk melakukan clone.`
     
   - [x] Selamat anda telah berhasil melakukan _clone repository_ :+1:
   
## DevNotes Menambahkan _file_ ke _Repository_ GITHUB

Sekarang kita dapat menambahkan/mengubah/menghapus ___file___ ataupun ___folder___ dari lokal repositori. Jangan khawatir semua jenis file dapat anda tambahkan ke repositori di GITHUB. Tentukan beberapa _file_ yang anda ingin tambahkan ke _repository_ anda atau bisa menggunakan contoh _file_ yang kita buat bersama !

### Perintah & Alur Direktori GIT

Ada banyak perintah yang dapat anda lakukan, tetapi kita akan belajar beberapa perintah yang sering digunakan saja. Kemudian alur direktori git hanya sebagai tambahan pemahaman saja, untuk mengetahui letak pada saat anda melakukan beberapa perintah tersebut.

#### Perintah
Untuk melakukan singkronisasi perubahan ada beberapa perintah yang dapat anda gunakan sebagai berikut:
+ __git fetch__
Unduh semua riwayat dari _remote tracking branchs_ 

+ __git Merge__
Menggabungkan _remote tracking branchs_  ke _branch_ lokal saat ini

+ __git push__
Unggah semua _commit branch_ lokal ke GitHub

+ __git pull__
Memperbarui _branch_ tempat kerja lokal Anda saat ini dengan yang baru. Melakukan dari _remote tracking branchs_ yang sesuai di GitHub. (__git pull__ adalah kombinasi dari git fetch dan git merge)

Untuk melakukan perubahan ada beberapa perintah yang dapat anda gunakan sebagai berikut:
+ __git show [commit]__
Metadata keluaran dan perubahan konten dari _commit_ yang ditentukan.

+ __git add [file]__
Snapshots file dalam persiapan untuk versi.

+ __git commit -m "[pesan deskriptif]"__
Merekam snapshot file secara permanen dalam riwayat versi.

#### Alur Direktori GIT

* Alur kerja dasar Git adalah seperti berikut:
    1. Anda mengubah berkas dalam _working directory_ Anda.
    2. Anda menyiapkan berkasnya, menambah snapshot darinya ke _staging area_ Anda.
    3. Anda melakukan _commit_, yang mengambil berkas-berkas yang ada pada _staging area_ dan menyimpan _snapshot_ tersebut secara tetap ke dalam direktori Git Anda.
    <img src="https://git-scm.com/book/en/v2/images/areas.png" width="500" title="areas">
    
    
## Daftar Kata-kata
* __Git__           : Sistem Kontrol Versi Terdistribusi yang _open source_.
* __GitHub__        : _Platform_ untuk hosting dan berkolaborasi pada repositori GIT.
* __Commit__        : Objek GIT, Snapshot dari seluruh repositori anda yang dikompres menjadi SHA.
* __Branch__        : Pointer yang dapat bergerak menuju ke _Commit_.
* __Clone__         : Versi lokal dari repositori, termasuk semua _Commit_ dan _Branch_.
* __Fork__          : Salinan repositori di GitHub yang dimiliki oleh pengguna lain.
* __Pull Request__  : Tempat untuk membandingkan dan mendiskusikan perbedaan pada sebuah _branch_ dengan ulasan, komentar, terintegrasi tes dan lainnya.
