# Dokumentasi Pengujian

Dokumen ini mencatat hasil pengujian fitur dan kualitas pada proyek Landing-UMKM (KlinShoes).

## Status

Belum ada pengujian yang dijalankan. `index.html` dan `css/style.css` masih kosong, sehingga belum ada fitur yang dapat diuji.

## Kriteria Penerimaan

Kriteria berikut diambil dari `docs/requirement.md` bagian 1.5 dan akan diuji setelah implementasi selesai.

| No | Kriteria | Status | Catatan |
|----|----------|--------|---------|
| 1 | Halaman lolos validasi HTML5 W3C tanpa error fatal | Belum diuji | - |
| 2 | Tidak ada elemen terpotong pada lebar layar 320px sampai 480px | Belum diuji | - |
| 3 | Tombol navigasi mengarah ke bagian yang tepat di halaman | Belum diuji | - |
| 4 | Tombol CTA WhatsApp membuka WhatsApp dengan pesan bawaan | Belum diuji | - |
| 5 | Seluruh tata letak dan gaya dirender dari file CSS eksternal | Belum diuji | - |

## Rencana Pengujian Fungsional

| No | Fitur | Skenario | Hasil Diharapkan | Status |
|----|-------|----------|------------------|--------|
| 1 | Navigasi | Klik menu Beranda, Layanan, Keunggulan, Galeri, Kontak | Halaman melompat ke seksi yang sesuai | Belum diuji |
| 2 | Katalog layanan | Halaman dimuat | Tampil minimal 3 layanan dengan deskripsi dan harga | Belum diuji |
| 3 | Galeri | Halaman dimuat | Tampil minimal 4 pasang foto before-after dalam grid | Belum diuji |
| 4 | CTA WhatsApp | Klik tombol "Konsultasi dan Cuci Sekarang" | Membuka wa.me dengan pesan otomatis | Belum diuji |
| 5 | Informasi bisnis | Halaman dimuat | Tampil alamat, jam operasional, dan tautan sosial | Belum diuji |

## Rencana Pengujian Nonfungsional

| No | Aspek | Metode | Target | Status |
|----|-------|--------|--------|--------|
| 1 | Responsivitas | Uji di lebar 320px, 375px, 480px, 768px, 1024px | Layout menyesuaikan, tanpa horizontal scroll | Belum diuji |
| 2 | Performa | Ukur waktu muat pada koneksi 4G | Muat di bawah 3 detik | Belum diuji |
| 3 | Kompatibilitas | Uji di beberapa browser (Chrome, Firefox, Edge) | Tampilan konsisten | Belum diuji |
| 4 | Hover effect | Arahkan kursor ke tombol dan tautan | Ada perubahan warna atau bayangan dengan transition | Belum diuji |

## Template Catatan Hasil Uji

Gunakan format berikut saat mencatat hasil pengujian:

```
Tanggal   : YYYY-MM-DD
Penguji   : nama
Lingkungan: browser, versi, ukuran layar
Skenario  : deskripsi singkat
Hasil     : Lulus / Gagal
Catatan   : detail temuan
```
