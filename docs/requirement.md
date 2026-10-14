# Spesifikasi dan Kebutuhan Perangkat Lunak (SKPL)
**Proyek:** Landing Page UMKM Jasa Cuci Sepatu "KlinShoes"
**Versi Dokumen:** 1.0
**Teknologi:** HTML5, Pure CSS3 (Tanpa Framework, Tanpa JavaScript)

---

## 1. Requirement Analysis (Analisis Kebutuhan)

Tahap ini mengidentifikasi masalah, pengguna sasaran, tujuan, batasan, dan kriteria penerimaan dalam pengembangan website KlinShoes.

### 1.1. Latar Belakang & Tujuan Bisnis
KlinShoes adalah UMKM yang bergerak di bidang jasa perawatan dan pencucian sepatu. Saat ini, promosi hanya mengandalkan *word of mouth* (dari mulut ke mulut) dan media sosial. Tujuan pembuatan *landing page* ini adalah untuk meningkatkan kredibilitas, memberikan informasi harga yang transparan, dan mempercepat proses konversi pelanggan baru melalui satu pintu (WhatsApp).

### 1.2. Pengguna Sasaran (User Persona)
*   **Demografi:** Pria & Wanita, usia 17 - 35 tahun (Mahasiswa, Pekerja Kantoran, Sneakerhead).
*   **Geografi:** Khususnya berdomisili di Depok dan sekitarnya (jangkauan layanan antar-jemput).
*   **Perilaku & Kebutuhan:** Memiliki kesibukan tinggi, tidak punya waktu mencuci sepatu sendiri, mengutamakan kepraktisan, dan butuh bukti hasil cucian sebelum mempercayakan sepatunya. Mereka sering mengakses internet melalui ponsel pintar (*smartphone*).

### 1.3. Kebutuhan Fungsional
Kebutuhan fungsional mendefinisikan interaksi dan fitur spesifik yang harus ada pada sistem:
1.  **Navigasi Halaman:** Sistem harus menyediakan menu navigasi yang dapat diklik untuk melompat (*scroll*) langsung ke bagian spesifik pada halaman yang sama (Beranda, Layanan, Galeri, Kontak).
2.  **Katalog Layanan & Harga:** Sistem harus menampilkan minimal 3 daftar layanan utama beserta deskripsi singkat dan estimasi harganya.
3.  **Galeri Portofolio:** Sistem harus menampilkan komparasi gambar sepatu kotor (sebelum) dan bersih (sesudah) dalam format *grid* atau daftar.
4.  **Integrasi Komunikasi (CTA):** Sistem harus memiliki tombol "Cuci Sekarang" atau "Hubungi Kami" yang menggunakan tautan format `wa.me` dengan pesan otomatis (contoh: *"Halo KlinShoes, saya ingin cuci sepatu..."*).
5.  **Informasi Bisnis:** Sistem harus menampilkan alamat lengkap, jam operasional bengkel, dan tautan ke media sosial (Instagram/TikTok).

### 1.4. Kebutuhan Nonfungsional
Kebutuhan nonfungsional mendefinisikan kualitas, performa, dan batasan teknis sistem:
1.  **Batasan Teknologi:** 
    *   Pengembangan secara eksklusif menggunakan murni **HTML5** dan **CSS3**.
    *   **Dilarang** menggunakan *framework* CSS (seperti Bootstrap, Tailwind, Foundation).
    *   **Dilarang** menggunakan JavaScript (*Vanilla* maupun *library* seperti jQuery).
2.  **Responsivitas & Tata Letak:** 
    *   Desain harus menggunakan pendekatan *Mobile-First*.
    *   Tata letak (*layout*) harus menyesuaikan ukuran layar secara otomatis menggunakan *CSS Media Queries*, *Flexbox*, atau *CSS Grid*.
    *   Konten harus dapat dibaca pada layar ponsel tanpa ada gulir mendatar (*horizontal scroll*).
3.  **Performa:** 
    *   Website harus ringan. Semua aset gambar (*Before-After* dan *Hero image*) harus dikompresi (format WebP atau JPEG yang dioptimasi) agar halaman dimuat di bawah 3 detik pada koneksi 4G.
4.  **Panduan Visual (UI/UX):**
    *   **Tipografi:** Menggunakan Google Fonts *Sans-Serif* agar modern dan mudah dibaca (Rekomendasi: `Poppins` untuk *Heading*, `Open Sans` atau `Inter` untuk *Body Text*).
    *   **Palet Warna:**
        *   *Primary Color* (Aksen & CTA): Biru Laut (`#0077B6`)
        *   *Background Utama*: Putih Bersih (`#FFFFFF`)
        *   *Background Sekunder* (Selang-seling seksi): Abu-abu Terang (`#F0F4F8`)
        *   *Teks Utama*: Hitam Keabuan (`#333333`)
    *   **Interaksi:** Harus ada *hover effect* (perubahan warna/bayangan) pada tombol dan tautan menggunakan CSS `transition` untuk memberikan umpan balik visual kepada pengguna.

