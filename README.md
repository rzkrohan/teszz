# UpToGH

Upload dokumen dan media langsung ke GitHub repository dari browser, tanpa perlu install apa pun.

## Cara pakai

1. Buka `index.html` di browser (atau jalankan `npm install` lalu `npm start` untuk local server).
2. Masuk menggunakan **username GitHub** dan **Personal Access Token** (buat di https://github.com/settings/tokens, izin minimal `repo`).
3. Isi nama repository tujuan. Jika belum ada, akan dibuat otomatis.
4. Pilih file (bisa banyak file, semua jenis dokumen/media didukung).
5. Jika salah satu file adalah `.zip`, akan muncul tombol **Ekstrak ZIP** — aktifkan jika ingin isi zip diekstrak langsung ke repository, atau biarkan mati untuk upload file zip apa adanya.
6. Klik **Upload**. Setelah selesai, tautan repository akan muncul.

## Catatan keamanan

Token GitHub hanya digunakan langsung dari browser kamu ke GitHub API (`api.github.com`) dan tidak dikirim atau disimpan ke server mana pun.

## Struktur file

- `index.html` — halaman utama
- `style.css` — tema biru-putih
- `app.js` — logika login & upload (ES module)
- `package.json` — opsional, untuk menjalankan local dev server

---
© 2026 rizky rohan — UpToGH
