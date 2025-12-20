<!-- portfolio -->
<!-- slug: authbook-laravel-filament -->
<!-- title: Sistem Manajemen AuthBook -->
<!-- description: Sistem autentikasi dan manajemen buku yang dibangun dengan Laravel 10 dan panel admin Filament -->
<!-- image: https://github.com/user-attachments/assets/de85ddfe-de3c-46dc-9cfa-0d77efd628f3 -->
<!-- tags: laravel, filament, php, autentikasi, panel-admin -->

# AuthBook Laravel 10 dengan Filament

<img width="1536" height="1024" alt="authbook-laravel-filament" src="https://github.com/user-attachments/assets/de85ddfe-de3c-46dc-9cfa-0d77efd628f3" />

Sistem autentikasi dan manajemen buku yang komprehensif dibangun dengan Laravel 10 dan panel admin Filament. Proyek ini berfungsi sebagai contoh pembelajaran untuk mengimplementasikan panel admin modern dengan Filament dalam aplikasi Laravel, dibuat untuk kelas Pemrograman Berbasis Web (PBW).

## 📋 Ringkasan

AuthBook adalah sistem manajemen buku fitur lengkap yang mendemonstrasikan integrasi Laravel 10 dengan panel admin Filament. Proyek ini menampilkan praktik terbaik dalam membangun aplikasi CRUD (Create, Read, Update, Delete) dengan autentikasi, otorisasi, dan antarmuka admin yang modern.

## ✨ Fitur

- **Autentikasi & Otorisasi Pengguna**
  - Sistem login/logout yang aman.
  - Kontrol akses berbasis peran (Role-based access control).
  - Manajemen profil pengguna.

- **Manajemen Buku**
  - Operasi CRUD lengkap untuk buku.
  - Kategorisasi dan penandaan buku (tagging).
  - Pencarian dan filter tingkat lanjut.
  - Dukungan tindakan massal (bulk actions).

- **Panel Admin Modern (Filament)**
  - UI yang cantik dan responsif.
  - Dashboard yang dapat dikustomisasi.
  - Manajemen resource.
  - Form builder dan tabel.
  - Notifikasi dan widget.

- **Manajemen Database**
  - Integrasi database MySQL.
  - Relasi Eloquent ORM.
  - Migrasi dan seeder database.

## 🛠️ Teknologi yang Digunakan

- **Framework**: Laravel 10
- **Panel Admin**: Filament v3
- **Bahasa**: PHP 8.1+
- **Database**: MySQL
- **Frontend**: Livewire, Alpine.js, Tailwind CSS
- **Autentikasi**: Laravel Breeze/Sanctum

## 📁 Struktur Proyek

```
authbook-laravel-filament/
├── app/
│   ├── Filament/              # Resource Filament
│   ├── Models/                # Model Eloquent
│   └── Policies/              # Kebijakan otorisasi (Policies)
├── database/
│   ├── migrations/            # Migrasi database
│   └── seeders/               # Seeder database
├── resources/
│   └── views/                 # Template Blade
├── routes/
│   └── web.php               # Rute web
└── config/
    └── filament.php          # Konfigurasi Filament
```

## 🚀 Memulai

### Prasyarat

- PHP 8.1 atau yang lebih baru.
- Composer.
- MySQL 5.7+ atau MariaDB.
- Node.js & NPM (untuk kompilasi aset).

### Langkah Instalasi

1. **Clone repositori**
   ```bash
   git clone <repository-url>
   cd authbook-laravel-filament
   ```

2. **Install dependensi PHP**
   ```bash
   composer install
   ```

3. **Install dependensi Node**
   ```bash
   npm install
   ```

4. **Pengaturan Environment**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

5. **Konfigurasi Database**
   - Buat database MySQL.
   - Perbarui file `.env`:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=authbook_db
   DB_USERNAME=root
   DB_PASSWORD=password_anda
   ```

6. **Jalankan Migrasi & Seeder**
   ```bash
   php artisan migrate --seed
   ```

7. **Buat Pengguna Admin**
   ```bash
   php artisan make:filament-user
   ```
   Ikuti petunjuk untuk membuat akun admin Anda.

8. **Build Aset**
   ```bash
   npm run dev
   ```

9. **Jalankan Server Pengembangan**
   ```bash
   php artisan serve
   ```

10. **Akses Aplikasi**
    - Frontend: `http://localhost:8000`
    - Panel Admin: `http://localhost:8000/admin`

## 💻 Penggunaan

### Mengakses Panel Admin

1. Navigasi ke `http://localhost:8000/admin`.
2. Login dengan kredensial admin yang telah dibuat sebelumnya.
3. Akses dashboard untuk mengelola buku dan pengguna.

### Mengelola Buku

1. Klik pada "Books" di sidebar admin.
2. Gunakan tombol "New Book" untuk menambah buku.
3. Isi detail buku (judul, penulis, ISBN, deskripsi, dll.).
4. Klik "Create" untuk menyimpan.

### Manajemen Pengguna

1. Akses "Users" dari panel admin.
2. Lihat, edit, atau hapus pengguna.
3. Tetapkan peran dan izin.

## 🎓 Tujuan Pembelajaran

Proyek ini mendemonstrasikan:

- **Integrasi Filament**: Cara mengintegrasikan dan menyesuaikan panel admin Filament.
- **Manajemen Resource**: Membuat resource Filament untuk operasi CRUD.
- **Autentikasi**: Mengimplementasikan autentikasi pengguna yang aman.
- **Otorisasi**: Kontrol akses berbasis peran.
- **Relasi Database**: Relasi Eloquent dan migrasi.
- **PHP Modern**: Fitur PHP 8.1+ terbaru dan praktik terbaik Laravel.

## 📚 Resource Filament

Proyek ini mencakup contoh resource Filament untuk:
- Manajemen buku.
- Administrasi pengguna.
- Manajemen kategori.
- Widget dashboard.

## 🔧 Konfigurasi

### Kustomisasi Filament

Edit `config/filament.php` untuk menyesuaikan:
- Nama brand dan logo.
- Skema warna.
- Item navigasi.
- Middleware dan guards.

### Seeder Database

Proyek ini menyertakan seeder untuk:
- Contoh buku.
- Pengguna demo.
- Kategori dan tag.

Jalankan seeder dengan:
```bash
php artisan db:seed
```

## 🤝 Kontribusi

Proyek ini digunakan untuk tujuan pendidikan di kelas Pemrograman Berbasis Web. Kontribusi untuk meningkatkan contoh dan dokumentasi sangat diterima!

1. Fork repositori.
2. Buat branch fitur.
3. Commit perubahan Anda.
4. Push ke branch tersebut.
5. Buka Pull Request.

## 📄 Lisensi

Proyek ini bersifat open source dan tersedia untuk tujuan edukasi.

## 📖 Resource

- [Dokumentasi Laravel](https://laravel.com/docs)
- [Dokumentasi Filament](https://filamentphp.com/docs)
- [Dokumentasi Livewire](https://livewire.laravel.com/docs)

## 📞 Kontak

Untuk pertanyaan tentang proyek pembelajaran ini, silakan hubungi melalui informasi yang tersedia di portofolio saya.
