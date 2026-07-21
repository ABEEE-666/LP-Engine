# LP ENGINE
Version 1.0

---

# Purpose

LP Engine adalah standar arsitektur untuk membangun Landing Page menggunakan pendekatan Single HTML.

Engine ini dirancang agar mudah dipahami oleh manusia maupun AI, tanpa memerlukan proses build atau framework JavaScript.

LP Engine bukan template desain, melainkan standar struktur project dan alur kerja.

---

# Goals

LP Engine memiliki tujuan utama:

- Mudah dipelihara.
- Mudah dikembangkan.
- Mudah dipahami AI.
- Mudah dipahami developer.
- Mudah dipindahkan ke hosting mana pun.
- Cukup upload satu file HTML.

---

# Core Principles

LP Engine dibangun berdasarkan prinsip berikut.

## Single HTML

Seluruh Landing Page berada dalam satu file HTML.

Tidak memerlukan bundler maupun build process.

---

## Config Driven

Seluruh data website berasal dari CONFIG.

Perubahan konten sebisa mungkin dilakukan melalui CONFIG tanpa mengubah Component.

---

## Component Based

Setiap bagian website dibuat sebagai Component yang berdiri sendiri.

Component bertugas menghasilkan tampilan berdasarkan data dari CONFIG.

---

## Render Based

Seluruh Component disusun oleh Render Engine menjadi satu halaman utuh.

Render Engine hanya mengatur urutan render dan tidak menyimpan data.

---

## AI Friendly

Struktur project dibuat konsisten agar mudah dipahami oleh AI.

Setiap project yang menggunakan LP Engine mengikuti pola yang sama.

---

# Standard Structure

Urutan standar di dalam file HTML adalah:

```
000 AI HEADER

100 HTML

200 External Libraries

300 CSS

400 CONFIG

500 Helper Functions

600 Components

700 Render Engine

800 Library Initialization

900 Application Initialization
```

---

# Responsibilities

## CONFIG

Menyimpan seluruh data website.

---

## Helper Functions

Berisi fungsi-fungsi umum yang dapat digunakan oleh Component.

---

## Components

Menghasilkan tampilan website berdasarkan CONFIG.

---

## Render Engine

Menyusun seluruh Component menjadi satu halaman.

---

## Library Initialization

Mengaktifkan seluruh library eksternal.

---

## Application Initialization

Menjalankan aplikasi dan memulai proses render.

---

# Development Philosophy

LP Engine mengutamakan:

- Konsistensi.
- Readability.
- Maintainability.
- Modularitas.
- Risiko perubahan yang kecil.

Perubahan kecil yang aman selalu lebih baik daripada refactor besar yang tidak diperlukan.

---

# Scope

LP Engine hanya mengatur:

- Struktur Landing Page.
- Arsitektur kode.
- Workflow rendering.
- Standar dokumentasi.
- Standar pengembangan.

LP Engine tidak mengatur:

- Desain visual.
- Identitas brand.
- Copywriting.
- Warna.
- Asset.
- Isi konten.

Hal tersebut menjadi tanggung jawab masing-masing project.

---

# Compatibility

LP Engine dapat digunakan untuk berbagai jenis Landing Page, seperti:

- Company Profile
- Travel
- Aqiqah
- Restaurant
- Product Launch
- Event
- UMKM
- Portfolio

Tanpa mengubah arsitektur dasar.

---

# Version

LP Engine

v1.0