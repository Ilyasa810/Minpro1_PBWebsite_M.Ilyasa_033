# 🌐 Portfolio Website Muhammad Ilyasa' 'Izzuddin
### Mini Project 1 Praktikum Pemrograman Berbasis Website (PBW)

---

## 👤 Profil

|**Nama :** Muhammad Ilyasa' 'Izzuddin|
|--------|
|**NIM :** 2409116033|
|**Kelas :** A '2024 Sistem Informasi| 

Website ini merupakan website portofolio sederhana yang dibuat menggunakan HTML dan CSS serta Bootstrap.

Website ini menampilkan informasi profil, kemampuan, dan sertifikat.

---

## 🛠 Teknologi yang Digunakan

Website ini dibuat menggunakan teknologi berikut:

- HTML5
- CSS3
- Bootstrap 5

---

## 📷 Tampilan Website

|🏠 Home Section|
|------|
|Menampilkan halaman utama yang berisi nama dan perkenalan singkat.|
|<img width="1920" height="842" alt="image" src="https://github.com/user-attachments/assets/68951542-b624-44d1-b7f1-63ff538c9a23" />|

---

|👨‍💻 About Me Section|
|-------|
|Menampilkan informasi tentang diri serta skill yang dimiliki dengan progress bar.|
|<img width="960" height="505" alt="{EF0F0DB2-4C01-44A5-862D-2B11D0EAE7E2}" src="https://github.com/user-attachments/assets/03a57c2b-0455-429a-9c44-e2c0e519ef54" />|


---

|📜 Certificates Section|
|Menampilkan daftar sertifikat menggunakan tampilan card layout.|
|<img width="960" height="504" alt="{2B42B6B6-3C4C-4056-84AF-D8C7F4953C08}" src="https://github.com/user-attachments/assets/1884b2cb-3670-4dc6-8943-1b4b13e2a9c7" />|

---

## 💻 Penjelasan Code Setiap Section

### 🧭 Navbar

Navbar digunakan sebagai menu navigasi untuk berpindah antar section pada website seperti Home, About Me, dan Certificates.

Contoh kode:

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
```

Penjelasan:

- `navbar` digunakan untuk membuat menu navigasi
- `navbar-expand-lg` agar navbar responsive
- `bg-primary` memberi warna biru
- Menu Home, About Me, dan Certificates terhubung menggunakan link seperti `#home` dan `#about`

Navbar akan tetap berada di bagian atas website dan memudahkan pengguna berpindah halaman.

---

### 🏠 Home Section

Home Section adalah halaman utama yang berisi perkenalan singkat.

Contoh kode:

```html
<section id="home" class="py-5">
```

Penjelasan:

- `<section id="home">` digunakan sebagai bagian Home
- `container` digunakan agar tampilan rapi
- `row` dan `col-md-6` digunakan untuk membagi tampilan menjadi dua bagian
- Bagian kiri berisi teks perkenalan
- Bagian kanan berisi foto profil

Foto profil dibuat menggunakan:

```html
<img src="Foto Ilyasa.png" class="img-fluid rounded-circle">
```

- `img-fluid` membuat gambar responsive
- `rounded-circle` membuat gambar menjadi bulat

---

### 👨‍💻 About Me Section

About Me Section berisi profil, skill, dan pengalaman.

Contoh kode:

```html
<section id="about" class="py-5 bg-light">
```

Penjelasan:

- Section ini menggunakan `bg-light` agar memiliki warna background abu-abu
- Informasi ditampilkan menggunakan card Bootstrap

Profil dibuat menggunakan card:

```html
<div class="card">
<div class="card-body">
```

Skills dibuat menggunakan progress bar:

```html
<div class="progress">
<div class="progress-bar" style="width: 22%"></div>
```

- `progress-bar` digunakan untuk menampilkan tingkat kemampuan
- Nilai persentase diatur menggunakan `width`

Pengalaman ditampilkan menggunakan list:

```html
<ul>
<li>Anggota INFORSA Departemen Cominfo (2025)</li>
</ul>
```

---

### 📜 Certificates Section

Certificates Section digunakan untuk menampilkan sertifikat yang dimiliki.

Contoh kode:

```html
<section id="certificates" class="py-5">
```

Penjelasan:

- Sertifikat ditampilkan menggunakan card Bootstrap
- Setiap card berisi gambar sertifikat dan keterangan

Contoh card:

```html
<div class="card h-100">
<img src="Sertifikat Cyber Security SC.png" class="card-img-top">
```

