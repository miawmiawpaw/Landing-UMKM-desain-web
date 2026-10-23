# Changelog

Semua perubahan penting pada proyek ini dicatat di dokumen ini.
Format mengikuti Keep a Changelog, penomoran versi mengikuti Semantic Versioning.

## [Unreleased]

### Added
- Aset gambar nyata pada `assets/images/`: `hero.jpg`, `before-1.jpg`, `after-1.jpg`, `before-2.jpg`, `after-2.jpg`.
- Bagian statistik metrik (100+ pasang dirawat, 24 jam pengerjaan, 95% kepuasan) di bawah galeri Before-After.
- Ikon SVG spesifik untuk fitur (deep cleaning, sabun ramah lingkungan, pickup) dan footer (Instagram, TikTok, WhatsApp).
- Tangkapan layar pengujian multi-viewport (Desktop, Tablet, Mobile) pada `docs/screenshots/` dan disematkan ke `docs/testing.md`.

### Removed
- Label/badge seksi kawat (*wireframe badges*: "Bagian 1: Navbar", "Bagian 2: Pembuka", dst) dari HTML dan CSS untuk tampilan produksi bersih.

### Changed
- Nama brand tetap dipertahankan sebagai **KlinShoes**.
- Palet warna diperbarui ke tema earthy green & warm cream sesuai gambar acuan:
  - Hero & Navbar: `#FAF7F0`
  - Konten utama: `#E8F0E4`
  - Aksen kartu: `#FFFFFF`
  - Aksen harga: `#D9825B` (Terracotta)
  - Tombol & Footer: `#4F7F5B` (Forest Green)
  - Teks: `#1F2D24`
- Tampilan responsif mobile disesuaikan persis dengan gambar acuan:
  - Navbar: Logo di atas, menu tautan berjejer horizontal di bawah logo.
  - Tombol hero CTA "Cuci Sekarang": Lebar penuh (*full-width*) pada layar ponsel.
  - Galeri Before-After: Tetap 2 kolom sejajar (*side-by-side*) pada mobile.
  - Kartu statistik metrik: Ditata 3 kolom berdampingan secara kompak pada mobile.
  - Footer: Tetap 2 kolom berdampingan (*Alamat & jam buka* kiri, *Hubungi kami* kanan).
- Typo direktori `assests/` diperbaiki menjadi `assets/`.
- Ditambahkan `scroll-padding-top: 100px` agar sticky header tidak menutupi judul seksi saat anchor link diklik.
- Dokumentasi spesifikasi `docs/requirement.md` disinkronkan: urutan navigasi resmi menjadi Keunggulan, Layanan, Galeri, Kontak, dan palet warna resmi diperbarui ke Earth Green & Terracotta.
- Seluruh hasil pengujian fungsional dan nonfungsional (responsivitas 320px–1200px, aset, CTA, CSS) dieksekusi dan dicatat di `docs/testing.md` dengan status Lulus.
- Dokumentasi utama `README.md` dirapikan secara lengkap: deskripsi proyek, preview gambar, daftar fitur, palet warna, struktur direktori, cara menjalankan server, dan info kelompok.

## [0.1.0] - 2026-10-14

### Added
- Dokumen spesifikasi kebutuhan perangkat lunak `docs/requirement.md` (versi 1.0).
- Struktur awal proyek: `index.html`, `css/style.css`.
- Berkas `README.md`.
- Inisialisasi repositori Git dan penghubungan ke remote GitHub.
