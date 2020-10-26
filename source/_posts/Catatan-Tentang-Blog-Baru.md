---
title: Catatan Tentang Blog Baru
date: 2020-09-28 12:25:56
tags: [Web]
thumbnail: rumah1.jpg
---

{% asset_img rumah1.jpg "ilustrasi rumah"%}
Photo by Adrien Olichon on Unsplash

Bismillah.

Menurut saya blog merupakan sebuah rumah untuk tempat berbagai cerita, opini, dan hal lainnya. Seperti halnya memiliki rumah, ada kebahagiaan tersendiri bagi saya untuk memiliki blog baru dan dapat sepenuhnya saya kelola dan rawat.

Seperti sudah saya tulis di halaman [tentang](https://adisaktijrs.github.io/tentang/), bahwa blog ini merupakan blog baru yang menggantikan [blog lama](adisaktijrs.wordpress.com) saya di WordPress. Blog itu sudah saya gunakan selama lebih dari empat tahun dan tentu banyak sekali kenangan tertulis di sana. Maka dari itu blog itu akan tetap di sana, tidak akan pergi ke mana-mana. Dan selanjutnya saya akan menggunakan blog baru ini untuk menulis.

Blog baru ini memang berbeda dengan blog sebelumnya, dimana ini sebenarnya adalah sebuah web statis, sedangkan blog sebelumnya merupakan Content Management System (CMS) dari WordPress. Saya akan sedikit membahas tentang itu dan alasan saya pindah ke web statis ini.

### Web Statis dan CMS

Jika saya artikan secara sederhana, web statis itu adalah web yang hanya menggunakan HTML, CSS, dan JavaScript saja. Jadi ketika pengguna membuka web tersebut melalui browser maka server akan langsung memberikan file-file tersebut tanpa ada proses logika, routing, operasi database, dan sebagainya.

Sedangkan CMS dalam hal ini WordPress itu menggunakan bahasa PHP dan database SQL untuk membuat logika dan penyimpanan database. Jadi ketika pengguna meminta suatu halaman (mengakses halaman) maka PHP sebagai server scripting mengelola permintaan pengguna tersebut, melakukan query/pencarian di database, dan mengolahnya lalu mengirimkan hasil filenya ke pengguna. Jadi secara proses akan lebih panjang dan memakan lebih banyak waktu. Meskipun hanya berbeda beberapa mili detik.

### Alasan Berganti ke Web Statis

Ada beberapa alasan mengapa saya pindah. Namun untuk disclaimer baik web statis maupun WordPress memiliki keunggulan dan kekurangan masing-masing, bergantung dari kebutuhan penggunanya hehe.

#### 1. Kecepatan Akses

Web statis pada dasarnya adalah bentuk awal dari pengembangan web di masa lalu, dan tidak bisa dipungkiri kelebihan dari web statis adalah [kecepatan aksesnya](https://scotch.io/bar-talk/5-reasons-static-sites-rock). WordPress pada dasarnya cukup cepat, namun dengan banyaknya fitur, plugin, dan file eksternal dari pihak ketiga membuat peformanya turun cukup drastis. Berikut ini perbandingan dari blog saya dulu dan blog saya yang baru menggunakan tools dari [web.dev](https://web.dev/):
{% asset_img lama.png "peforma dari blog lama"%}
Ini adalah peforma dari blog saya yang lama. Dan dibawahnya peforma dari blog yang baru. Cukup terlihat sangat jauh perbandingannya.
{% asset_img baru.png "peforma dari blog baru"%}
Memang tidak adil rasanya membandingkan peforma web statis dengan WordPress, karena memang WordPress adalah CMS yang memiliki banyak sekali fitur dan kemudahan yang disediakan, maka pasti membuatnya lebih berat. Dan blog saya yang baru benar-benar saya buat seminimalis mungkin.

#### 2. Hosting dan Domain Gratis
Ini nih yang jauh lebih penting haha. Keduanya menyediakan fasilitas hosting dan domain gratis. Domain pada free plan di WordPress memberikan domain gratis berekstensi .wordpress.com.

Lalu blog baru saya menggunakan hosting di GitHub dan domain gratis berekstensi .github.io. Keduanya menggunakan ekstensi dari perusahaan penyedia masing-masing. Namun untuk gaya-gayaan di kalangan mahasiswa ilmu komputer tentu .github.io jauh lebih kece hehe.

#### 3. Pengelolaan dan Customisation
WordPress menang jauh di bagian pengelolaan konten. Tentu dengan editor barunya dan Jetpack sungguh sangat memudahkan untuk menulis dan mengelola konten.

Sedangkan blog baru saya menggunakan [Hexo.js](https://hexo.io/) yang merupakan Static Site Generator (SSG). Jadi saya membuat blog dengan API dari Hexo dan membuat UI dengan template engine EJS. Jadi ya ngoding juga akhirnya. Lalu untuk menulis konten saya menggunakan text editor dan menggunakan bahasa Markdown (.md). Namun setelah tema jadi dan tulisan sudah saya buat maka si Hexo ini akan secara otomatis di belakang layar men-generate semuanya menjadi file untuk web statis.

Memang agak ribet dibandingkan ketika saya menggunakan WordPress tetapi hal itu juga menjadi keunggulan dari membuat blog dengan Hexo. Saya sangat bebas untuk membuat blog dengan bentuk, presentasi tampilan, dan fitur seperti yang saya inginkan. Dan karena saya ingin membuat blog yang minimalis maka hal ini bisa dilakukan dengan Hexo. Di WordPress sebenarnya juga bebas untuk custom banyak hal, tapi itu tidak tersedia di free plan-nya. Yee gratis, tapi minta banyak hehe.

### Akhir Kata
Penggunaan web statis dengan SSG memang sedang hype dan naik daun. Maka dari itu saya akhirnya kepincut untuk mencoba menggunakannya. Saya menggunakan Hexo karena hanya dibutuhkan pengetahuan dasar HTML, CSS, JS, dan EJS sebagai template engine.

Dibandingkan dengan framework mewah seperti Gatsby, Next, Nuxt, dan lainnya yang membutuhkan pengetahuan dasar dari framework lain seperti React dan Vue, Hexo jauh lebih mudah untuk dipelajari dan digunakan untuk membuat web (khususnya blog). Seperti blog ini, juga hanya membutuhkan waktu beberapa hari untuk belajar API-nya dan untuk membuat template/tema blognya. Dan jika ingin menggunakan tema yang disediakan Hexo, maka akan lebih cepat dalam membuat blog.

Nah, semoga dengan blog baru ini saya bisa lebih produktif dan semoga juga ini tidak saya jadikan alasan untuk menunda menulis skripsi hehe.
