# Brum-Brum - Single Page Application (SPA) Toko Motor

Aplikasi Web Satu Halaman (SPA) interaktif bertema katalog toko motor bernama **"Brum-Brum"**. Proyek ini dibuat menggunakan **Vanilla JavaScript (JavaScript murni)** dan memanfaatkan **Fetch API** untuk mensimulasikan operasi CRUD (Create, Read, Update, Delete) menggunakan layanan mock-up dari *DummyJSON API*.

## 🚀 Fitur Utama & Alur Kerja
1. **Daftar Katalog (GET):** Menampilkan daftar motor bawaan dari API secara asinkron saat halaman pertama kali dibuka.
2. **Tambah Produk (POST):** Form interaktif untuk menginputkan Nama Motor dan Harga. Respon sukses dari server langsung diolah untuk memanipulasi DOM secara dinamis (*real-time*) di bagian paling atas list tanpa reload.
3. **Edit Produk (PUT):** Mengklik tombol "Edit" akan melempar data ke dalam form pengisian. Perubahan data dikirim via HTTP Method `PUT`, lalu memperbarui komponen visual produk terpilih.
4. **Hapus Produk (DELETE):** Menghapus entitas data produk dari server simulasi dan langsung menendang komponen HTML elemen tersebut secara dinamis dari layar setelah menerima tanda sukses (`isDeleted: true`).
5. **Error Handling & Alert Sistem:** Menggunakan blok `try...catch` modern dengan tampilan pesan kesalahan berupa *alert box* informatif langsung di layar pengguna jika transaksi jaringan/API bermasalah.

## 🛠️ Aturan Teknis yang Diterapkan
- Penulisan skrip asynchronous menggunakan arsitektur modern `async/await`.
- Bebas dari ketergantungan library eksternal (100% Pure Vanilla JS, HTML5, dan CSS3 GRID/Flexbox).
- State manajemen lokal yang sinkron dengan aksi HTTP Request untuk menjaga sifat SPA tetap dinamis tanpa pemicu siklus *reload/refresh* halaman.

## 📁 Cara Menjalankan Aplikasi
1. **Clone Repositori Ini:**
   ```bash
   git clone [https://github.com/USERNAME_KAMU/NAMA_REPO_KAMU.git](https://github.com/USERNAME_KAMU/NAMA_REPO_KAMU.git)