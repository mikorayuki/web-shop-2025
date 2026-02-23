WEB SHOP

```
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Web%20Shop%202025&fontSize=50&animation=fadeIn" width="100%">
  
  <h1>🛒 Web Shop 2025</h1>
  <p><i>Platform E-Commerce Modern, Dinamis & Responsif</i></p>

  <p>
    <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge&logo=github" alt="Status">
    <img src="https://img.shields.io/badge/Version-1.0.0-blue?style=for-the-badge" alt="Version">
  </p>
</div>

---

## 📖 Tentang Project

**Web Shop 2025** adalah platform e-commerce statis yang dirancang untuk menjadi ringan, cepat, dan mudah dikelola. Proyek ini sangat cocok untuk toko online skala kecil menengah atau portofolio. Keunggulan utama dari proyek ini adalah Anda tidak memerlukan database backend yang rumit; semua data toko, kategori, dan produk dikelola sepenuhnya melalui satu file JSON (`shop-data.json`).

## ✨ Fitur Utama

- 🛍️ **Katalog Produk Dinamis:** Menampilkan daftar produk yang di-generate secara otomatis dari file JSON.
- 📱 **Desain Super Responsif:** Tampilan menyesuaikan secara mulus di layar Desktop, Tablet, maupun Smartphone.
- 🔍 **Pencarian & Filter Kategori:** Fitur pencarian produk real-time dan penyaringan berdasarkan kategori.
- 🖼️ **Pop-up Detail Produk (Modal):** Pengguna dapat melihat detail produk tanpa harus berpindah halaman.
- ⚙️ **Manajemen Tanpa Coding:** Tambah, edit, atau hapus produk cukup dengan mengubah teks di file `shop-data.json`.
- ⚡ **Performa Tinggi:** Tidak ada waktu tunggu dari server database, memuat halaman secara instan.

## 🛠️ Teknologi yang Digunakan

Proyek ini dibangun murni menggunakan teknologi web standar tanpa framework JavaScript yang berat:
- **HTML5** untuk semantik dan struktur halaman.
- **CSS3 (Vanilla)** dengan penerapan *Custom Properties (Variables)* untuk tema.
- **JavaScript (ES6+)** untuk logika DOM, Fetch API, dan interaktivitas.
- **FontAwesome 6** untuk ikon UI.
- **Animate.css** untuk animasi transisi halaman yang halus.
- **Google Fonts** (Poppins & Montserrat) untuk tipografi modern.

## 📂 Susunan Project (Project Structure)

```text
📁 web-shop-2025/
├── 📄 index.html        # Halaman utama toko (UI E-commerce)
├── 📄 panduan.html      # Panduan lengkap cara mengedit data toko untuk pemilik
├── 📄 styles.css        # File styling utama (Warna, Layout, Responsif)
├── 📄 test.css          # File styling eksperimental / cadangan
├── 📄 main.js           # Logika utama UI (pencarian, filter, modal)
├── 📄 shop-data.js      # Script untuk mengambil dan memvalidasi JSON
├── 📄 shop-data.json    # "Database" utama toko (Konfigurasi info, kategori & produk)
└── 📄 README.md         # Dokumentasi project ini

```

## 📋 Prasyarat Instalasi

Karena proyek ini menggunakan fitur `Fetch API` JavaScript untuk memuat file `shop-data.json`, Anda **tidak bisa** membukanya hanya dengan klik ganda file `index.html` di browser (akan terkena pemblokiran CORS). Anda memerlukan **Local Web Server**.

Beberapa opsi web server lokal yang bisa digunakan:

* Ekstensi **Live Server** di Visual Studio Code.
* Web Server for Chrome.
* Python (jalankan `python -m http.server` di terminal).
* Node.js (seperti `http-server` atau `live-server`).

## 🚀 Cara Instalasi & Menjalankan

1. **Clone repository ini ke komputer/HP Anda:**
```bash
git clone [https://github.com/mikorayuki/web-shop-2025.git](https://github.com/mikorayuki/web-shop-2025.git)

```


2. **Masuk ke direktori project:**
```bash
cd web-shop-2025

```


3. **Jalankan local server.** (Contoh menggunakan Python):
```bash
python -m http.server 8000

```


4. Buka browser dan akses alamat: `http://localhost:8000`

## 💡 Contoh Penggunaan

Untuk mengubah nama toko, kontak, atau menambah produk, Anda hanya perlu mengedit file `shop-data.json`.

**Contoh Menambah Produk Baru:**
Buka `shop-data.json`, lalu pada bagian array `"products"`, tambahkan objek produk baru seperti ini:

```json
{
  "id": "item-003",
  "categoryId": "apkprem",
  "name": "Spotify Premium 1 Bulan",
  "price": "Rp 15.000",
  "description": "Akun Spotify Premium legal dan bergaransi penuh selama 1 bulan.",
  "image": "[https://link-gambar-anda.com/spotify.jpg](https://link-gambar-anda.com/spotify.jpg)",
  "link": "[https://wa.me/083833826401](https://wa.me/083833826401)",
  "badge": "Promo"
}

```

*Catatan: Pastikan `categoryId` cocok dengan ID yang ada di dalam daftar `"categories"`. Untuk panduan lebih lengkap, buka file `panduan.html` di browser Anda.*

## 🤝 Kontribusi (Contributing)

Kontribusi sangat dipersilakan! Jika Anda ingin memperbaiki bug, menambah fitur, atau meningkatkan tampilan:

1. Lakukan *Fork* pada repository ini.
2. Buat branch fitur baru Anda: `git checkout -b fitur-keren-saya`
3. Lakukan commit perubahan Anda: `git commit -m 'Menambahkan fitur keren'`
4. Push ke branch tersebut: `git push origin fitur-keren-saya`
5. Buka **Pull Request** di GitHub.

```

```