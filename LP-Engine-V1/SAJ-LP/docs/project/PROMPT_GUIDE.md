# PROMPT GUIDE
LP Engine v1.0

Version : 1.0

---

# Tujuan

Dokumen ini menjelaskan bagaimana AI harus memahami, menganalisis, dan melakukan perubahan pada project.

Dokumen ini bukan kumpulan prompt.

Dokumen ini adalah panduan workflow AI.

---

# Sebelum Memulai

Sebelum mengubah apapun, AI WAJIB membaca dokumen berikut secara berurutan.

1.

README.md

↓

2.

CONTEXT.md

↓

3.

LP_ENGINE_v1.md

↓

4.

AI_RULES.md

↓

5.

PROJECT_STRUCTURE.md

↓

6.

ROADMAP.md

↓

7.

BRAND_GUIDE.md

↓

8.

CHANGELOG.md

Baru setelah seluruh konteks dipahami, AI boleh membuka:

index_v2.html

---

# AI Workflow

Ketika menerima tugas, AI harus melalui langkah berikut.

STEP 1

Pahami permintaan pengguna.

↓

STEP 2

Identifikasi area yang akan diubah.

↓

STEP 3

Cari dokumentasi yang relevan.

↓

STEP 4

Analisis dampak perubahan.

↓

STEP 5

Lakukan perubahan sekecil mungkin.

↓

STEP 6

Pastikan website tetap berjalan.

---

# Mapping Task

Jika pengguna meminta:

Mengubah teks

↓

Edit CONFIG

---

Mengubah gambar

↓

Edit CONFIG

---

Mengubah icon

↓

Edit CONFIG

---

Mengubah warna

↓

CSS

---

Mengubah layout

↓

Component

---

Menambah section

↓

Buat Component baru

↓

Tambahkan ke Render Engine

---

Mengubah animasi

↓

Library Initialization

---

Optimasi performa

↓

CSS

↓

JavaScript

↓

Assets

---

Menambah library

↓

Analisis dependency

↓

Pastikan kompatibel

---

# Editing Rules

Selalu lakukan:

- Perubahan sekecil mungkin.
- Pertahankan struktur project.
- Pertahankan nama object.
- Pertahankan kompatibilitas browser.
- Pertahankan filosofi Single HTML.

Jangan melakukan refactor besar tanpa diminta.

---

# Safe Edit Area

AI bebas mengubah:

- CONFIG
- Isi Component
- CSS
- Animasi
- Copywriting
- Asset

---

# Sensitive Area

AI harus berhati-hati ketika mengubah:

- Render Engine
- Initialization
- External Library
- HTML ID
- JavaScript Event
- Global Object

---

# Saat Menambah Fitur Baru

Urutan yang disarankan:

1.

Update ROADMAP jika fitur merupakan pengembangan baru.

↓

2.

Tambahkan Component.

↓

3.

Tambahkan Config apabila diperlukan.

↓

4.

Daftarkan ke Render Engine.

↓

5.

Update CHANGELOG.

---

# Saat Memperbaiki Bug

Urutan yang disarankan:

1.

Cari penyebab.

↓

2.

Perbaiki akar masalah.

↓

3.

Jangan mengubah bagian lain tanpa alasan.

↓

4.

Catat pada CHANGELOG.

---

# Saat Mengoptimasi Kode

Prioritas:

1.

Readability

↓

2.

Maintainability

↓

3.

Performance

↓

4.

Optimization

Kode yang mudah dipahami lebih penting daripada kode yang terlalu pintar.

---

# AI Decision Rules

Jika terdapat beberapa solusi:

Pilih solusi yang:

- Paling sederhana.
- Paling stabil.
- Paling mudah dipelihara.
- Paling sedikit mengubah kode.

---

# AI Checklist

Sebelum menyelesaikan pekerjaan, AI harus memastikan:

✓ Website tetap berjalan.

✓ Tidak ada syntax error.

✓ Tidak ada duplicate ID.

✓ Tidak ada function yang hilang.

✓ Tidak ada object yang berubah nama.

✓ Tidak ada library yang rusak.

✓ Responsive tetap bekerja.

✓ Tidak mengubah perilaku yang tidak diminta.

---

# Communication Style

Ketika memberikan rekomendasi:

- Jelaskan alasan perubahan.
- Sebutkan area yang diubah.
- Jelaskan dampaknya.
- Hindari perubahan yang tidak diminta.
- Jangan menambahkan fitur tanpa persetujuan pengguna.

---

# Philosophy

LP Engine dibuat agar:

- Mudah dipahami manusia.
- Mudah dipahami AI.
- Mudah dikembangkan.
- Mudah dipelihara.

Setiap perubahan harus menjaga tujuan tersebut.

Lebih baik melakukan sepuluh perubahan kecil yang aman daripada satu refactor besar yang berisiko.

LP Engine bukan hanya sekumpulan file HTML, tetapi sebuah standar kerja yang konsisten untuk developer dan AI.