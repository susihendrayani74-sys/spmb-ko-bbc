Penjelasan Detail Struktur dan Coding Landing Page

Website ini adalah landing page penerimaan siswa baru untuk SMK Budi Bakti Ciwidey yang dibuat menggunakan:

HTML → struktur halaman
CSS → desain/tampilan
TailwindCSS CDN → utility styling tambahan
SVG → ilustrasi hero modern
Google Fonts → font elegan dan modern


Website ini memakai konsep modern:

Full responsive
Animasi halus
Warna profesional
Landing page marketing sekolah
Fokus pada konversi pendaftaran



---

1. Struktur Proyek

Struktur proyek paling ideal untuk coding ini:

smk-budi-bakti/
│
├── index.html
│
├── assets/
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   └── script.js
│   │
│   ├── images/
│   │   ├── logo.png
│   │   ├── hero.png
│   │   └── background.jpg
│   │
│   └── icons/
│       └── icon.svg
│
└── README.md


---

2. Penjelasan Bagian HEAD

<!doctype html>
<html lang="id">

Fungsi

Menentukan:

Dokumen menggunakan HTML5
Bahasa website adalah Indonesia



---

<meta charset="UTF-8" />

Fungsi

Mengatur encoding karakter UTF-8 supaya:

Huruf Indonesia aman
Emoji tampil
Simbol tidak rusak



---

<meta name="viewport" content="width=device-width, initial-scale=1.0" />

Fungsi

Membuat website responsive di HP.

Tanpa ini:

Tampilan mobile rusa
Zoom otomatis
Layout berantakan



---

<title>SMK Budi Bakti Ciwidey - Penerimaan Siswa Baru 2025/2026</title>

Fungsi

Judul website pada:

Tab browser
Hasil Google
Bookmark



---

3. Import TailwindCSS

<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>

Fungsi

Mengambil framework TailwindCSS dari CDN.

Kegunaan Tailwind

Mempermudah:

Flexbox
Grid
Responsive
Spacing
Layout modern

Walaupun di coding ini lebih dominan memakai CSS manual.


---

4. Import Google Fonts

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display...

Font yang dipakai

Playfair Display

Dipakai untuk:

Judul besar
Headline
Memberi kesan premium


DM Sans

Dipakai untuk:

Isi teks
Body text
UI modern



---

5. CSS Root Variables

:root {
  --navy: #0B1A3E;
  --blue: #1A4DB5;
  --green: #50C878;
}

Fungsi

Membuat variabel warna global.
Keuntungan

Kalau ingin ganti tema:

cukup ubah di satu tempat


Contoh:

background: var(--navy);
Lebih rapi daripada:
background: #0B1A3E;


---

6. Reset CSS

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

Fungsi
Menghilangkan style bawaan browser.
box-sizing: border-box

Agar:

padding tidak menambah ukuran elemen
layout lebih stabil



---

7. Smooth Scroll

html {
  scroll-behavior: smooth;
}

Fungsi

Saat klik menu:

scroll jadi halus
lebih modern



---

8. Body Styling

body {
  font-family: 'DM Sans', sans-serif;
  background: var(--light);
}

Fungsi

Mengatur:

font utama
warna background
warna teks default



---

9. Navbar

<nav>

Navbar dibuat:

fixed
transparan blur
selalu muncul di atas



---

Penjelasan CSS Navbar

position: fixed;
top: 0;
z-index: 999;

Fungsi

Navbar:

tetap di atas saat scroll
tidak tertutup elemen lain



---

backdrop-filter: blur(12px);

Fungsi

Membuat efek:

glassmorphism
blur modern



---

10. Hero Section

<section id="hero">

Ini bagian paling penting.

Tujuan Hero

Membuat pengunjung:

tertarik
percaya
ingin daftar



---

11. Hero Layout

display:flex;
justify-content:space-between;

Fungsi

Membagi:

kiri = teks
kanan = ilustrasi SVG



---

12. Hero Badge

<div class="hero-badge">

Fungsi

Label kecil:

memberi highlight informasi penting


Contoh:

“Penerimaan Siswa Baru 2025/2026”



---

13. Hero Headline

<h1 class="hero-headline">

Fungsi

Judul utama marketing.

Tujuan psikologis:

menarik perhatian
meningkatkan rasa percay
memberi motivasi



---

14. Hero CTA Buttons

<a class="btn-primary">

CTA = Call To Action.

Fungsi

Mengajak user:

daftar
melihat jurusan



---

Primary Button

background: var(--green);

Hijau dipakai karena:

identik sukses
positif
action



---

Hover Effect

transform: translateY(-3px);

Fungsi

Saat hover:

tombol naik sedikit
terasa interaktif



---

15. Hero Stats

<div class="hero-stats">

