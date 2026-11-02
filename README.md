# Manajemen Karu RSUD Merauke — GitHub Pages

Antarmuka web untuk aplikasi **Manajemen Kepala Ruangan (Karu)** yang terhubung ke sistem KMKP (Komite Mutu dan Keselamatan Pasien) RSUD Merauke.

## Cara Pasang

1. Upload semua isi folder ini ke repository GitHub (atau branch `gh-pages`).
2. Aktifkan **GitHub Pages** di Settings → Pages → pilih branch/folder.
3. Edit file `config.js` → isi `KARU_API_URL` dengan URL `/exec` proyek Google Apps Script Karu Anda.
4. Commit & push. Tunggu 1-2 menit, buka URL GitHub Pages, tekan Ctrl+F5.

## Syarat Sebelum Membuka

- Proyek GAS KARU sudah di-deploy sebagai **Aplikasi web** (Jalankan sebagai: Saya, Akses: Siapa saja).
- Proyek GAS KMKP sudah di-deploy dan URL-nya sudah diisikan di `KMKP_URL_TETAP` pada `Kode.gs` KARU.
- Fungsi `setupKaru` sudah dijalankan satu kali dari editor Apps Script.
- Login menggunakan akun KMKP dengan peran **Karu**, Admin, Komite, atau KetuaKomite.

## File

| File | Keterangan |
|---|---|
| `index.html` | Halaman utama aplikasi (satu halaman / SPA) |
| `config.js` | **Edit ini**: isi `KARU_API_URL` dengan URL /exec |
| `manifest.json` | Metadata PWA (installable di Android/iOS) |
| `sw.js` | Service worker untuk akses offline |
| `logo.png` | Ikon aplikasi |
| `.nojekyll` | Mencegah GitHub Pages memproses dengan Jekyll |
