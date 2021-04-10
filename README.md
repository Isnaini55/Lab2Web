# Lab2Web

# Praktikum 2

# Pemograman WEB

~~~
Nama  : Isnaini Rizkyana
NIM   : 311910254
Kelas : TI.19.C1
~~~
## Langkah-langkah Praktikum
## 1. Membuat dokumen HTML
Buatlah dokumen HTML seperti berikut
~~~
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
    <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>.
Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.
</p>
    <!-- CSS Class Selector -->
    <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
</div>
</body>
</html>
~~~
Selanjutnya buka pada brwoser untuk melihat hasilnya.

![1  Membuat dokumen HTML](https://user-images.githubusercontent.com/81541764/114257496-a97ef980-99ea-11eb-97d5-401f3469aab4.JPG)

## 2. Mendeklarasikan CSS Internal
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
~~~
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
    h1 i { color:#6d6a6b;
    }
</style>
</head>
~~~
Selanjutnya simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat hasilnya.

![2  Mendeklarsi CSS Internal](https://user-images.githubusercontent.com/81541764/114257796-75a4d380-99ec-11eb-975e-13c5230445dd.JPG)

## 3. Menambahkan Inline CSS
Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
~~~
    <p style="text-align: center; color: #ccd8e4;">
~~~
Simpan kembali dan refresh kembali browser untuk melihat perubahannya.
