# Undangan Pernikahan Digital

Website undangan pernikahan digital yang interaktif dan responsif. Tamu dapat melihat informasi mempelai dan acara, menjelajahi galeri, mengirim konfirmasi kehadiran melalui WhatsApp, serta mengakses halaman E-Angpao.

> **Catatan:** Nama, tanggal acara, nomor rekening, foto, dan informasi lain yang tersedia di project ini merupakan **data contoh (dummy)**. Ganti dengan data yang benar sebelum undangan dibagikan.

---

## Masalah

Informasi pernikahan sering dibagikan melalui banyak media sehingga detail acara, lokasi, konfirmasi kehadiran, dan ucapan tamu tidak terkumpul dalam satu tempat.

## Solusi

Undangan Pernikahan Digital menyajikan informasi acara dalam satu website yang mudah dibuka melalui browser. Tamu dapat melihat detail acara, membuka lokasi di Google Maps, menghubungi keluarga melalui WhatsApp, dan mengirim ucapan melalui buku tamu yang dapat dihubungkan ke Google Sheets.

## Fitur Utama

**Undangan utama (`index.html`)**

- Animasi amplop pembuka dan kontrol musik
- Profil mempelai, keluarga, dan cerita perjalanan pasangan
- Galeri prewedding dengan lightbox
- Informasi akad dan resepsi beserta hitung mundur acara
- Tautan lokasi Google Maps dan konfirmasi kehadiran via WhatsApp
- Buku tamu yang dapat dihubungkan ke Google Sheets melalui Google Apps Script
- Tautan menuju halaman E-Angpao

**E-Angpao (`e-angpao.html`)**

- Informasi transfer bank dengan tombol salin nomor rekening
- Area QRIS yang dapat diganti dengan QRIS asli
- Form konfirmasi dan ucapan yang diteruskan melalui WhatsApp

## Tech Stack

- HTML5
- CSS3 (Flexbox, Grid, animasi, dan responsive layout)
- JavaScript (Vanilla)
- Google Fonts
- Google Apps Script dan Google Sheets (opsional, untuk buku tamu)

## Demo

Buka `index.html` di browser untuk melihat undangan. Halaman E-Angpao dapat dibuka melalui tombol di undangan atau langsung dari `e-angpao.html`.

## Instalasi

Project ini tidak memerlukan proses build atau instalasi dependency.

```bash
git clone https://github.com/SulthanAfif/UndanganPernikahan.git
cd UndanganPernikahan
```

Buka `index.html` di browser, atau unggah file project ke hosting statis seperti GitHub Pages, Netlify, atau Vercel.

## Kustomisasi

Sebelum membagikan undangan, ganti data contoh di file HTML, termasuk:

- Nama mempelai, keluarga, cerita, dan foto
- Tanggal, waktu, dan lokasi acara
- Tautan Google Maps dan nomor WhatsApp RSVP
- Nomor rekening, nama pemilik rekening, QRIS, dan nomor WhatsApp konfirmasi E-Angpao
- URL Google Apps Script pada variabel `SCRIPT_URL` di `index.html` jika buku tamu akan digunakan

Untuk mengaktifkan buku tamu, siapkan Google Sheets dengan kolom `timestamp`, `name`, dan `message`, lalu deploy Google Apps Script sebagai Web App. Petunjuk dan kode integrasi tersedia di dalam `index.html`.

## Repository

📦 [github.com/SulthanAfif/UndanganPernikahan](https://github.com/SulthanAfif/UndanganPernikahan)

---

**Undangan Pernikahan Digital** — informasi hari bahagia dalam satu undangan online.
