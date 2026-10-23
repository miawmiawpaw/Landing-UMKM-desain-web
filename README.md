# KlinShoes - Landing Page UMKM Jasa Cuci Sepatu

> Proyek Desain Web: Landing Page UMKM responsif berbasis murni **HTML5** dan **CSS3** (tanpa framework, tanpa JavaScript).

---

## Tentang Proyek

**KlinShoes** adalah *landing page* promosi untuk usaha mikro, kecil, dan menengah (UMKM) jasa perawatan dan cuci sepatu di wilayah Depok. Website dirancang menggunakan pendekatan *Mobile-First*, mengutamakan kemudahan navigasi, transparansi harga, bukti portofolio *Before-After*, dan konversi pemesanan cepat via WhatsApp.

---

## Preview Tampilan

| Desktop (1200px) | Mobile (390px) |
|:---:|:---:|
| <img src="docs/screenshots/desktop-view.png" width="450" alt="Tampilan Desktop KlinShoes"> | <img src="docs/screenshots/mobile-view.png" width="180" alt="Tampilan Mobile KlinShoes"> |

*Screenshot lengkap pengujian resolusi dapat dilihat di [`docs/testing.md`](docs/testing.md).*

---

## Fitur Utama

- **Mobile-First & Responsif:** Tata letak fleksibel beradaptasi mulus dari ponsel pintar (320px) hingga monitor desktop (1200px+) menggunakan CSS Grid & Flexbox.
- **Sticky Header Navigation:** Navigasi tetap melayang di atas layar dengan *smooth scroll* dan `scroll-padding-top` yang presisi.
- **Katalog Layanan & Harga Transparan:** Kartu paket Fast Clean, Deep Clean, dan Unyellowing dengan harga aksen terracotta.
- **Portofolio Galeri Before-After:** Tampilan perbandingan hasil cucian sepatu kotor dan bersih dalam grid 2 baris.
- **Ringkasan Metrik Statistik:** 3 indikator performa usaha (pasang dirawat, waktu pengerjaan, tingkat kepuasan).
- **Integrasi Direct WhatsApp CTA:** Tombol pemesanan dengan tautan `wa.me` dan teks pesan otomatis (*pre-filled message*).
- **Pure Native Stack:** 100% bebas ketergantungan *library/framework* pihak ketiga dan bebas JavaScript.

---

## Palet Warna & Desain

- **Hero & Header:** Warm Cream (`#FAF7F0`)
- **Konten Utama:** Sage Green Muda (`#E8F0E4`)
- **Kartu Konten:** Pure White (`#FFFFFF`)
- **Tombol Utama & Footer:** Forest Green (`#4F7F5B`)
- **Aksen Harga:** Terracotta (`#D9825B`)
- **Teks Utama:** Deep Charcoal (`#1F2D24`)
- **Tipografi:** Google Fonts *Poppins* (Heading) & *Inter* (Body Text)

---

## Struktur Berkas

```
Landing-UMKM/
├── assets/
│   └── images/              # Aset foto (Hero & Before-After)
│       ├── hero.jpg
│       ├── before-1.jpg
│       ├── after-1.jpg
│       ├── before-2.jpg
│       └── after-2.jpg
├── css/
│   └── style.css            # Stylesheet murni (Mobile-First, Grid & Flexbox)
├── docs/
│   ├── requirement.md       # Dokumen spesifikasi kebutuhan (SKPL v1.0)
│   ├── testing.md           # Laporan hasil pengujian fungsional & nonfungsional
│   └── screenshots/         # Bukti tangkapan layar pengujian multi-viewport
├── index.html               # Halaman utama landing page
├── CHANGELOG.md             # Riwayat perubahan proyek
└── README.md                # Dokumentasi utama proyek
```

---

## Cara Menjalankan Proyek

Pilih salah satu cara di bawah ini untuk membuka website secara lokal:

### Cara 1: Menggunakan Ekstensi Live Server (VS Code)
1. Buka folder proyek di VS Code.
2. Pasang ekstensi **Live Server** (oleh Ritwick Dey).
3. Buka file `index.html`, klik kanan lalu pilih **Open with Live Server**.

### Cara 2: Menggunakan Python (Terminal / Command Prompt)
```bash
python -m http.server 5500
```
Buka peramban di URL: `http://localhost:5500`

### Cara 3: Langsung Buka di Browser
Klik dua kali file `index.html` pada File Explorer untuk membukanya langsung di browser.

---

## Informasi Akademik

- **Mata Kuliah:** Desain Web
- **Dosen Pengampu:** Asep Kurniawan, S.Pd., M.Kom.
- **Kelompok:** 5

### Anggota Kelompok:
1. **Rena Ade Widya** &mdash; `2507431021`
2. **Nadine Safira** &mdash; `2507431027`
3. **Ribby Julina Bangun** &mdash; `2507431055`
4. **Faza Nimas Hayugi Putri Kamila** &mdash; `2507431056`
5. **Fadlan Ahmad Kamil** &mdash; `2507431064`

---

&copy; 2026 KlinShoes &bull; Kelompok 5 Desain Web.
