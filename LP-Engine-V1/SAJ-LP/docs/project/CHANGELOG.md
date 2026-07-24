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
  - formatRupiah(val) — format angka ke format Rupiah (Rp X.XXX.XXX).
- Component Metadata pada setiap Component (COMPONENT, DESCRIPTION, DEPENDS_ON, SAFE TO EDIT).
- Component Registry — ENGINE.registry.
- Render Queue — ENGINE.renderQueue.
- Render Engine section (700 RENDER ENGINE) — runRenderEngine().
- initLibraries() helper function untuk init library eksternal.
- Error handling pada render engine dan inisialisasi library.
- Library CDN baru: CountUp.js (animasi angka statistik Hero) dan Typed.js (animasi teks rating).

### Changed

- Struktur section index.html: 100 HTML → 200 CSS → 300 CONFIG → 400 ENGINE → 500 HELPERS → 600 COMPONENTS → 700 RENDER ENGINE → 800 APP INIT.
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

# Version 2.4.0

Status

Production

Tanggal

22 Juli 2026

---

## Phase 4 — Item 3: Logo Fill Loading Screen Animation

- Menambahkan **Logo Fill Loading Screen Animation** saat halaman pertama kali dimuat.
- Menambahkan konfigurasi `config.loadingScreen` untuk mengontrol status & durasi tayang loading screen.
- Menggunakan background warna hijau SAJ (`#003333`) dengan efek animasi pulsa emas (`pulseGlow`) pada logo SVG dan progress fill bar (`logoFill`).
- Menambahkan transisi `fade-out` yang halus sebelum elemen dihapus dari DOM setelah inisialisasi aplikasi selesai.

---

# Version 2.5.0

Status

Production

Tanggal

22 Juli 2026

---

## Phase 4 — Item 4: Mobile Spacing & CTA Polish Optimization

- Menambahkan `@media (max-width: 768px)` pada CSS `index.html` untuk mengoptimalkan tampilan seluler.
- Mengurangi *vertical section padding* pada mobile dari `5rem` menjadi `2.5rem` agar konten tidak terlalu renggang dan mudah di-scroll.
- Menyesuaikan ukuran *typography* (`h1`, `h2`, `.lead`, `.top-bar-text`) agar responsif & tidak terpotong di layar HP.
- Mengoptimalkan ukuran tombol gender toggle & pemilih box agar pas dan mudah ditekan oleh ibu jari (*thumb-friendly*).
- Menambahkan animasi *pulse* bergelombang (`waPulse`) pada tombol Floating WhatsApp CTA untuk meningkatkan visibilitas & rasio konversi pada mobile.

---

# Version 2.6.0

Status

Production

Tanggal

22 Juli 2026

---

## Phase 4 — Item 5: Testimonials Focus Mode

Pembaruan besar pada Section Testimoni — dari slider statis menjadi sistem interaktif dua-panel dengan Focus Mode Hero Card.

### Added

- **Testimonials Focus Mode** — arsitektur dua-panel baru:
  - **Preview Slider** (Swiper): menampilkan kartu-kartu testimoni ringkas yang bisa di-scroll.
  - **Hero Card** (Focus Mode): muncul saat pengguna mengklik salah satu kartu, menampilkan highlight quote testimoni yang dipilih.
- State management testimoni (`window._testi`) dengan properti `activeIndex` dan `isExpanded`.
- Handler interaktif:
  - `selectTestimonial(index)` — klik kartu untuk membuka/menutup Hero Card.
  - `toggleTestiReview(expand)` — toggle antara mode highlight dan pesan ulasan utuh.
  - `_renderHeroContent(withFade)` — internal renderer Hero Card dengan animasi fade.
- Tombol **"Baca Review Lengkap"** di Hero Card untuk menampilkan teks ulasan asli secara penuh.
- Tombol **"Tutup"** untuk menutup tampilan pesan utuh dan kembali ke mode highlight.
- Field `highlightText` pada setiap data testimoni di `config.testimonials.items` — teks singkat ringkasan kuotasi yang ditampilkan di Hero Card dan Preview Slider.
- CSS baru untuk komponen Focus Mode:
  - `.testi-card`, `.testi-card-stars`, `.testi-card-text`, `.testi-card-footer`, `.testi-card-avatar`, `.testi-card-name`, `.testi-card-location`.
  - `.testi-hero-wrapper` dengan animasi `max-height` & `opacity`.
  - `.testi-hero-card`, `.testi-hero-body`, `.testi-hero-stars`, `.testi-hero-text`, `.testi-hero-name`, `.testi-hero-location`.
  - `.badge-google-review`, `.btn-read-review`, `.btn-close-review`.
  - State `.is-active` pada Preview Card dan `.is-visible` pada Hero Wrapper.
  - `.testi-hero-body.is-fading` untuk animasi konten saat beralih testimoni.
