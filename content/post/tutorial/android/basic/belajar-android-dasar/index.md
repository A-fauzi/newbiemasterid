---
title: "Belajar Android Dasar"
description: Pengenalan android dan cara menginstall android studio
date: 2023-01-07
image: android-basic.png
tutorials:
  - Android
tags:
  - tutorials
---

# Introduction

Halo sahabat **_NMI_**, ketemu lagi nih sama mimin hehe

Ini waktu yang ditunggu nih, kali ini mimin bakal ngajarin cara buat aplikasi android menggunakan **Kotlin**.

Gausah lama lama ya langsung aja gass 🚀

## Panduan Developer

Artikel ini ngabahas cara mem-build aplikasi Android menggunakan API di framework Android dan library lainnya.

Kalo Kalian baru mengenal Android dan mau langsung nulis kode, kalian bisa kunjungi ke bagian tutorial [Build Aplikasi Pertama Kamu]().

Kalian juga bisa lihat referensi lainnya yang udah di sediain sama Google untuk mempelajari pengembangan Android kunjungi berikut:

- [Codelab](): Tutorial singkat mandiri yang masing-masing membahas topik tersendiri. Sebagian besar codelab memandu Kalian dalam proses mem-build aplikasi kecil, atau menambahkan fitur baru ke aplikasi yang ada.

- [Kursus](): Jalur pelatihan dengan panduan yang mengajarkan cara mem-build aplikasi Android.
  Jika tidak, berikut ini adalah beberapa pilihan panduan developer penting yang harus Kalian ketahui.

### Dokumentasi Penting

Ada banyak banget dokumentasi yang udah di sediain Android Developer, berikut contoh nya:

- **Menentukan kebutuhan akses data sensitif**
- **Panduan performa aplikasi**
- **Ringkasan resource aplikasi**
- **Ringkasan Notifikasi**
- **Tata letak**
- **Gaya dan Tema**
- **DLL**

Karna banyak banget dokumentasi resmi, jadi mimin cuma melampirkan beberapa nya saja. 😀

---

# Buat Aplikasi Pertama Kamu

## Membuat Aplikasi Hello Newbie Master ID

### Sebelum mulai

[Instal Android Studio]() dulu di komputer kalian kalo kalian belum menginstall. Pastiin komputer kalian memenuhi persyaratan sistem yang diperlukan untuk menjalankan Android Studio (ada di bagian bawah halaman download) di dokumentasi resmi nya. kalo kalian memerlukan petunjuk yang lebih detail terkait proses installasi dan penyiapan, Kalian bisa kunjungi ke bagian [Install Android Studio]().

Di halaman belajar adroid dasar ini, Kalian akan membuat aplikasi Android pertama dengan template project yang disediakan oleh Android Studio. Kalian menggunakan Kotlin dan Jetpack Compose untuk menyesuaikan aplikasi Kalian. Perhatikan bahwa Android Studio selalu diupdate dan terkadang ada perubahan UI, jadi gak masalah kalo Android Studio Kalian terlihat sedikit berbeda dari screenshot yang ada di artikel ini. Kebetulan mimin pake _**Android Studio Chipmunk | 2021.2.1 Patch 2**_

#### Persyaratan

- Pengetahuan kotlin dasar

Kalo kalian belum belajar kotlin, kalian bisa kunjungi dulu ke bagian halaman tutoral [Belajar Kotlin]() sebelum melanjutkan ke tahap selanjutnya, kalian harus paham dulu tentang kotlin.

#### Yang dibutuhin

- Versi terbaru android studio

#### Yang akan dipelajari

- Cara membuat aplikasi Android dengan Android Studio
- Cara menjalankan aplikasi dengan alat Pratinjau di Android Studio
- Cara mengubah text dengan Kotlin
- Cara mengupdate User Interface (UI) dengan Jetpack Compose
- Cara melihat Pratinjau aplikasi dengan Pratinjau di Jetpack Compose

Berikut adalah tampilan akhir aplikasi:

![default preview](img/default-preview-1.png)

### Membuat project menggunakan template

Untuk membuat project di Android Studio:

1. Setelah kalian menginstall Android Studio Masuk kedalam aplikasi Android Studio.

2. Dalam dialog Welcome to Android Studio, klik New Project.
   ![default preview](img/Screensho-new-project.png)

