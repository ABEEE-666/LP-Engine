# AI RULES
LP Engine v1.0

---

# Purpose

Dokumen ini berisi aturan yang WAJIB dipatuhi oleh AI ketika melakukan perubahan pada project yang menggunakan LP Engine.

Tujuan utama aturan ini adalah menjaga stabilitas, konsistensi, dan kemudahan maintenance.

AI harus mengutamakan perubahan yang aman dan tidak melakukan refactor besar tanpa diminta.

---

# AI Priorities

Urutan prioritas AI ketika melakukan perubahan.

1. Jangan merusak website.
2. Jangan menghapus fitur yang sudah ada.
3. Jangan mengubah struktur tanpa alasan.
4. Jangan mengubah dependency yang digunakan.
5. Lakukan perubahan sekecil mungkin.
6. Pertahankan backward compatibility.

---

# Allowed Actions

AI diperbolehkan:

- Mengubah teks.
- Mengubah gambar.
- Mengubah icon.
- Mengubah warna.
- Mengubah styling.
- Mengubah animasi.
- Menambah Component baru.
- Menambah helper function.
- Mengoptimalkan performa.
- Mengoptimalkan readability.
- Menambahkan komentar.

---

# Restricted Actions

AI tidak boleh:

- Mengubah nama Global Object tanpa alasan.
- Mengubah nama Function yang digunakan oleh Render Engine.
- Mengubah HTML ID yang digunakan oleh JavaScript.
- Menghapus dependency tanpa izin.
- Menghapus section tanpa izin.
- Menghapus komentar penting.
- Mengubah urutan Application Initialization.

---

# Naming Convention

Gunakan camelCase untuk function.

Contoh:

renderHero()

createButton()

createCard()

---

Gunakan UPPER_CASE untuk konstanta global.

Contoh:

CONFIG

DEFAULT_THEME

DEFAULT_OPTIONS

---

Gunakan PascalCase apabila suatu saat project menggunakan class.

Contoh:

HeroSection

CardComponent

ButtonFactory

---

# Comment Standard

Setiap section utama disarankan memiliki komentar yang konsisten.

Contoh:

/****************************************************************

SECTION

<SECTION_NAME>

DESCRIPTION

<SECTION_DESCRIPTION>

SAFE TO EDIT

YES / NO

****************************************************************/

---

# Before Editing

Sebelum melakukan perubahan AI harus:

- Memahami tujuan perubahan.
- Memahami dependency yang digunakan.
- Memahami dampak terhadap bagian lain.
- Memastikan kompatibilitas browser tetap terjaga.

---

# After Editing

Setelah perubahan selesai AI harus memastikan:

- Website tetap berjalan.
- Tidak ada syntax error.
- Tidak ada duplicate ID.
- Tidak ada variable yang hilang.
- Tidak ada function yang rusak.
- Tidak ada dependency yang hilang.

---

# Scope Rules

AI hanya boleh mengubah area yang diminta oleh pengguna.

Jangan:

- Mengubah styling yang tidak diminta.
- Mengubah copywriting yang tidak diminta.
- Menambahkan fitur tanpa persetujuan.
- Melakukan refactor di luar scope.

---

# AI Decision Rules

Jika terdapat beberapa solusi:

1. Pilih solusi yang paling sederhana.
2. Pilih solusi dengan risiko paling kecil.
3. Hindari refactor besar apabila masalah dapat diselesaikan dengan perubahan kecil.
4. Gunakan dependency yang sudah ada sebelum menambahkan dependency baru.

---

# Philosophy

LP Engine dibangun dengan prinsip:

- Konsisten.
- Stabil.
- Mudah dipelihara.
- Mudah dipahami manusia.
- Mudah dipahami AI.

Lebih baik melakukan sepuluh perubahan kecil yang aman daripada satu refactor besar yang berisiko.