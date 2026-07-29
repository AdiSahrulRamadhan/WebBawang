# Subang — Website Bawang (Surabaya Bawang)

Website satu halaman (single page), statis, siap deploy gratis di Netlify.

## Isi folder
- `index.html` — seluruh website (HTML, CSS, JS jadi satu file, tanpa build step)
- `netlify.toml` — konfigurasi dasar Netlify
- `README.md` — file ini

## Cara deploy ke Netlify (gratis, ±2 menit)

**Cara termudah — drag & drop:**
1. Buka https://app.netlify.com/drop
2. Login/daftar (bisa pakai akun Google/GitHub, gratis)
3. Seret (drag) folder ini ke halaman tersebut
4. Netlify otomatis kasih link publik, misalnya `nama-acak.netlify.app`
5. Kalau mau ganti nama, buka **Site settings → Change site name**

**Cara lain — lewat GitHub (kalau mau auto-update tiap ada perubahan):**
1. Upload folder ini ke repository GitHub
2. Di Netlify, klik **Add new site → Import an existing project**
3. Pilih repository tersebut, biarkan setting default (tidak perlu build command)
4. Klik **Deploy**

## Mengganti data kontak
Buka `index.html`, cari bagian `id="kontak"`, lalu ubah:
- Nama & inisial di lingkaran avatar
- Nomor WhatsApp (di `href="https://wa.me/62..."`, format: 62 + nomor tanpa angka 0 di depan)
- Email
- Alamat
- Link Instagram & TikTok (saat ini masih pakai username contoh `subang.id` — ganti dengan username asli)

## Formulir kontak
Formulir di bagian bawah sudah memakai **Netlify Forms** (`data-netlify="true"`), jadi begitu website ini di-deploy di Netlify, pesan yang dikirim lewat form akan otomatis masuk ke dashboard Netlify (menu **Forms**) tanpa perlu server atau backend tambahan — semuanya gratis di tier dasar Netlify.

## Mengganti warna/teks
Semua warna diatur di bagian atas `index.html` dalam `:root { ... }` (variabel CSS), jadi bisa diganti dari satu tempat saja.