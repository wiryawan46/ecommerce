# E-Commerce Sederhana dengan Laravel, Livewire, Filament, dan Tailwind

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk membangun platform **E-Commerce sederhana** menggunakan:
- **Laravel** sebagai backend utama.
- **Livewire** untuk interaksi dinamis tanpa perlu JavaScript langsung.
- **Filament** sebagai admin panel untuk mengelola produk dan pesanan.
- **Tailwind CSS** untuk tampilan yang modern dan responsif.

Proyek ini cocok bagi pemula yang ingin belajar membangun sistem E-Commerce dari awal dengan teknologi modern berbasis Laravel.

---

## 🔧 Teknologi yang Digunakan

| Teknologi  | Fungsi  |
|------------|---------|
| **Laravel** | Framework backend utama untuk routing, autentikasi, dan logika bisnis. |
| **Livewire** | Framework frontend berbasis PHP untuk interaksi dinamis. |
| **Filament** | Admin panel berbasis Laravel untuk mengelola produk dan pesanan. |
| **Tailwind CSS** | Framework CSS untuk tampilan yang modern dan responsif. |
| **MySQL** | Database untuk menyimpan produk, pengguna, dan transaksi. |
| **Vite** | Build tool untuk mengelola asset bundling. |

---

## 🎯 Fitur-Fitur

### **Fitur Pengguna (Frontend)**
- 🔹 Halaman Beranda: Menampilkan daftar produk dengan fitur pencarian dan filter.
- 🔹 Detail Produk: Informasi lengkap produk dengan opsi menambah ke keranjang.
- 🔹 Keranjang & Checkout: Menambah/menghapus produk, pengisian alamat, dan pembayaran.
- 🔹 Autentikasi: Registrasi, login, logout, dan pengelolaan profil pengguna.
- 🔹 Riwayat Pesanan: Melihat pesanan yang telah dilakukan.

### **Fitur Admin (Backend - Filament Panel)**
- 🔹 **Dashboard Admin**: Statistik penjualan, pengguna, dan pesanan.
- 🔹 **Manajemen Produk**: CRUD produk dan upload gambar.
- 🔹 **Manajemen Pesanan**: Mengubah status pesanan (Diproses, Dikirim, Selesai).
- 🔹 **Manajemen Pengguna**: Mengelola data pengguna.

---

## 🔄 Alur Kerja Aplikasi
1. **Pengguna mengakses website** → melihat daftar produk.
2. **Pengguna memilih produk** → menambah ke keranjang.
3. **Pengguna checkout** → mengisi detail pengiriman & menyelesaikan pembayaran.
4. **Admin menerima pesanan** → memproses pesanan melalui dashboard Filament.
5. **Pesanan dikirim ke pelanggan** → pengguna mendapatkan update status pesanan.

---

## 📁 Struktur Folder Proyek
```
ecommerce-laravel/
│── app/
│   ├── Http/
│   │   ├── Controllers/  # Berisi controller untuk request
│   │   ├── Livewire/     # Komponen Livewire untuk frontend
│   ├── Models/          # Model untuk Produk, Pesanan, User, dll.
│── database/
│   ├── migrations/      # File migrasi database
│── resources/
│   ├── views/           # Template Blade dan komponen Livewire
│   ├── css/             # File Tailwind CSS
│── routes/
│   ├── web.php          # Routing utama aplikasi
│── public/              # Asset publik (gambar produk, dll.)
│── composer.json        # Konfigurasi Laravel & dependensi PHP
│── package.json         # Konfigurasi npm untuk Tailwind & Vite
```

---

## ⚙️ Instalasi dan Konfigurasi

### **1️⃣ Clone Repository & Install Dependencies**
```bash
git clone https://github.com/wiryawan46/ecommerce.git
cd ecommerce-laravel
composer install
npm install
```

### **2️⃣ Konfigurasi Environment**
Salin file `.env.example` menjadi `.env`:
```bash
cp .env.example .env
```
Ubah pengaturan database di `.env`:
```
DB_DATABASE=ecommerce_db
DB_USERNAME=root
DB_PASSWORD=password_mysql
```

### **3️⃣ Jalankan Migrasi dan Seeder**
```bash
php artisan migrate --seed
```

### **4️⃣ Jalankan Server**
```bash
php artisan serve
npm run dev
```
Buka `http://127.0.0.1:8000` di browser.

---

## 📌 Pengembangan Selanjutnya
- 🔹 **Integrasi Midtrans/Xendit** untuk pembayaran online.
- 🔹 **Menambahkan API** untuk aplikasi mobile.
- 🔹 **Fitur Review & Rating** untuk produk.
- 🔹 **Diskon & Kupon Belanja**.
- 🔹 **Optimasi performa dengan Lazy Loading & Caching**.

---

## 📚 Referensi & Tutorial
Proyek ini terinspirasi dari tutorial berikut:
🔗 [YouTube Playlist - Belajar E-Commerce Laravel](https://www.youtube.com/playlist?list=PL6u82dzQtlfv8fJF3gm42TDHJdtA2NDWT)

---

🚀 **Selamat belajar dan selamat coding!** 🎉
