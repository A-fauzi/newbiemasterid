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

Setelah mengenal Android Studio, nah sekarang waktunya mulai membuat aplikasinya 😍

Lihat tampilan Code file MainActivity.kt. Perhatiin bahwa ada beberapa fungsi yang dihasilkan secara otomatis dalam kode ini, khususnya fungsi onCreate() dan setContent().

```kotlin
class MainActivity : ComponentActivity() {
   override fun onCreate(savedInstanceState: Bundle?) {
       super.onCreate(savedInstanceState)
       setContent {
           GreetingCardTheme {
               // A surface container using the 'background' color from the theme
               Surface(
                   modifier = Modifier.fillMaxSize(),
                   color = MaterialTheme.colors.background
               ) {
                   Greeting("Android")
               }
           }
       }
   }
}
```

Sekarang mimin bakal jelasin fungsi fungsi kode di atas:

Fungsi onCreate() adalah titik entri ke aplikasi ini dan memanggil fungsi lain untuk membuat antarmuka pengguna. Dalam program Kotlin, fungsi main() adalah tempat spesifik dalam kode Kalian tempat compiler Kotlin dimulai. Di aplikasi Android, fungsi onCreate() mengisi peran tersebut.
Jadi layak nya fungsi main() yang ada di kotlin untuk menjalankan program, di android menggunakan fungsi onCeate().

Fungsi setContent() dalam fungsi onCreate() digunakan untuk menentukan tata letak yang kalian buat melalui fungsi composable. Semua fungsi yang ditandai dengan anotasi @Composable dapat dipanggil dari fungsi setContent() atau dari fungsi Composable lainnya. Anotasi ini memberi tahu compiler Kotlin bahwa fungsi ini digunakan oleh Jetpack Compose untuk membuat UI.

> Catatan: Compiler mengambil kode Kotlin yang Kalian tulis, melihatnya baris demi baris, dan menerjemahkannya menjadi sesuatu yang dapat dipahami komputer. Proses ini disebut mengompilasi kode.

Selanjutnya, coba kalian lihat fungsi Greeting(). Fungsi Greeting() adalah fungsi composable. Perhatiin anotasi @Composable di atasnya. Fungsi composable mengambil beberapa input dan menghasilkan apa yang ditampilkan di layar.

```kotlin
@Composable
fun Greeting(name: String) {
   Text(text = "Hello $name!")
}
```

Kalian udah belajar fungsi sebelumnya di halaman [belajar kotlin](), kalo kalian belum mempelajari nya silahkan kunjungi halaman tersebut dan pelajari untuk memudahkan kalian belajar android.

![img](img/fungsi-composable.png)

- Nama fungsi @Composable menggunakan PascalCase.
- Harus menambahkan anotasi @Composable sebelum fungsi.
- Fungsi @Composable tidak dapat menampilkan apa pun.

```kotlin
@Composable
fun Greeting(name: String) {
   Text(text = "Hello $name!")
}
```

Sekarang kalian perhatiin, fungsi Greeting() menggunakan nama dan menampilkan Hello.

1. Sekarang ubah fungsi Greeting() untuk memperkenalkan diri Kalian, Jangan menggunakan "Hello" kaya contoh kode dibawah:

```kotlin
@Composable
fun Greeting(name: String) {
   Text(text = "Hi, my name is $name!")
}
```

2. Build ulang DefaultPreview dengan menekan tombol di kiri atas panel desain

![img](img/build-preview.png)

Nah sekarang kalian berhasil mengubah teks, tapi text disini di set nama sebagai Android yang pasti bukan nama Kalian. Sekarang, Kalian akan mempersonalisasinya agar memperkenalkan nama kalian sendiri.

Fungsi `DefaultPreview()` adalah fitur keren yang memungkinkan kalian melihat tampilan aplikasi tanpa harus mem-build seluruh aplikasi. Agar menjadi fungsi Pratinjau, kalian perlu menambahkan anotasi `@Preview`.

Seperti yang udah kalian lihat nih, anotasi `@Preview` menggunakan parameter yang disebut `showBackground`. Jika `showBackground` disetel ke true, latar belakang akan ditambahkan ke pratinjau aplikasi kalian.

Android Studio secara default menggunakan tema terang untuk editor sehingga perbedaan antara `showBackground` = true dan `showBackground` = false mungkin bakal sulit dilihat. Tapi, inilah perbedaan tampilan dengan tema gelap. Perhatiin latar belakang putih pada gambar yang disetel ke true.

![img](img/preview-background.png)

2. Sekarang ubah fungsi DefaultPreview() dengan nama Kalian. Kemudian, build ulang dan lihat text yang dipersonalisasi.

```kotlin
@Preview(showBackground = true)
@Composable
fun DefaultPreview() {
   GreetingCardTheme {
       Greeting("Akhmad Fauzi")
   }
}
```

![img](img/build-view.png)

### Mengubah warna latar belakang

Sekarang Kalian punya teks pengantar, tapi hal ini bikin bosen karna ga ada style apa apa. Di bagian ini, Kalian bakal mempelajari cara mengubah warna latar belakang.

