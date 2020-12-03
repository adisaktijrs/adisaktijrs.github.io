---
title: Kita Tetap Butuh Mentor
date: 2020-12-03 16:11:59
tags: [Opini, Web]
thumbnail: forest.jpg
---
![](forest.jpg)

<span>Photo by <a href="https://unsplash.com/@olipaulgibbs?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Oli Gibbs</a> on <a href="https://unsplash.com/s/photos/forest-from-top?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>

Bismillah.

Sudah sebulan saya tidak menulis, rasanya kangen juga menulis hal acak dan ringan untuk menikmati waktu luang.

Saya ingin cerita tentang salah satu opini saya tentang belajar. Sebagai disclaimer, opini ini saya tulis tanpa dasar literasi sama sekali. Saya sedang malas menulis hal yang berat hehe.

Pemikiran ini sebenarnya saya dapat dari pengamatan pribadi (sebagian besar tulisan saya memang kebanyakan [self-referencing](https://en.wikipedia.org/wiki/Self-reference#In_language)). Selain itu, opini ini juga sebatas apa yang saya lalui ketika belajar di bidang IT, tapi barangkali bisa menjadi lebih umum.

{% blockquote %}
Sehebat apapun, kita tetap butuh mentor
{% endblockquote %}

Dulu saya berpikir bahwa belajar secara mandiri itu berarti belajar hal baru di luar kelas, yang artinya dengan melakukan pengamatan dan eksperimen yang [secara empiris](https://pendidikan.co.id/pengertian-empiris/#:~:text=Empiris%20merupakan%20suatu%20keadaan%20yang,juga%20eksperimen%20yang%20pernah%20dilakukan.) dilakukan oleh diri sendiri.

Hal itu yang hampir selalu saya lakukan ketika belajar banyak hal di bidang IT. Lalu di masa 'akselerasi' ini, saya belajar hal kecil yang saya luput: Sekeras apapun belajar sendiri, tetap akan kalah efektif dibandingkan dengan belajar dengan bantuan mentor.

Salah satu contoh yang saya alami yaitu ketika saya belajar konsep [Object and Array Destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment) di JavaScript (These codes below are just examples, bear with me hehe).

Ada sebuah tantangan yang harus saya lakukan dari online course yang saya ikuti di Udemy, yaitu menerapkan konsep destructuring ini untuk menampilkan data dari `practice.js` kedalam sebuah code JSX yang tidak boleh diubah.

```js
//practice.js
const cars = [
  {
    model: "Honda Civic",
    coloursByPopularity: ["black", "silver"],
    speedStats: {
      topSpeed: 140,
      zeroToSixty: 8.5
    }
  },
  {
    model: "Tesla Model 3",
    coloursByPopularity: ["red", "white"],
    speedStats: {
      topSpeed: 150,
      zeroToSixty: 3.2
    }
  }
];

export default cars;

```

Data itu harus saya masukan ke code JSX di bawah ini tanpa mengubahnya, maka saya harus melakukan destructuring terlebih dahulu.

```js
//...
ReactDOM.render(
  <table>
    <tr>
      <th>Brand</th>
      <th>Top Speed</th>
    </tr>
    <tr>
      <td>{tesla.model}</td>
      <td>{teslaTopSpeed}</td>
      <td>{teslaTopColour}</td>
    </tr>
    <tr>
      <td>{honda.model}</td>
      <td>{hondaTopSpeed}</td>
      <td>{hondaTopColour}</td>
    </tr>
  </table>,
  document.getElementById("root")
);
```

Karena saya sudah belajar konsep ini dan tentu dengan berbekal googling sana-sini akhirnya saya bisa menyelesaikannya. Lalu setelah itu saya melanjutkan ke sesi berikutnya yang merupakan sesi solution yang berisi pemecahan masalah dan pembahasan dari mentor untuk tantangan tersebut.

Berikut ini adalah hasil cara saya dan mentor saya dalam melakukan destructuring:

```js
// My solution sucks, but it still works tho haha.
const [honda, tesla] = cars;

const [
  {
    coloursByPopularity: [hondaTopColour],
    speedStats: {topSpeed: hondaTopSpeed}
  },
  {
    coloursByPopularity: [teslaTopColour],
    speedStats: {topSpeed: teslaTopSpeed}
  }
] = cars;

// Best practice from my mentor, it was so much better than mine.
const [honda, tesla] = cars;

const {speedStats: {topSpeed: hondaTopSpeed}} = honda;
const {speedStats: {topSpeed: teslaTopSpeed}} = tesla;

const {coloursByPopularity: [hondaTopColour]} = honda;
const {coloursByPopularity: [teslaTopColour]} = tesla;
```
Solusi yang saya buat memang bekerja sesuai yang dibutuhkan, tetapi ini masih redudan dan sulit dibaca (karena harus memasukkan `coloursByPopularity` dan `speedStats` di satu konstanta). Sedangkan solusi dari mentor saya jelas lebih readable dan lebih modular.

Jika saya belajar tanpa mentor pasti saya akan terus menggunakan cara 'bad practice' asal programnya berjalan (seperti ketika saya menggunakan Mongoose di banyak project).

Dari hal kecil itulah saya percaya bahwa sehebat apapun cara kita belajar hal baru, masih akan kalah efektif dengan orang yang belajar hal baru dengan bantuan mentor, meski hanya satu arah (melihat tutorial, online course dsb).

Selain itu hal yang tidak saya dapat dari belajar tanpa mentor adalah kekurangan di sisi kurikulum/roadmap yang terarah. Umumnya si mentor sudah lebih tau roadmap yang tepat dalam belajar hal tertentu terutama bagi para noobian

Lalu terakhir, berita baiknya adalah di masa sekarang ini sudah terbuka semua kesempatan untuk belajar hampir semua hal. Bahkan sudah banyak organisasi yang memberikan fasilitas belajar dan mentoring secara gratis. Nah, tinggal kitanya bagaimana nih menanggapi kesempatan seperti sekarang ini (nasihat ke diri sendiri haha).

Salam dan see ya next time 😁
