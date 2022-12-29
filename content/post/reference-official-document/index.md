---
title: Beberapa referensi teknologi untuk dipelajari
description: Saya akan memberikan beberapa referensi teknologi yang wajib dipelajari untuk membuat sistem aplikasi
slug: referensi-teknologi
date: 2022-12-28 00:00:00+0000
image: reference.jpg
categories:
- Reference
- Programming
tags:
- Reference Tag
---


#### Halo Ngab!,

#### Kali ini gue bakal bagiin beberapa referensi teknologi buat ngembangin sistem aplikasi nih, ini sih cocok banget buat kalian yang baru mau belajar tapi bingung nentuin arah tujuan "labil ya hehe".

#### Nah.. dalam pengembangan sistem aplikasi itu sebenernya ada dua role yang mengerjakan, yang pertama ada yang nama nya, "Front-end". Dia ini yang bertanggung jawab untuk mengembangkan aplikasi secara tampilan bagian depan, seperti tombol, card view, animation, dan widget lainya sehingga role ini dituntut dapat mengembangkan aplikasi secantik mungkin :)

#### yang kedua ada yang nama nya, "Back-end". Nah untuk role yang satu ini gak kalah penting dalam pengembangan sistem aplikasi karna dia yang akan sediain berbagai macam data untuk nanti di olah dan di kelola oleh "Front-end".

#### Langsung aja gue bakal kasih kalian referensi teknologi yang di pake di kedua role tersebut, agar nanti nya dapat mengembangkan sistem aplikasi secara utuh.

>## Technology Back-end
>
> 1. **MySQL (Basis Data)**
>
> #### MySQL adalah sistem manajemen basis data relasional (RDBMS) yang populer. RDBMS adalah sistem manajemen basis data yang menyimpan data dalam bentuk tabel yang saling terkait dengan menggunakan relasi antar tabel. MySQL merupakan salah satu RDBMS yang paling sering digunakan, karena mudah digunakan, cepat, dan bersifat open source (gratis). MySQL dapat digunakan untuk mengelola basis data yang berisi berbagai jenis data, seperti data transaksi, data inventori, data pelanggan, dan lain-lain. MySQL dapat diintegrasikan dengan berbagai bahasa pemrograman, seperti PHP, Java, dan Python, sehingga dapat digunakan dalam pengembangan aplikasi web, sistem informasi, dan lain-lain.

---

> 2.  **Postman (API Testing)**
>
> #### Postman adalah aplikasi atau alat yang digunakan untuk melakukan tes dan debugging API (Application Programming Interface). API adalah sekumpulan fungsi yang disediakan oleh sebuah sistem atau aplikasi untuk dapat diakses dan digunakan oleh aplikasi atau sistem lain. Postman memungkinkan pengguna untuk mengirim permintaan HTTP (Hypertext Transfer Protocol) ke server dan menerima respons yang dikirim oleh server. Permintaan HTTP dapat berupa GET, POST, PUT, DELETE, dan lain-lain. Postman juga memiliki fitur-fitur yang berguna seperti environment variable, collection, testing, mock server, dan lain-lain. Postman banyak digunakan oleh developer untuk menguji API sebelum aplikasi atau sistem tersebut dipublikasikan.

---

> 3. **Springboot (Framework)**
>
> #### Spring Boot adalah framework atau kerangka kerja yang dikembangkan oleh Pivotal untuk memudahkan pengembangan aplikasi Java. Spring Boot merupakan bagian dari proyek Spring yang lebih luas, yang memfokuskan pada kemudahan pengembangan aplikasi Java dengan menyediakan beragam fitur dan konfigurasi yang telah terotomatisasi. Spring Boot menyediakan cara mudah untuk membuat aplikasi Java yang independen, yang dapat dijalankan langsung dari command line atau dari sebuah web container seperti Apache Tomcat. Spring Boot juga menyediakan cara untuk mengkonfigurasi dan mengelola dependensi aplikasi dengan menggunakan Maven atau Gradle. Spring Boot sangat populer karena memudahkan pengembangan aplikasi Java dengan mengurangi konfigurasi yang diperlukan dan memberikan akses ke fitur-fitur yang berguna dari Spring Framework.

---

> 4. **Java (Bahasa Pemrograman)**
> 
> #### Java adalah bahasa pemrograman yang dikembangkan oleh Sun Microsystems (sekarang Oracle) pada tahun 1995. Java merupakan bahasa pemrograman yang bersifat general-purpose, artinya bahasa ini dapat digunakan untuk membuat berbagai macam aplikasi, seperti aplikasi desktop, aplikasi web, sistem operasi, dan lain-lain. Java mengadopsi sintaksis dari bahasa C++, namun memiliki tipe data yang lebih sederhana dan menggunakan garbage collection untuk mengelola memori secara otomatis. Java juga memiliki fitur-fitur seperti keamanan, portabilitas, dan multithreading, yang membuatnya sangat cocok untuk pengembangan aplikasi yang dapat dijalankan di berbagai sistem operasi. Java juga merupakan bahasa pemrograman yang paling populer di dunia, dan banyak digunakan oleh perusahaan-perusahaan besar di berbagai industri.

---

