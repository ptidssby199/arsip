# Arsip Parkir & Tol

Aplikasi web statis (satu file `index.html`) untuk mengarsipkan bukti parkir dan tol beserta foto, dengan laporan siap cetak. Data disimpan di IndexedDB browser.

## Deploy ke GitHub Pages
1. Buat repositori baru di GitHub (mis. `arsip-parkir-tol`).
2. Upload semua file: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`, dan `README.md`.
3. Buka Settings > Pages > Source: pilih branch `main`, folder `/ (root)`, lalu Save.
4. Tunggu 1-2 menit. Alamat: `https://USERNAME.github.io/arsip-parkir-tol/`

## Catatan
- Data tersimpan di browser tiap perangkat, tidak otomatis sinkron.
- Pindah data antar perangkat: tombol **Cadangkan** (unduh .json), lalu **Pulihkan** di perangkat lain.

## Pasang sebagai aplikasi (PWA)
- Android/Chrome: buka alamat GitHub Pages, menu titik tiga > **Instal aplikasi** / **Tambahkan ke layar utama**.
- iPhone/Safari: tombol Bagikan > **Tambah ke Layar Utama**.
- Setelah dibuka sekali dengan internet, aplikasi bisa dipakai offline.
- Saat memperbarui `index.html`, ubah `CACHE = "arsip-pt-v1"` di `sw.js` (mis. `v2`) agar versi baru terambil.
