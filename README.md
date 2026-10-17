# Sistem Pendaftaran Ekstrakurikuler SMK Negeri 1 Cijati

Aplikasi web untuk mengelola pendaftaran kegiatan ekstrakurikuler secara
daring. Sistem ini menggantikan pendaftaran manual (formulir kertas dan
rekap berkas) dengan alur yang lebih cepat, rapi, dan terpusat bagi siswa,
pembina, dan pihak sekolah.

## Fitur Utama

### Siswa
- Pembuatan akun dan login
- Melihat daftar eskul lengkap dengan foto, jadwal, deskripsi, dan pembina
- Mendaftar eskul secara online (maksimal 5 eskul per siswa, tanpa
  pendaftaran ganda pada eskul yang sama)

### Pembina
- Melihat daftar pendaftar pada eskul yang dibina
- Mengubah dan menghapus data siswa anggota eskulnya

### Administrator
- Mengelola data eskul (nama, pembina, foto, jadwal, deskripsi)
- Mengelola akun pembina dan siswa
- Memantau dan menghapus data pendaftaran
- Mengelola keanggotaan eskul

### Keamanan Akses
Hak akses dibedakan menjadi tiga level (siswa, pembina, admin). Halaman
admin dilindungi middleware sehingga hanya dapat diakses oleh administrator.

## Teknologi yang Digunakan

- Framework: Laravel 13
- Bahasa pemrograman: PHP 8.3 atau lebih baru
- Basis data: MySQL
- Antarmuka: Blade Template, CSS, JavaScript

## Persyaratan Sistem

- PHP 8.3 atau lebih baru
- Composer
- Node.js dan NPM
- MySQL

## Instalasi

1. Clone repositori
   git clone https://github.com/ulwanFM72/<nama-repo>.git
   cd <nama-repo>

2. Pasang dependensi
   composer install
   npm install

3. Siapkan berkas lingkungan
   cp .env.example .env
   php artisan key:generate

4. Buat basis data MySQL kosong, lalu atur pada `.env`:
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=<nama_database>
   DB_USERNAME=<username>
   DB_PASSWORD=<password>

5. Jalankan migrasi dan data awal
   php artisan migrate --seed

6. Jalankan aplikasi
   php artisan serve

Aplikasi dapat diakses melalui http://localhost:8000.

Akun administrator awal dibuat oleh seeder. Segera ganti kata sandinya
setelah login pertama.

## Alur Penggunaan

1. Admin mendaftarkan pembina dan eskul beserta jadwal dan deskripsinya.
2. Siswa membuat akun, lalu login.
3. Siswa memilih eskul dan mendaftar.
4. Pembina memantau pendaftar dan anggota eskulnya.
5. Admin memantau dan mengelola seluruh data.

## Kredit

Dikembangkan oleh Ulwan Fauzul Muqtaf.

## Lisensi

Cantumkan lisensi sesuai ketentuan sekolah.
