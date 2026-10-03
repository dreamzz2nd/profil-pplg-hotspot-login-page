# profil-pplg-hotspot-login-page

Template Hotspot Login MikroTik bertema Profil Jurusan PPLG SMKN 1 Cirebon.

## Fitur
- **Pure Account Login**: Login menggunakan akun Username & Password (terintegrasi dengan MikroTik CHAP MD5).
- **Responsive Landing Page**: Desain modern dengan Tailwind CSS, responsif untuk Mobile, Tablet, dan Desktop.
- **Dynamic Swiper Carousel**: Banner showcase terintegrasi dengan API dinamis backend Laravel (`/api/iklan`) serta fallback banner lokal.
- **Stand-alone Inline SVG Icons**: Semua icon menggunakan inline SVG sehingga tidak memerlukan dependensi eksternal / CDN saat klien belum login hotspot.
- **Halaman Lengkap**: 
  - `login.html` (Halaman Login & Landing Page Profil)
  - `status.html` (Status Koneksi, IP, Uptime, Transfer Data, Sisa Waktu & Kuota)
  - `logout.html` (Ringkasan Sesi & Tombol Login Kembali)
  - `alogin.html` (Redirecting & Auto-forward ke status)
  - `error.html` (Tampilan Notifikasi Kesalahan Login)
  - `radvert.html` (Halaman Iklan / Sponsor)

## Cara Pemasangan di MikroTik
1. Salin seluruh isi folder ini ke direktori hotspot router MikroTik Anda (misalnya `/hotspot`).
2. Pastikan file `md5.js` berada di direktori yang sama dengan `login.html`.
3. Set Server Profile Hotspot MikroTik Anda untuk menggunakan HTML directory tersebut.