> #### Technology Front-end
>
>1. **HTML**
>
> #### HTML (HyperText Markup Language) adalah bahasa markup yang digunakan untuk menentukan struktur dan konten dari sebuahhalaman web. HTML menggunakan tag-tag yang ditandai dengan tanda kurung siku untuk menandai elemen-elemen yang ada pada halaman, seperti judul, paragraf, daftar, dan lain-lain.
>
```yaml
<html>

<head>
    <title>My Website</title>
</head>

<body>
    <h1>Welcome to my website</h1>
    <p>This is a paragraph on my website</p>
    <ul>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
</body>

</html>

```
>
> #### Di atas adalah contoh sederhana dari sebuah halaman web yang ditulis dengan HTML. Halaman tersebut > memiliki judul "My
> #### Website", dan terdiri dari sebuah judul utama ("Welcome to my website") dan sebuah paragraf. Di bawahnya, terdapat
> #### sebuah daftar dengan tiga item.
>
> #### HTML merupakan bagian dasar dari pengembangan web, dan sangat penting untuk dipahami oleh front-end developer atau siapa saja yang tertarik untuk membuat atau mengelola website.

---

> #### 2. **CSS**
>
> #### CSS (Cascading Style Sheets) adalah bahasa yang digunakan untuk mengontrol tampilan dan nuansa dari sebuah halaman web. Dengan CSS, Anda dapat mengatur aspek-aspek seperti warna, font, margin, dan layout dari elemen-elemen pada halaman web.
>
> #### CSS ditulis dalam file terpisah dari HTML, dan kemudian di-include pada halaman web menggunakan tag
><link>. 
> #### Dengan cara ini, Anda dapat mengatur gaya dari seluruh website dengan mudah, tanpa perlu mengubah kode HTML masing-masing halaman.
>
> #### Contoh CSS:
>
```yaml
body {
font-family: Arial, sans-serif;
color: #333;
background-color: #fff;
margin: 0;
padding: 0;
}

h1 {
font-size: 2em;
margin-bottom: 0.5em;
color: #069;
}

p {
font-size: 1em;
line-height: 1.5;
margin-bottom: 1em;
}

```
>
> #### Di atas adalah contoh sederhana dari sebuah file CSS yang mengatur font, warna, dan margin dari elemen-elemen pada halaman web. Dengan CSS, Anda dapat mengontrol tampilan dari seluruh website dengan mudah, tanpa perlu mengubah kode HTML masing-masing halaman.
>
> #### CSS merupakan bagian penting dari pengembangan web, dan sangat penting dipahami oleh front-end developer atau siapa saja yang tertarik untuk membuat atau mengelola website.

---

>3. **Javascript**
>
> #### JavaScript adalah bahasa pemrograman yang digunakan untuk menambahkan interaksi dan fitur dinamis pada situs web. JavaScript dapat digunakan untuk menciptakan efek animasi, menangani masukan pengguna, dan mengambil dan menampilkan data dari server. JavaScript biasanya dijalankan di browser web, tetapi juga dapat dijalankan di server menggunakan runtime seperti Node.js.
>
> #### JavaScript merupakan salah satu bahasa pemrograman yang paling populer di dunia, dan sangat penting bagi pengembangan aplikasi web modern. Banyak framework dan library JavaScript yang tersedia, seperti React, Angular, dan Vue.js, yang
> #### memudahkan pengembangan aplikasi web dengan JavaScript.
>
---

>4. **React Js**
>
> #### React (juga dikenal sebagai React.js atau ReactJS) adalah sebuah library JavaScript yang dikembangkan oleh Facebook yang digunakan untuk membangun antarmuka pengguna (UI) dalam aplikasi web. React menggunakan prinsip-prinsip pemrograman terstruktur yang disebut "react components" untuk membuat UI yang terdiri dari bagian-bagian kecil yang dapat digunakan kembali.
>
> #### React menggunakan sintaksis yang disebut JSX, yang memungkinkan Anda menulis kode HTML yang terintegrasi dengan
> #### JavaScript. Dengan menggunakan React, Anda dapat membangun aplikasi web yang responsif dan skalabel dengan mudah. React
> #### juga dapat digunakan untuk membangun aplikasi mobile dengan menggunakan framework seperti React Native.
>
---

#### Nah.. Jadi itu adalah beberapa mengenai teknologi yang dapat membuat sistem aplikas, sebenernya banyak banget cuma ga mungkin kalo dibahas semua dalam satu artikel wkwkwk.

#### Berikan saya beberapa ide atau topik yang ingin Anda bahas, dan saya akan mencoba membantu Anda membuat outline untuk artikel tersebut. Dengan memiliki ide yang jelas tentang apa yang ingin Anda tulis, saya dapat membantu Anda menyusun struktur yang sesuai dan mengembangkan ide-ide Anda menjadi sebuah artikel yang menarik dan bermanfaat bagi pembaca.

>Info lebih lanjut tentang saya, pantau link github: [my-github]https://github.com/A-fauzi
>
>Want a site like this? Check out [hugo-theme-stack-stater](https://github.com/CaiJimmy/hugo-theme-stack-starter)
>
> Photo by [Pawel Czerwinski](https://unsplash.com/@pawel_czerwinski) on [Unsplash](https://unsplash.com/)
