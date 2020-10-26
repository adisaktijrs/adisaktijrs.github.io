---
title: Bagaimana Fanatisme Melumpuhkan Teknisi Perangkat Lunak
date: 2020-10-01 10:57:48
tags: [Opini]
thumbnail: people.jpg
---
{% asset_img people.jpg "Ilustrasi tentang pilihan" %}
Photo by Ethan Hu on Unsplash

Saya ingat ketika pertama kali membuka laman dokumetasi dari [Express](http://expressjs.com/), framework dari Node.js yang menggunakan Static Site Generator (SSG). Karena saya penasaran dengan framework SSG apa yang mereka gunakan, maka saya melihat ke laman GitHub mereka. Dan di situ saya agak kaget. Kurang lebih ini yang saya pikirkan dalam kepala saya:

{% blockquote %}
Lah, kok pakainya Jekyll? Itu kan SSG dari bahasa Ruby. Kenapa engga pakai yang dari ekosistem JavaScript, padahal banyak juga SSG-nya.
{% endblockquote %}

Dari situ, saya mulai menyadari bahwa saya 'mulai fanatis' dengan hal yang sedang saya pelajari sekarang: Ekosistem JavaScript.

### Kenapa Orang Cenderung Fanatis
Secara umum, fanatisme bisa terjadi karena perilaku investasi. Secara sederhana, ketika kita mulai menginvestasikan waktu, tenaga, uang, dan sebagainya pada suatu hal, kita akan memiliki kecenderungan meyakinkan diri sendiri bahwa pilihan yang telah kita pilih itu adalah paling baik dari semua pilihan yang ada.

Lalu, semakin banyak tenaga, waktu, dan uang yang kita investasikan di sana, semakin besar kecenderungan kita untuk menjadi fanatis pada objek investasi kita tersebut.

### Ternyata Sudah Sejak Dulu Saya Fanatis
Jika saya berkontemplasi sedikit, saya ingat bahasa server-side yang pertama saya pelajari adalah PHP pada semester tiga perkuliahan.

Dan saya ingat juga bahwa dulu saya sering sekali melakukan googling dengan query: 'PHP vs. bla bla bla' dan berharap mendapat artikel yang menguatkan PHP dari sisi perbandingan manapun haha.

Dan saya ingat juga, dulu di semester empat akhir dosen saya pernah memberikan saran bahwa fitur ini bisa dibuat lebih bagus dengan menggunakan JavaScript (JS) agar tidak full-reload ketika satu aksi dilakukan. Dan ternyata saya tetap stick, dan tidak menggunakan itu, karena ingin satu tugas project itu sepenuhnya menggunakan PHP haha.

### Lubang Jebakan Fanatisme bagi Teknisi Perangkat Lunak
Saya mulai sadar tentang bahaya fanatisme software developer pada satu bahasa/teknologi tertentu ketika melihat video mas Ryan Dahl (kreator dari Node.js) pada acara JSConf EU 2018 tentang hal-hal yang dia sesalkan pada pengembangan Node.js (lihat videonya [di sini](https://www.youtube.com/watch?v=M3BM9TB-8yA)). Terlepas dari tidak sejalannya beliau dengan beberapa tim inti pengembang Node.js pada masa itu, tetapi ini cukup menampar juga.

{% blockquote %}
Ryan Dahl, kreator Node.js, menyatakan sendiri tentang kelemahan yang ada pada Node.js!
{% endblockquote %}

Selain itu beliau juga pernah menyatakan kelebihan bahasa Go dibandingkan dengan Node.js. Dan sekarang beliau sedang membuat JS runtime baru: Deno, sebagai sukesor Node.js.

Tamparan selanjutnya yang saya alami saat saya mulai fanatis pada JS adalah ketika saya melihat Podcast dari [Pak Dika dengan Pak Riza Fahmi](https://www.youtube.com/watch?v=ohL5VIHs36s). Sosok pak Riza Fahmi ini memang nama besar di komunitas JS di Indonesia, tidak perlu dijelaskan lebih jauh.

Pada podcast itu hal yang menyadarkan saya adalah ketika pertanyaan Pak Dika ke beliau tentang pengalaman beliau dalam pengembangan perangkat lunak. Saya awalnya berpikir pasti beliau akan menomorsatukan JS dong. Tapi ternyata saya salah, beliau justru menyarankan agar kita tidak mengotak-ngotakan seorang pengembang perangkat lunak dengan sebutan web developer, Android dev, iOS dev dst. Beliau justru menyuruh untuk menggunakan istilah software developer. Dengan tujuan agar kita selalu membuka pikiran pada hal-hal baru dan tidak hanya bisa satu teknologi saja.

Saran dari Pak Riza Fahmi ini justru lebih luas lagi, tidak hanya menyarankan kita untuk tidak fanatis/hanya menggunakan satu framework/bahasa saja, tapi justru menyarankan agar kita tidak hanya menjadi pengembang di satu platform saja.

### Sisi Negatif Fanatisme
Saya akan coba merangkum sedikit tentang downside dari fanatisme. Ini bersumber dari opini pribadi yang berakar dari nasihat, saran, dan hal lain dari berbagai sumber.

#### 1. Teknologi Terus Berkembang, Developer?
Saya mendengar bahwa dulu Bapak Ibu dosen kita, ketika pertama kali belajar bahasa pemrograman menggunakan bahasa BASIC. Sekarang bayangkan, jika mereka/kolega mereka terlampau suka dengan bahasa tersebut dan tidak belajar bahasa lain? Bagaimana mereka mengimplementasikan pengetahuan mereka pada logika bisnis industri sekarang yang sudah menggunakan bahasa modern seperti Go, JS, Java?

Di sini fanatisme berlebihan akan membuat kita sebagai pengembang perangkat lunak menjadi tertutup dengan perkembangan teknologi yang ada. Dan ketika ada teknologi baru datang, kita menutup mata, lalu di saat apa yang kita suka mulai kehilangan pasar, kita baru akan memulai start? Padahal akan banyak anak-anak baru (generasi mendatang) yang setiap waktu bisa menggantikan kita dengan pengetahuan tentang teknologi terbaru.

Jangan sampai fanatisme membuat kita berhenti belajar.

#### 2. Mempersempit Peluang
Jika ada klien meminta kita untuk membuat sebuah web dengan framework A lalu apakah kita bilang pada mereka bahwa kita adalah developer yang menggunakan framework B? Tentu tidak masalah, namun peluang kita semakin menyempit dan terkotak hanya pada framework B saja.

#### 3. Fanatisme Tidak Sekeren itu!
Semakin fanatis pada satu hal akan membuat kita nampak tidak berpengalaman. Ada satu quote yang saya temukan dari [jawaban pengguna Quora](https://www.quora.com/Why-are-most-developers-fanatic-of-a-programming-language) tentang topik ini.

{% blockquote Anonim, Quora User %}
Most fanatics are people who just lack the experience of doing it the other way.
{% endblockquote %}

Kebanyakan orang fanatik adalah orang-orang yang tidak memiliki pengalaman melakukannya dengan cara lain. Saya jadi ingat dulu ketika saya pertama kali belajar silat di kelas satu SMA, ketika di rumah saya jadi sering nendang-nendang tidak jelas. Dan akhirnya diingatkan oleh bapak tentang satu hal: 'Terlalu berlebihan dalam show-off pada satu hal itu memperlihatkan bahwa kamu adalah pemula' (maaf OOT hehe).

Dari situlah saya mulai sadar bahwa saya fanatis pada JS, karena saya masih pemula di sana. Dan sangat disayangkan kalau nanti saya tidak belajar hal baru/teknologi baru hanya karena saya fanatis pada JS.

### Akhir Kata dan Saran
Saran ini saya dapat dari banyak pihak, kurang lebih seperti ini: Fanatisme itu sah-sah saja, tetapi dalam kadar yang tepat agar kita bisa menjadi ahli dalam satu bidang, tetapi tidak lupa untuk selalu meng-upgrade kemampuan diri dengan teknologi baru. Jadilah 'Jack of all trades, master of some'. Pelajari teknologi yang kamu suka dan bisa membuatmu membayar tagihan (peluang project dan kerja banyak). Dan jangan lupa melihat trend teknologi terbaru.

Kita bisa melihat banyak contoh developer hebat yang meski mereka dikenal karena keahliannya di satu bidang/teknologi tapi justru selalu terbuka dengan teknlogi lain dan menggunakannya sesuai dengan kebutuhan. Tambahan sedikit: Alasan Tim Express menggunakan Jekyll

{% blockquote Express.js Team https://github.com/expressjs/expressjs.com#why-use-jekyll-instead-of-an-express-based-solution Express GitHub Repository %}
Why use Jekyll instead of an Express-based solution? Jekyll comes built-in with GitHub Pages. Since we are already using GitHub Pages to host the website, it makes sense to leverage the capabilities it provides. **It's all about using the right tool, for the right job, under the right circumstances.**
{% endblockquote %}
