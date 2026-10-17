# Sistem Pendaftaran Ekstrakurikuler SMK Negeri 1 Cijati

Aplikasi web untuk mengelola pendaftaran kegiatan ekstrakurikuler secara
daring. Sistem ini menggantikan proses pendaftaran manual (formulir kertas
dan rekap berkas) dengan alur yang lebih cepat, rapi, dan transparan bagi
siswa, pembina, maupun pihak sekolah.

## Latar Belakang

Pendaftaran eskul secara manual rentan terhadap data ganda, berkas hilang,
dan rekap yang memakan waktu. Aplikasi ini dibuat agar seluruh proses,
mulai dari pemilihan eskul, pendaftaran, hingga pengelolaan anggota,
dilakukan dalam satu sistem terpusat.

## Fitur Utama

### Siswa
- Registrasi dan login akun siswa
- Melihat daftar eskul beserta deskripsi, jadwal, dan pembina
- Mendaftar eskul secara online
- Memantau status pendaftaran (menunggu, diterima, ditolak)
- Melihat riwayat eskul yang diikuti

### Pembina
- Melihat daftar pendaftar pada eskul yang dibina
- Menyetujui atau menolak pendaftaran
- Mengelola data anggota

### Administrator
- Mengelola data eskul (tambah, ubah, hapus)
- Mengelola akun siswa dan pembina
- Mengatur periode dan kuota pendaftaran
- Rekap data pendaftar dan ekspor laporan

## Teknologi yang Digunakan

- Framework: Laravel
- Bahasa pemrograman: PHP
- Basis data: MySQL
- Antarmuka: Blade Template, Bootstrap, JavaScript

## Persyaratan Sistem

- PHP 8.2 atau lebih baru
- Composer
- Node.js dan NPM
- MySQL

## Instalasi

1. Clone repositori
   git clone https://github.com/ulwanFM72/official_smkn1cijati.git
   cd official_smkn1cijati

2. Pasang dependensi
   composer install
   npm install

3. Siapkan berkas lingkungan
   cp .env.example .env
   php artisan key:generate

4. Atur koneksi basis data pada `.env`, lalu migrasi dan isi data awal
   php artisan migrate --seed

5. Jalankan aplikasi
   php artisan serve
   npm run dev

Aplikasi dapat diakses melalui http://localhost:8000.

## Alur Penggunaan

1. Siswa membuat akun dan masuk ke sistem.
2. Siswa memilih eskul dan mengirim pendaftaran.
3. Pembina meninjau dan memberi keputusan.
4. Siswa menerima pembaruan status pendaftaran.
5. Admin memantau dan merekap seluruh data.

## Kontribusi

Silakan ajukan *issue* untuk melaporkan masalah atau usulan fitur, dan
kirimkan *pull request* untuk perbaikan.

## Kredit

Dikembangkan oleh ulwan fauzul muqtaf

## Lisensi

Cantumkan lisensi sesuai ketentuan sekolah dan repositori asal.
