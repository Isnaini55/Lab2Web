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
![3  Menambahkan Inline CSS](https://user-images.githubusercontent.com/81541764/114258083-63c43000-99ee-11eb-9f9b-53a732343145.JPG)

## 4. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
~~~
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
~~~

![4  style CSS Eksternal](https://user-images.githubusercontent.com/81541764/114258389-5740d700-99f0-11eb-98b2-cc85b9334a6f.JPG)

Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>
~~~
<head>
    <!-- menyisipkan css eksternal -->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
~~~
Selanjutnya refresh kembali browser untuk melihat perubahannya.

![4  style CSS Eksternal (Link)](https://user-images.githubusercontent.com/81541764/114258298-e13c7000-99ef-11eb-8ded-8f86a34c24b2.JPG)


## 5. Menambahkan CSS Selector
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, tambahkan kode berikut.
~~~
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
~~~
Kemudian simpan kembali dan refresh browser untuk melihat perubahannya.
![5  ID selector](https://user-images.githubusercontent.com/81541764/114258611-fca87a80-99f1-11eb-885b-5966ea59be49.JPG)

## Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
   ~~~
   Saya menambahkan border dan warna border pada kode CSS, sehingga ada beberapa perubahan seperti gambar dibawah ini.
   ~~~
   ![Pertanyaan no1](https://user-images.githubusercontent.com/81541764/114267183-88d39580-9a24-11eb-9ea8-afc617f19d90.JPG)

2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
   ~~~
   Ketika kita mengganti nilai CSS elemen h1 {....} maka yang akan berubah yang memiliki tag h1 seperti <h1>CSS Internal dan Inline CSS</h1>
   dan <h1>Hello World</h1>. Sedangkan jika kita mengganti #intro h1{....} maka yang berubah hanya memiliki
   tag div id="intro" saja yang berubah seperti <h1> Hello World </h1>
   ~~~
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
    ~~~
    Jika ada deklarasi CSS secara internal kemudian ditambahkan CSS Eksternal dan inline CSS pada elemen yang sama, maka deklarasi inline CSS yang akan muncul pada browser.
    Karena salah satu manfaat dari inline CSS adalah permintaan HTTP yang lebih kecil, sehingga web server bisa lebih cepat membacanya.
    ~~~
   ![Capture](https://user-images.githubusercontent.com/81541764/114271914-fd66fe00-9a3d-11eb-80d8-c595beb2fb2b.JPG)
![Pertanyaan no3](https://user-images.githubusercontent.com/81541764/114271916-ffc95800-9a3d-11eb-8068-952aed7d55a3.JPG)


4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )
    ~~~
    Perbedaan dari class dan id adalah class di panggil menggunakan tanda titik (.) dan id dengan tanda pagar (#),
    jadi kedua deklarasi tetap akan tampil pada browser. Hanya saja class dapat di berikan pada banyak element html
    dan dapat di panggil sekaligus, sedangkan id hanya dapat bekerja pada satu penandaan saja.
    ~~~
![Pertanyaan no4 b](https://user-images.githubusercontent.com/81541764/114271834-9e08ee00-9a3d-11eb-90d2-45b6bf755142.JPG)
![Pertanyaan no4](https://user-images.githubusercontent.com/81541764/114271836-9fd2b180-9a3d-11eb-84ba-fd63843ae422.JPG)
