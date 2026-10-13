# Contoh Undangan Pernikahan Digital

Project undangan pernikahan digital interaktif berbasis HTML/CSS/JS murni (tanpa framework).

> **Catatan:** Semua data di dalam project ini adalah **data contoh (dummy)**.  
> Silakan ganti dengan data asli sebelum digunakan.

---

## Struktur File

| File                       | Keterangan                                                 |
| -------------------------- | ---------------------------------------------------------- |
| `undangan-pernikahan.html` | **Halaman Utama** — undangan lengkap                       |
| `e-angpao.html`            | **Halaman Kirim Duit** — transfer bank + QRIS + konfirmasi |
| `README.md`                | Dokumentasi project ini                                    |

---

## Fitur Halaman Utama

- Animasi amplop pembuka (envelope opening)
- Musik background (play/pause)
- Quote Al-Qur'an
- Profil mempelai + nama keluarga
- Love Story (timeline)
- Gallery Prewedding + Lightbox
- Detail acara (Akad & Resepsi)
- Countdown timer real-time
- Tombol Google Maps & RSVP WhatsApp
- Tombol menuju E-Angpao
- Buku Tamu (siap dihubungkan ke Google Sheet)

## Fitur Halaman E-Angpao

- Nomor rekening bank (BCA & Mandiri) + tombol salin
- Placeholder QRIS
- Form konfirmasi (nama, jumlah, ucapan) → langsung ke WhatsApp
- Design menyesuaikan tema undangan

---

## Cara Menjalankan

1. Download / clone semua file
2. Buka `undangan-pernikahan.html` di browser (Chrome / Safari / Firefox)
3. Atau upload ke hosting gratis (Netlify, Vercel, GitHub Pages) agar bisa dibagikan lewat link

---

## Yang Perlu Diganti (Data Asli)

### Halaman Utama (`undangan-pernikahan.html`)

- Nama mempelai pria & wanita
- Nama orang tua & saudara
- Tanggal, waktu, dan tempat acara
- Link Google Maps
- Nomor WhatsApp RSVP
- Foto prewedding (ganti URL Unsplash)
- Cerita Love Story
- URL Google Apps Script untuk Buku Tamu (lihat petunjuk di dalam kode)

### Halaman E-Angpao (`e-angpao.html`)

- Nomor rekening + nama bank + atas nama
- Gambar / link QRIS
- Nomor WhatsApp tujuan konfirmasi transfer

---

## Setup Buku Tamu (Google Sheet) — Opsional

1. Buat Google Sheet baru
2. Header baris 1: `timestamp` | `name` | `message`
3. Extensions → Apps Script → paste kode `doGet` & `doPost` (ada di dalam file HTML)
4. Deploy sebagai Web App (Execute as: Me, Who has access: Anyone)
5. Copy URL → ganti `SCRIPT_URL` di dalam `undangan-pernikahan.html`

---

## Teknologi

- HTML5
- CSS3 (Flexbox, Grid, Animations)
- JavaScript (Vanilla)
- Google Fonts (Great Vibes, Playfair Display, Poppins)
- Unsplash (foto contoh)

---