### 1.5. Kriteria Penerimaan (Acceptance Criteria)
Website dinyatakan selesai dan memenuhi syarat apabila:
*   [ ] Halaman lolos validasi HTML5 W3C tanpa *error* fatal.
*   [ ] Saat dibuka di layar HP dengan lebar 320px - 480px, tidak ada elemen yang terpotong ke samping.
*   [ ] Tombol navigasi (Beranda, Layanan, dll) berfungsi dan mengarahkan pengguna ke bagian yang tepat di halaman tersebut.
*   [ ] Mengklik tombol CTA WhatsApp langsung membuka aplikasi/web WhatsApp dengan pesan bawaan (*pre-filled message*).
*   [ ] Seluruh tata letak dan gaya dirender murni dari file `.css` eksternal.

---

## 2. Site Structure (Perancangan Struktur Website)

Website dirancang dengan model *Single Page Application* (SPA) / Landing Page. Berikut adalah Peta Konten (Rancangan Informasi per Bagian) dari atas ke bawah:

### Bagian 1: Header & Navigasi (*Navbar*)
*   **Posisi:** Tetap di bagian paling atas layar (*Sticky Header* menggunakan CSS).
*   **Konten Kiri:** Logo "KlinShoes" (Teks atau Gambar).
*   **Konten Kanan (Menu):** Tautan ke `[Layanan]`, `[Keunggulan]`, `[Galeri]`, `[Kontak]`.
*   **Layout Mobile:** Karena tanpa JS, menu di mobile akan ditampilkan berjejer secara rapi (menggunakan Flexbox `flex-wrap` atau ditata di bawah logo).

### Bagian 2: Beranda (*Hero Section*)
*   **Latar Belakang:** Foto estetis proses cuci sepatu atau pola abstrak berwarna abu-abu terang.
*   **Copywriting:** 
    *   *Headline (H1):* "Sepatu Kotor Jadi Seperti Baru Lagi."
    *   *Sub-headline (p):* "Layanan perawatan sepatu profesional di Depok. Cepat, bersih, dan wangi."
*   **CTA Utama:** Tombol besar berwarna biru laut bertuliskan **"Konsultasi & Cuci Sekarang ➔"**.

### Bagian 3: Pengenalan Usaha (*Keunggulan / Why Us*)
*   **Judul Seksi (H2):** "Kenapa Memilih KlinShoes?"
*   **Konten:** Dibagi menjadi 3 kolom (pada Desktop) atau 1 kolom ke bawah (pada Mobile) berisi ikon sederhana (SVG) dan teks:
    1.  *Deep Cleaning:* Membersihkan hingga ke pori-pori bahan tanpa merusak sepatu.
    2.  *Fast Service:* Estimasi selesai dalam 2-3 hari kerja.
    3.  *Free Pickup:* Gratis antar-jemput untuk wilayah Depok (S&K berlaku).

### Bagian 4: Katalog Layanan & Harga (*Services*)
*   **Latar Belakang:** Abu-abu Terang (`#F0F4F8`) untuk membedakan dengan bagian atasnya.
*   **Judul Seksi (H2):** "Layanan & Harga"
*   **Konten (Peta Harga):** Direpresentasikan dalam bentuk *Card* (Kartu).
    *   **Kartu 1:** Fast Clean (Pembersihan luar midsole & upper) – Rp 35.000
    *   **Kartu 2:** Deep Clean (Pembersihan total luar & dalam, insole, tali) – Rp 50.000
    *   **Kartu 3:** Unyellowing (Mengembalikan warna putih sole yang menguning) – Rp 65.000
*   **Aksi tambahan:** Tombol CTA kecil di setiap kartu bertuliskan "Pilih Paket".

### Bagian 5: Galeri Portofolio (*Before - After*)
*   **Judul Seksi (H2):** "Bukti Kualitas Kami"
*   **Konten:** *Grid* (kisi-kisi) foto yang menampilkan minimal 4 pasang foto perbandingan sepatu sebelum dicuci dan sesudah dicuci oleh KlinShoes. Menggunakan CSS Grid untuk menata kolom gambar.

### Bagian 6: Kontak & Lokasi (*Footer*)
*   **Latar Belakang:** Biru Laut (`#0077B6`) dengan teks Putih (`#FFFFFF`).
*   **Kolom 1 (Info):** Alamat lengkap (Misal: Jl. Margonda Raya No. X, Depok), Jam Operasional (Senin-Sabtu, 09.00 - 18.00).
*   **Kolom 2 (Sosial):** Tautan ikon Instagram, TikTok, dan nomor WhatsApp.
*   **Bawah (*Copyright*):** `© 2026 KlinShoes. All rights reserved.`