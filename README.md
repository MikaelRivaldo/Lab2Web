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