- Foto testimoni pelanggan (`image` field) tersedia di data config (disiapkan untuk pengembangan berikutnya).
- Pesan petunjuk di bawah section header: *"Klik kartu testimoni untuk melihat detail review"*.
- Mobile responsive CSS untuk Hero Card (`padding`, `border-width` pada `max-width: 768px`).

### Changed

- Struktur `renderTestimonials` sepenuhnya direfactor dari slider sederhana menjadi sistem dua-panel interaktif.
- Data testimoni diperluas: setiap item kini memiliki `name`, `location`, `rating`, `text`, `highlightText`, dan `image`.
- Tampilan Preview Card menggunakan teks `highlightText` yang dipotong maksimal 80 karakter.
- Hero Card default menampilkan testimoni pertama (index 0) sebagai konten awal.
- Swiper breakpoints dioptimalkan untuk menampilkan 1 / 2 / 3 / 4 slide sesuai lebar layar.

### Impact

- Meningkatkan engagement pengguna pada section testimoni.
- Pengguna dapat membaca ulasan asli tanpa meninggalkan halaman.
- Tampilan lebih premium dan interaktif.

---

## Phase 4 — Item 6: FAQ CTA Card

- Menambahkan **CTA Card "Masih ada pertanyaan lain?"** di bawah accordion FAQ.
- CTA mengarahkan pengguna ke WhatsApp dengan pesan pre-filled: *"Halo Kak SAJ, saya ingin konsultasi seputar aqiqah 🙏"*.
- Desain card menggunakan gradient hijau muda, border kuning SAJ, efek dekoratif bubble, dan ikon WhatsApp.
- Tombol hover effect mengubah warna dari hijau ke kuning dengan animasi `translateY`.

---

# Version 2.7.0

Status

Production

Tanggal

24 Juli 2026

---

## LP Engine Phase 5 — Dedicated Promo Landing Page Engine (`promopdjuli26.html`)

Pembuatan Landing Page khusus Sales/Promo Campaign terpisah (`promopdjuli26.html`) berbasis arsitektur LP Engine v1.0 yang berfokus pada konversi penawaran spesial (Payday Sale Juli 2026).

### Added

- **Single Page Promo Architecture (`promopdjuli26.html`)**: Halaman landing page independen untuk campaign promo diskon hingga Rp 600.000.
- **Campaign Configuration Object (`config.campaign`)**:
  - Pengaturan kode promo, badge campaign (`⚡ PROMO SPESIAL PAYDAY JULI 2026 ⚡`), title, subtitle, flyer promo image, periode promo, serta custom WhatsApp pre-filled message (`PROMO-SAJ-PAYDAYSALE7`).
- **Komponen Dedicated Promo (`600 COMPONENTS`)**:
  - `renderTopBar`: Announcement top bar khusus klaim promo potongan harga.
  - `renderPromoHero`: Hero section dengan dual CTA, badge diskon, countdown timer/periode promo, dan flyer banner.
  - `renderPromoBenefits`: Grid 4 benefit utama promo (Bonus Souvenir, Free Dokumentasi, Gratis Ongkir, Olahan Lezat).
  - `renderPromoPackages`: Grid 4 paket promo spesifik (Hemat & Spesial untuk Perempuan & Laki-laki) dengan informasi *normal price*, *promo price*, *savings*, serta komparasi hemat.
  - `renderPromoClaimSteps`: 3 langkah mudah klaim promo.
  - `renderPromoTerms`: Accordion Syarat & Ketentuan klaim promo.
  - `renderPromoClosingCTA`: Call-to-action penutup berorientasi urgensi stok/kuota promo.
  - `renderBottomBar`: Sticky bottom CTA bar khusus mobile untuk kemudahan klaim via WhatsApp.
  - `renderPromoFooter`: Footer ringkas promo beserta Floating WhatsApp CTA.
- **Interaktivitas & Visual Polish**:
  - **Parallax Scroll Effect**: Efek parallax gerakan halus flyer promo (`heroParallaxFlyer`) saat scroll di antara Hero & Benefit.
  - Integration `AOS` animation & Loading Screen Animation dengan branding SAJ.

---

# Next Planned Version

Version

3.0.0

Target

LP Engine Phase 6 — Content Management & Multi-Brand Expansion (Qurban Berkah)

Status

Planned

Rencana pengembangan mengacu pada ROADMAP.md.