Untuk menetapkan warna latar belakang yang berbeda pada pendahuluan, Kalian harus mengapit teks dengan Surface. Surface adalah penampung yang menampilkan bagian UI tempat Kalian dapat mengubah tampilan, seperti warna latar belakang atau batas.

1. Untuk mengapit teks dengan Surface, tandai baris teks, tekan (Alt+Enter untuk Windows atau Option+Enter di Mac), lalu pilih Surround with widget.

![img](img/img-1.png)

2. Pilih Surround with Container.

![img](img/img-2.png)

Penampung default yang bakal dikasih ke Kalian adalah Box, tapi Kalian dapat mengubahnya ke jenis penampung lainnya.

![img](img/img-3.png)

3. Hapus `Box` dan ketik `Surface()` sebagai gantinya.

```kotlin
@Composable
fun Greeting(name: String) {
   Surface() {
       Text(text = "Hi, my name is $name!")
   }
}
```

4. Penampung Surface memiliki parameter color, tetapkan ke Color.

```kotlin
@Composable
fun Greeting(name: String) {
   Surface(color = Color) {
       Text(text = "Hi, my name is $name!")
   }
}
```

5. Saat mengetik Color, Kalian pasti melihat warnanya merah dan digaris bawahi. Untuk mengatasi hal ini, scroll ke bagian atas file yang bertuliskan import, lalu tekan ketiga tombol.

![img](img/import.png)

6. Tambahin pernyataan ini ke bagian bawah daftar impor.

```kotlin
import androidx.compose.ui.graphics.Color
```

Daftar lengkap impor bakal keliatan kaya gini:

```kotlin
import android.os.Bundle
import androidx.activity.ComponentActivity
import androidx.activity.compose.setContent
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.material.MaterialTheme
import androidx.compose.material.Surface
import androidx.compose.material.Text
import androidx.compose.runtime.Composable
import androidx.compose.ui.Modifier
import androidx.compose.ui.tooling.preview.Preview
import com.example.myapplication.ui.theme.GreetingCard
import androidx.compose.ui.graphics.Color
```

7. Didalam kode Kalian, praktik terbaiknya adalah dengan tetap mencantumkan impor menurut abjad. Untuk ngelakuin nya, tekan `Help` di `toolbar` bagian atas, ketik `Optimize Imports`, lalu klik `Optimize Imports`.

Sekarang daftar lengkap impor bakal keliatan kaya gini:

```kotlin
import android.os.Bundle
import androidx.activity.ComponentActivity
import androidx.activity.compose.setContent
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.material.MaterialTheme
import androidx.compose.material.Surface
import androidx.compose.material.Text
import androidx.compose.runtime.Composable
import androidx.compose.ui.Modifier
import androidx.compose.ui.graphics.Color
import androidx.compose.ui.tooling.preview.Preview
import com.example.myapplication.ui.theme.GreetingCard
```

8. Perhatiin Color yang Kalian ketik di tanda kurung Surface udah berubah dari warna merah dan digaris bawahi menjadi digaris bawahi warna merah. Untuk memperbaikinya, tambahkan titik setelahnya. Kalian bakal lihat pop-up yang menampilkan berbagai opsi warna.

Ini adalah salah satu fitur keren di Android Studio, Dalam hal ini, Kalian tahu bahwa Kalian mau nentuin warna sehingga fitur ini akan menyarankan warna yang berbeda.

![img](img/color.png)

9. Pilih warna untuk background text Kalian. disini mimin menggunakan magenta, tapi Kalian bisa pilih color favorit Kalian.

10. Klik Build & Refresh. Sekarang teks dikelilingi oleh warna yang Kalian pilih.

![img](img/finish.png)

### Menambahkan padding

Nah sekarang teks Kalian punya warna latar belakang nih, selanjutnya Kalian akan menambahkan beberapa spasi (padding) di sekitar teks.

`Modifier` digunakan untuk menambah atau menghias komposisi. Satu Pengubah yang dapat Kalian gunakan adalah padding pengubah, yang menerapkan ruang di sekitar elemen (dalam hal ini, menambahkan ruang di sekitar teks). Ini dicapai dengan menggunakan fungsi Modifier.padding().

1.  Tambahkan impor ini ke bagian pernyataan impor.
    Pastiin untuk menggunakan Optimalkan Impor untuk mengurutkan impor baru berdasarkan abjad.

```kotlin
import androidx.compose.ui.unit.dp
import androidx.compose.foundation.layout.padding
```

2. Tambahkan pengubah padding pada teks dengan ukuran 24.dp, klik Build & Refresh.

> Catatan: Anda mempelajari lebih lanjut tentang kepadatan-independen piksel (DP) di jalur berikutnya, tetapi merujuk ke artikel ini jika Anda ingin membaca lebih lanjut sekarang.

```kotlin
@Composable
fun Greeting(name: String) {
   Surface(color = Color.Magenta) {
       Text(text = "Hi, my name is $name!", modifier = Modifier.padding(24.dp))
   }
}
```

![img](img/padding.png)

Mantap👏 - Kalian udah buat aplikasi Android pertama di Compose! Ini adalah pencapaian yang bagus. Kalian bisa latihan dan coba coba praktekin apa yang udah kita pelajari.

Semangat💪

Setelah ini kalian bisa masuk ke artikel berikut nya untuk mempelajari [Dasar dasar android]()