Setelah itu Jendela New Project akan terbuka dengan daftar template yang disediakan oleh Android Studio.
![default preview](img/choose-template.png)

3. Pastiin kalo kalian pilih Phone and Jablet pada jenis template

4. Karna kita mau menggunakan Jetpack Compose Kalian bisa pilih template Empty Compose Activity untuk memilihnya sebagai template untuk project Kalian. Template Empty Compose Activity adalah template untuk membuat project sederhana yang bisa kalian gunakan untuk membuat aplikasi Compose. Template ini memiliki satu layar dan menampilkan teks "Hello Android!".

5. Klik Next. Dialog New Project akan terbuka. Kolom ini memiliki beberapa kolom untuk mengonfigurasi project Kalian.

6. Konfigurasikan project Kalian sebagai berikut:

Kolom **Name** digunain buat masukin nama project Kalian, untuk jenis project yang saya gunai yaitu "Build-First-App".

Biarin kolom **Package name** apa adanya. Ini adalah cara file Kalian bakal disusun dalam struktur file. Dalam hal ini, nama paket bakal menjadi com.example.greetingcard.

Biarin kolom **Save location** sebagaimana adanya. Project ini berisi lokasi tempat semua file yang terkait dengan project Kalian disimpan. Catat lokasi tersebut di komputer agar Kalian dapat menemukan file Kalian.

**Kotlin** sudah dipilih di kolom **Language**. Bahasa menentukan bahasa pemrograman yang ingin Kalian gunain buat project. Karena Compose hanya kompatibel dengan Kotlin, Kalian tidak dapat mengubah kolom ini.

Pilih **API 23: Android 6.0 (Marshmallow)** dari menu di kolom **Minimum SDK**. [Minimum SDK]() menunjukkan versi minimum Android yang dapat dijalankan oleh aplikasi Kalian.

Kotak centang **Use legacy android.support libraries** sudah tidak dicentang.
![default preview](img/init-project.png)

7. Tekan Finish. Proses ini mungkin memerlukan waktu lama - sembari menunggu Kalian dapat melakukan aktivitas lain. Ketika Android Studio sedang menyiapkan, status progres dan pesan menunjukkan apakah Android Studio masih menyiapkan project Kalian. Tampilannya mungkin terlihat seperti ini:
   ![default preview](img/process-running.png)

Pesan yang terlihat serupa dengan ini akan menginformasikan Kalian saat penyiapan project dibuat.

![default preview](img/gradle-sync.png)

8. Kalian mungkin melihat panel What's New yang berisi informasi terkini tentang fitur-fitur baru di Android Studio. Tutup sekarang.
   ![default preview](img/img-8.png)

9. Klik Split di kanan atas Android Studio, ini memungkinkan Kalian untuk melihat kode dan desain. Kalian juga dapat mengklik Code untuk melihat kode saja atau klik Design untuk melihat desain saja.
   ![default preview](img/img-9.png)

### Menemukan file project

Di bagian ini, Kalian akan terus menjelajahi Android Studio dengan lebih memahami struktur file.

1. Di Android Studio, lihat tab Project. Tab Project menampilkan file dan folder project Kalian. Saat Kalian menyiapkan project, nama paketnya adalah com.example.greetingcard. Kalian dapat melihat paket tersebut di sini, di tab Project. Paket pada dasarnya adalah folder tempat kode berada. Android Studio menyusun project dalam struktur direktori yang terdiri dari paket.

2. Jika perlu, pilih Android dari menu drop-down di tab Project.
   ![default preview](img/img-file-project.png)

Ini adalah tampilan standar dan susunan file yang Kalian gunain. Ini akan berguna saat Kalian menulis kode untuk project karena Kalian bisa dengan mudah mengakses file yang akan Kalian kerjakan di aplikasi. Namun, jika Kalian melihat file di file browser, seperti Finder atau Windows Explorer, hierarki file disusun dengan sangat berbeda.

3. Pilih Project Source Files dari menu drop-down. Sekarang Kalian dapat menjelajahi file dengan cara yang sama seperti di file browser apa pun.
   ![default preview](img/img-10.png)

4. Pilih Android lagi untuk beralih kembali ke tampilan sebelumnya. Kalian dapat menggunakan tampilan Android untuk latihan ini. Jika struktur file Kalian terlihat aneh, periksa untuk memastikan Kalian masih dalam tampilan Android.

### Memperbarui Text

---

# Dasar dasar android
