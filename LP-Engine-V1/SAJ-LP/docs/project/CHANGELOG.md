# CHANGELOG

Semua perubahan pada project SAJ Landing Page dicatat pada dokumen ini.

Dokumen ini mengikuti format kronologis berdasarkan versi Landing Page dan perkembangan LP Engine.

---

# Version 2.0.0

Status

Production

Tanggal

22 Juli 2026

---

## Initial Release

Landing Page resmi Aqiqah Saung Abah Jajat menggunakan LP Engine v1.0.

Fitur utama:

- Single HTML Architecture.
- Config Driven Content.
- Component Based Rendering.
- Responsive Layout.
- Hero Section.
- Features Section.
- Certification Section.
- Package Section.
- Testimonials.
- FAQ.
- Footer.
- WhatsApp CTA.
- CDN Library.
- Vanilla HTML, CSS, dan JavaScript.

---

# Version 2.1.0

Status

Production

Tanggal

22 Juli 2026

---

## LP Engine Phase 3

Pembaruan arsitektur internal untuk meningkatkan keterbacaan kode, maintainability, dan kompatibilitas dengan AI.

### Added

- AI Header diperbarui dengan informasi struktur project.
- ENGINE Object sebagai pusat pengelolaan render.
- Helper Functions baru.
- Component Metadata pada setiap Component.
- Component Registry (`ENGINE.registry`).
- Render Queue (`ENGINE.renderQueue`).
- `runRenderEngine()` dengan Error Handling.

### Changed

- Struktur Components disesuaikan mengikuti standar LP Engine v1.0.
- App Initialization menggunakan Render Engine.
- Render flow dibuat lebih terstruktur.
- Helper `createStars()` digunakan pada renderTestimonials().
- Penomoran section disesuaikan dengan standar LP Engine.

### Fixed

- Konsistensi struktur internal.
- Konsistensi proses render.
- Peningkatan keterbacaan kode.
- Persiapan engine untuk pengembangan berikutnya.

### Impact

- Tidak mengubah tampilan website.
- Tidak mengubah isi konten.
- Tidak mengubah desain.
- Tidak mengubah perilaku pengguna.

Seluruh perubahan merupakan improvement pada arsitektur internal.

---

# Version 2.2.0

Status

Production

Tanggal

22 Juli 2026

---

## Engine Improvement — Phase 3

Peningkatan arsitektur internal LP Engine tanpa mengubah tampilan website.

### Added

- ENGINE global object (400 ENGINE OBJECT).
- Helper Functions layer (500 HELPER FUNCTIONS):
  - createStars(rating) — generate HTML bintang dari angka.
  - createWaLink(number, message) — generate URL WhatsApp.
  - createSectionHeader(title, subtitle, theme) — generate header section standar.
- Component Metadata pada setiap Component (COMPONENT, DESCRIPTION, DEPENDS_ON, SAFE TO EDIT).
- Component Registry — ENGINE.registry.
- Render Queue — ENGINE.renderQueue.
- Render Engine section (700 RENDER ENGINE) — runRenderEngine().
- initLibraries() helper function untuk init library eksternal.
- Error handling pada render engine dan inisialisasi library.

### Changed

- Struktur section index.html: 300 CONFIG → 400 ENGINE → 500 HELPERS → 600 COMPONENTS → 700 RENDER ENGINE → 800 APP INIT.
- App Initialization lebih bersih: hanya memanggil runRenderEngine() dan initLibraries().
- renderTestimonials menggunakan createStars() dari Helper Functions.
- AI Header diperbarui ke Version 1.2.0.

### Impact

- Tidak mengubah tampilan website.
- Tidak mengubah isi konten.
- Backward compatible dengan seluruh Component yang sudah ada.
- Helper Functions siap digunakan pada Component baru di fase berikutnya.

---

# Version 2.3.0

Status

Production

Tanggal

22 Juli 2026

---

## Phase 4 — Item 1: Top Bar Text (Non-floating)

- Menambahkan Top Bar sederhana di atas Navbar dengan warna hijau SAJ (`#003333`).
- Teks pengumuman: `"CLAIM PROMO POTONGAN BULAN INI SEKARANG! PROMO TERBATAS!"`.
- Link default mengarah ke `#hero`.
- Bersifat non-floating (akan hilang saat di-scroll ke bawah dan muncul kembali saat di paling atas).
- Menambahkan `renderTopBar` ke Component Registry & Render Queue.

## Phase 4 — Item 2: Update Card Paket Harga, Toggle, & Inclusions Bar

- Mengintegrasikan seluruh data dari file `listcontent_asset.csv` ke dalam `config.packages`.
- Menambahkan **Gender Toggle Bar** interaktif (Perempuan / Laki-Laki) dengan default `Perempuan`.
- Meng-update 7 Menu Card (Paket Hemat, Reguler, Spesial, Kebuli Basmati, Kebuli Lokal, Hewan Masak, Karkas) dengan gambar asli & promo tag.
- Menambahkan **Tombol Pemilih Jumlah Box** interaktif (e.g. 50, 75, 100 Box) yang secara otomatis memperbarui estimasi total harga & link WhatsApp.
- Menambahkan **Section Bar Ketentuan & Fasilitas Bonus** lengkap dengan icon (Dokumentasi Foto & Video Penyembelihan, Sertifikat Frame, Boneka Domba, Free Plastik Pembungkus, Free Kartu Ucapan, Free Ongkir SEJABODETABEK).
- Penyesuaian tampilan Inclusions: penyederhanaan judul header menjadi bold tunggal, penambahan fasilitas dokumentasi di paling awal, penghapusan icon asterisk pada catatan, serta update teks ketentuan domba betina/upgrade CS.

---

# Next Planned Version

Version

2.3.0

Target

LP Engine Phase 4 — UI Improvement

Status

Planned

Rencana pengembangan mengacu pada ROADMAP.md.