- `card` digunakan untuk membuat tampilan kotak
- `card-img-top` digunakan untuk menampilkan gambar di atas card
- `h-100` membuat ukuran card sama tinggi

---

### 🔻 Footer

Footer digunakan sebagai penutup halaman website.

Contoh kode:

```html
<footer class="bg-dark text-white text-center py-3">
```

Penjelasan:

- `bg-dark` memberi warna hitam
- `text-white` memberi warna tulisan putih
- `text-center` membuat tulisan berada di tengah

Footer berisi informasi copyright website.
---

## 🎨 Penjelasan File CSS (style.css)

File **style.css** digunakan untuk mengatur tampilan website agar memiliki tema gelap (dark theme) dengan background hitam dan teks berwarna putih.

---

### Background dan Text

Kode berikut digunakan untuk mengatur tampilan utama website.

```css
body {
    font-family: Arial, sans-serif;
    background-color: #000000;
    color: #ffffff;
}
```

Penjelasan:

- `font-family` mengatur jenis huruf menjadi Arial
- `background-color` memberi warna hitam pada background
- `color` memberi warna putih pada teks

---

### Section

Kode berikut digunakan untuk mengatur ukuran section.

```css
section {
    min-height: 50vh;
    padding-top: 80px;
}
```

Penjelasan:

- `min-height: 50vh` membuat tinggi section minimal setengah layar
- `padding-top` memberi jarak dari atas agar tidak tertutup navbar

---

### Heading dan Paragraf

Kode berikut mengatur warna teks judul dan paragraf.

```css
h1 {
    font-size: 2.5rem;
    color: #ffffff;
}

h2, h4, h5 {
    color: #ffffff;
}

p {
    color: #ffffff;
}
```

Penjelasan:

- Judul dan paragraf dibuat berwarna putih agar terlihat jelas pada background hitam.

---

### Navbar

Kode berikut digunakan untuk mengatur warna navbar.

```css
.bg-primary {
    background-color: #1a1a1a !important;
}
```

Penjelasan:

- Mengubah warna navbar Bootstrap menjadi warna abu gelap.
- `!important` digunakan agar warna Bootstrap tertimpa oleh CSS sendiri.

---

### Card

Kode berikut digunakan untuk mengatur tampilan card.

```css
.card {
    background-color: #1a1a1a;
    border: 1px solid #333;
    color: #ffffff;
}
```

Penjelasan:

- Background card dibuat gelap agar sesuai tema
- Border dibuat abu-abu
- Text dibuat putih

---

### Progress Bar

Kode berikut digunakan untuk mengatur tampilan skill.

```css
.progress {
    background-color: #333;
    height: 20px;
}

.progress-bar {
    background-color: #0d6efd;
}
```

Penjelasan:

- Progress bar digunakan untuk menampilkan skill
- Warna biru diambil dari warna Bootstrap

---

### Footer

Kode berikut digunakan untuk mengatur tampilan footer.

```css
footer {
    background-color: #1a1a1a;
    color: #ffffff;
}
```

Penjelasan:

- Footer dibuat berwarna gelap agar sesuai dengan tema website.

---

### Link

Kode berikut digunakan untuk mengatur warna link.

```css
a {
    color: #0d6efd;
}

a:hover {
    color: #0a58ca;
}
```

Penjelasan:

- Link berwarna biru
- Saat diarahkan mouse warnanya berubah menjadi biru lebih gelap.

---

### List

Kode berikut digunakan untuk mengatur warna tulisan list.

```css
ul li {
    color: #cccccc;
}
```

Penjelasan:

- Warna list dibuat abu-abu agar tidak terlalu terang.

---

### Justify Text

Kode berikut digunakan untuk meratakan teks pada card.

```css
.card-text {
    text-align: justify;
}
```

Penjelasan:

- Teks dibuat rata kiri dan kanan agar terlihat lebih rapi.
---

## 📁 Struktur Project

```
MINPRO 1
│── Foto Ilyasa.png
│── index.html
│── README.md
│── Sertifikat Cyber Security SC.png
│── Sertifikat Kepengurusan INFORSa 2025.jpeg
│── style.css
```

---

## 🚀 Cara Menjalankan Website

1. Clone repository

```
git clone https://github.com/Ilyasa810/Minpro1_PBWebsite_M.Ilyasa_033.git
```

2. Masuk ke folder project

```
cd Minpro1_PBWebsite_M.Ilyasa_033
```

3. Buka file berikut di browser:

```
index.html
```

Website akan langsung tampil di browser.
