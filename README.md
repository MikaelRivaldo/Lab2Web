# Tugas

1. Persiapkan text editor misalnya VSCode.
2. Buat file baru dengan nama lab2_css_dasar.html
3. Buat struktur dasar dari dokumen HTML.
4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
5. Lakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/

# Membuat dokumen Html

`Untuk sourcodenya bisa menggunakan dibawah ini  :`

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CSS Dasar</title>
</head>
<body>
<header>
<h1>CSS Internal dan <i>Inline CSS</i></h1>
</header>
<nav>
<a href="lab2_css_dasar.html">CSS Dasar</a>
<a href="lab2_css_eksternal.html">CSS Eksternal</a>
<a href="lab1_tag_dasar.html">HTML Dasar</a>
</nav>
<!-- CSS ID Selector -->
<div id="intro">
<h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
<!-- CSS Class Selector -->
<a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
</div>
</body>
</html>

```

`Dan untuk hasilnya akan seperti ini  :`

![tampilan pertama](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/242f7e8f-c749-4720-918c-3345d6bad0cf)

`Selanjutnya Mendeklarasikan CSS Internal`

Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen

`Untuk sourcodenya bisa menggunakan dibawah ini:`

```html
<head>
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>

```

`Dan untuk hasilnya akan seperti ini  :`

![tampilan ke2](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/f078f983-5cce-4936-84a8-98588679bdad)

`Selanjutnya Menambahkan Inline CSS`
Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut

`Untuk sourcodenya bisa menggunakan dibawah ini:`

```html

<p style="text-align: center; color: #ccd8e4;">

```

`Dan untuk hasilnya akan seperti ini  :`

![tampilan inline css](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/724fdcf1-ad97-4dc8-ae02-17830c1e9ecd)

`Selanjutnya Menambahkan Membuat CSS Eksternal`

Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut

`Untuk sourcodenya bisa menggunakan dibawah ini:`

```html

nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}

```

`Dan untuk hasilnya akan seperti ini  :`

![tampilan css ekternal](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/d7fc125b-dd77-4cb3-9908-ad087567a460)

`Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>`

`Untuk sourcodenya bisa menggunakan dibawah ini:`

```html

<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>

```
`kita bisa sisipkan seperti dibawah ini`

![tampilan link](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/5e46f2d8-db73-448d-8319-6a38cdc415b4)

`Dan untuk hasilnya akan seperti ini  :`

![tampilan css ekternal](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/2fb334a0-4fda-45e5-a08c-175feda7d8a2)

`Selanjutnya Menambahkan Membuat CSS Selector`

Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut

`Untuk sourcodenya bisa menggunakan dibawah ini:`

```html

/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}

```

`Dan untuk hasilnya akan seperti ini  :`

![tampilan css selector](https://github.com/MikaelRivaldo/Lab2Web/assets/115770247/ecbe8400-4e85-4b7d-bcb5-5b44f59066ab)

---

Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya!
( <p id="paragraf-1" class="text-paragraf"> )


---

# Jawab

1.---

2.Ini adalah sebuah selektor CSS umum yang akan mempengaruhi semua elemen `<h1>` di halaman HTML.
    Dalam hal ini, gaya yang didefinisikan akan berlaku untuk setiap elemen `<h1>` di seluruh halaman.

   `#intro h1 {...}:`
    Ini adalah selektor CSS yang lebih spesifik dan berlaku hanya untuk elemen `<h1>` yang berada di dalam elemen dengan ID intro.
    Dalam hal ini, gaya yang didefinisikan hanya akan mempengaruhi elemen `<h1>` yang merupakan turunan dari elemen dengan ID intro.
    Dalam kedua kasus di atas, h1 dan `#intro h1` adalah selektor CSS yang mengacu pada elemen `<h1>`. 
    Namun, perbedaannya terletak pada ruang lingkup elemen yang dipengaruhi oleh gaya yang didefinisikan. 
    `h1 {...}` akan mempengaruhi semua elemen `<h1>` di halaman, sedangkan `#intro h1 {...}` akan mempengaruhi hanya elemen `<h1>` yang berada di dalam elemen dengan ID intro.

3.

