Fungsi

Menampilkan social proof:

98% kerja

akreditasi A

alumni


Tujuan:

Meningkatkan kepercayaan.


---

16. SVG Illustration

<svg viewBox="0 0 420 400">

Fungsi

Ilustrasi custom modern.
Kenapa SVG bagus?
ringan
tidak pecah
scalable
animasi mudah



---

17. Floating Animation

@keyframes floatHero

Fungsi

Membuat ilustrasi:

bergerak naik turun
terlihat hidup



---

18. Problem Section

<section id="problem">

Fungsi

Strategi marketing: menunjukkan masalah user dulu.


---

19. Problem Cards

<div class="problem-card">

Isi

Masalah calon siswa:

bingung jurusan
takut salah sekolah



---

Warna Merah

background: #FFF5F5;
border-left: 4px solid #FF6B6B;

Fungsi

Merah memberi kesan:

warning
masalah
perhatian



---

20. Solution Box

<div class="solution-box">

Fungsi

Menawarkan solusi dari masalah.

Teknik marketing:

Problem → Solution


---

21. Programs Section

<section id="programs">

Fungsi

Menampilkan jurusan/program keahlian.


---

22. CSS Grid

grid-template-columns:
repeat(auto-fit, minmax(280px, 1fr));

Fungsi

Responsive otomatis.

Hasil:

Desktop → banyak kolom
Mobile → turun jadi 1 kolom



---

23. Program Card Hover

transform: translateY(-6px);

Fungsi

Card naik saat hover.

Memberi efek:

premium
interaktif



---

24. Proof Section

<section id="proof">

Fungsi

Social proof section.

Berisi:

statistik
testimoni



---

25. Testimonials

<div class="testimonial">

Fungsi

Meningkatkan kepercayaan calon siswa.
Karena: orang lebih percaya pengalaman alumni.


---

26. CTA Form Section

<section id="cta">

Fungsi

Bagian paling penting untuk konversi.

Tujuan: membuat user daftar.


---

27. Form Input

.form-group input

Fungsi

Styling form modern:

rounded
clean
fokus biru



---

28. Focus Effect

border-color: var(--blue);

Fungsi

Saat diklik:

input berubah biru
user tahu field aktif



---

29. Button Submit

.btn-submit

Fungsi

Tombol kirim form.

Menggunakan:

gradient
shadow
hover animation


Supaya lebih menarik.


---

30. Footer

<footer>

Fungsi

Penutup website.

Biasanya berisi:

copyright
alamat
kontak



---

31. Alert Overlay

.alert-overlay

Fungsi

Popup sukses.

Contoh: “Pendaftaran Berhasil”


---

32. Responsive Design

@media (max-width: 768px)

Fungsi

Mengatur tampilan HP.


---

Contoh

.problem-grid {
  grid-template-columns: 1fr;
}

Desktop:

2 kolom


Mobile:

1 kolom



---

33. Kenapa Website Ini Terlihat Modern?

Karena memakai:

Gradient
Blur effect
Floating animation
Rounded corner
Shadow lembut
Layout whitespace luas
Typography premium
SVG illustration
Glassmorphism



---

34. Alur Landing Page

Struktur marketing website ini:

Navbar
↓
Hero (menarik perhatian)
↓
Problem (masalah user)
↓
Solution
↓
Programs
↓
Proof/Testimoni
↓
CTA Form
↓
Footer

Ini disebut:

Landing Page Funnel

Tujuannya: mengubah pengunjung menjadi pendaftar.


---

35. Kelebihan Coding Ini

UI/UX

Modern
Clean
Responsive
Professional


Performance
Ringan
SVG lebih cepat
Tidak banyak library


Marketing

Ada CTA
Ada social proof
Ada problem solving


Responsive

Cocok desktop & mobile



---

36. Kekurangan Coding Ini

Belum Ada Backend

Form belum menyimpan data.


---

Belum Ada Database

Belum terhubung MySQL/Firebase.


---

Belum Ada Validasi

Input masih bisa kosong.


---

Belum Ada Security

Belum aman dari spam.


---

37. Pengembangan Selanjutnya

Website ini bisa dikembangkan menjadi:

Sistem PPDB Lengkap

Fitur:

login siswa

upload berkas

pembayaran

dashboard admin



---

Backend yang Bisa Dipakai

Beberapa pilihan:

PHP + MySQL
Laravel
Node.js
Firebase
Supabase



---

38. Kesimpulan

Coding ini adalah:

Landing page sekolah modern dengan konsep UI premium.

Menggunakan:

HTML5
CSS3
SVG animation
Responsive design
Marketing funnel


Tujuan utamanya:

menarik calon siswa
meningkatkan kepercayaan
meningkatkan pendaftaran PPDB sekolah.
