# PROJECT STRUCTURE
LP Engine v1.0

---

# Purpose

Dokumen ini menjelaskan struktur standar yang digunakan oleh LP Engine v1.0.

Dokumen ini bersifat universal dan berlaku untuk seluruh project yang menggunakan LP Engine.

Dokumen ini tidak menjelaskan implementasi brand tertentu.

---

# Architecture

LP Engine menggunakan arsitektur:

- Single HTML
- Config Driven
- Component Based
- Vanilla HTML
- Vanilla CSS
- Vanilla JavaScript
- AI Friendly

Seluruh project yang menggunakan LP Engine mengikuti arsitektur ini.

---

# Standard Project Structure

```
PROJECT/

README.md

CONTEXT.md

index.html

docs/

├── engine/
│   ├── LP_ENGINE_v1.md
│   ├── AI_RULES.md
│   └── PROJECT_STRUCTURE.md
│
└── project/
    ├── BRAND_GUIDE.md
    ├── CHANGELOG.md
    ├── PROMPT_GUIDE.md
    └── ROADMAP.md
```

---

# File Responsibilities

## README.md

Entry point project.

Menjelaskan project secara umum dan mengarahkan AI membaca dokumentasi.

---

## CONTEXT.md

Menjelaskan tujuan bisnis, filosofi, target pengguna, serta konteks project.

---

## index.html

Merupakan file utama Landing Page.

Berisi:

- HTML
- CSS
- JavaScript
- CONFIG
- Components
- Render Engine

Deployment cukup menggunakan satu file ini.

---

# Engine Documentation

Folder:

docs/engine/

Berisi dokumentasi yang berlaku untuk seluruh project.

File pada folder ini tidak bergantung pada brand tertentu.

---

LP_ENGINE_v1.md

↓

Menjelaskan konsep LP Engine.

---

AI_RULES.md

↓

Menjelaskan aturan AI saat bekerja.

---

PROJECT_STRUCTURE.md

↓

Menjelaskan struktur project dan hubungan antar file.

---

# Project Documentation

Folder:

docs/project/

Berisi dokumentasi yang hanya berlaku untuk satu project.

Isi dokumentasi dapat berbeda pada setiap brand.

---

BRAND_GUIDE.md

↓

Identitas visual dan karakter brand.

---

ROADMAP.md

↓

Rencana pengembangan project.

---

CHANGELOG.md

↓

Riwayat perubahan project.

---

PROMPT_GUIDE.md

↓

Workflow AI khusus untuk project tersebut.

---

# index.html Structure

LP Engine menggunakan struktur standar berikut.

```
AI HEADER

↓

HTML

↓

External Libraries

↓

CSS

↓

CONFIG

↓

Components

↓

Render Engine

↓

Library Initialization

↓

Application Initialization
```

Seluruh Landing Page mengikuti urutan ini.

---

# CONFIG

CONFIG merupakan sumber utama seluruh data Landing Page.

Semua konten website berasal dari CONFIG.

Contoh data yang biasanya berada di CONFIG:

- Brand Information
- Hero
- Sections
- Navigation
- CTA
- Footer
- Assets
- Contact Information

Struktur isi CONFIG dapat berbeda pada setiap project.

---

# Components

Component merupakan kumpulan function yang bertugas menghasilkan tampilan website.

Contoh:

renderNavbar()

renderHero()

renderSection()

renderFooter()

Nama Component dapat berbeda sesuai kebutuhan project.

---

# Render Engine

Render Engine bertugas menyusun seluruh Component menjadi satu halaman.

Render Engine tidak menyimpan data.

Render Engine hanya mengatur urutan render.

---

# Library Initialization

Bagian ini digunakan untuk mengaktifkan library eksternal.

Contoh:

- AOS
- Swiper
- CountUp
- Typed.js

Library yang digunakan dapat berbeda pada setiap project.

---

# Application Initialization

Merupakan titik awal website dijalankan.

Urutan standar:

Application Start

↓

Render Components

↓

Initialize Libraries

↓

Website Ready

---

# Safe Edit Area

Area yang aman untuk diedit:

- CONFIG
- CSS
- Component
- Copywriting
- Asset
- Animation

---

# Sensitive Area

Perubahan pada area berikut harus dilakukan dengan hati-hati:

- Render Engine
- Initialization
- Global Object
- External Library
- HTML ID
- Function Name

---

# Maintenance Philosophy

LP Engine mengutamakan:

- Konsistensi.
- Kemudahan pemeliharaan.
- Kemudahan pengembangan.
- Kemudahan dipahami AI.
- Perubahan sekecil mungkin.
- Risiko sekecil mungkin.

Lebih baik melakukan perubahan kecil yang aman daripada refactor besar yang tidak diperlukan.

---

# Compatibility

LP Engine dirancang agar dapat digunakan untuk berbagai jenis Landing Page, seperti:

- Travel
- Aqiqah
- Restaurant
- UMKM
- Company Profile
- Event
- Product Launch
- Portfolio

Selama menggunakan arsitektur LP Engine, struktur project tetap konsisten.

---

# Version

LP Engine

v1.0