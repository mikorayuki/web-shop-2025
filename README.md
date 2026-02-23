<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Web%20Shop%202025&fontSize=50&animation=fadeIn" width="100%" alt="Header Web Shop 2025">
  
  <h1>🛒 Web Shop 2025</h1>
  <p><i>Platform E-Commerce Modern, Dinamis & Responsif</i></p>

  <p>
    <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge&logo=github" alt="Status">
    <img src="https://img.shields.io/badge/Version-1.0.0-blue?style=for-the-badge" alt="Version">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License MIT">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  </p>
</div>

---

<details>
  <summary><b>📑 Daftar Isi</b></summary>
  <ol>
    <li><a href="#-tentang-project">Tentang Project</a></li>
    <li><a href="#-fitur-utama">Fitur Utama</a></li>
    <li><a href="#-teknologi-yang-digunakan">Teknologi yang Digunakan</a></li>
    <li><a href="#-susunan-project">Susunan Project</a></li>
    <li><a href="#-prasyarat-instalasi">Prasyarat Instalasi</a></li>
    <li><a href="#-cara-instalasi--menjalankan">Cara Instalasi & Menjalankan</a></li>
    <li><a href="#-contoh-penggunaan">Contoh Penggunaan</a></li>
    <li><a href="#-kontribusi">Kontribusi</a></li>
  </ol>
</details>

---

## 📖 Tentang Project

**Web Shop 2025** adalah platform e-commerce statis yang dirancang untuk menjadi ringan, cepat, dan mudah dikelola. Proyek ini sangat cocok untuk toko online skala kecil menengah atau sebagai portofolio web developer. 

Keunggulan utama dari proyek ini adalah **tidak memerlukan database backend yang rumit**. Semua data toko, kategori, dan produk dikelola sepenuhnya dan dinamis melalui satu buah file JSON (`shop-data.json`).

> 📸 **Screenshot Tampilan** > *(Tambahkan gambar screenshot project kamu di sini nantinya)* > `<img src="link-gambar-screenshot.jpg" alt="Preview Web Shop" width="800">`

## ✨ Fitur Utama

- 🛍️ **Katalog Produk Dinamis:** Menampilkan daftar produk yang di-generate secara otomatis dari file JSON.
- 📱 **Desain Super Responsif:** Tampilan menyesuaikan secara mulus di layar Desktop, Tablet, maupun Smartphone.
- 🔍 **Pencarian & Filter Kategori:** Fitur pencarian produk *real-time* dan penyaringan berdasarkan kategori.
- 🖼️ **Pop-up Detail Produk (Modal):** Pengguna dapat melihat detail lengkap produk tanpa harus memuat ulang atau berpindah halaman.
- ⚙️ **Manajemen Tanpa Coding:** Tambah, edit, atau hapus produk cukup dengan mengubah teks di file konfigurasi.
- ⚡ **Performa Tinggi:** Memuat halaman secara instan tanpa waktu tunggu respon dari server database.

## 🛠️ Teknologi yang Digunakan

Proyek ini dibangun murni menggunakan teknologi web standar tanpa *framework* yang berat:

- **HTML5** untuk semantik dan struktur halaman.
- **CSS3 (Vanilla)** dengan penerapan *Custom Properties (Variables)* untuk tema.
- **JavaScript (ES6+)** untuk logika DOM, Fetch API, dan interaktivitas.
- **FontAwesome 6** untuk ikon UI.
- **Animate.css** untuk animasi transisi halaman yang halus.
- **Google Fonts** (Poppins & Montserrat) untuk tipografi modern.

## 📂 Susunan Project

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
📋 Prasyarat Instalasi
Karena proyek ini menggunakan fitur Fetch API JavaScript untuk memuat file shop-data.json, Anda tidak bisa membukanya hanya dengan klik ganda file index.html di browser (akan terkena pemblokiran aturan CORS).
Anda memerlukan Local Web Server untuk menjalankannya. Beberapa opsi yang bisa digunakan:
 * Ekstensi Live Server di Visual Studio Code.
 * Ekstensi Web Server for Chrome.
 * Python (jalankan python -m http.server di terminal).
 * Node.js (install modul seperti http-server atau live-server).
🚀 Cara Instalasi & Menjalankan
 * Clone repository ini ke komputer/HP Anda:
   ```bash
   git clone [https://github.com/mikorayuki/web-shop-2025.git](https://github.com/mikorayuki/web-shop-2025.git)
   ```
 * Masuk ke direktori project:
 ```bash
   cd web-shop-2025
 ```
 * Jalankan local server (Contoh menggunakan Python):
   python -m http.server 8000

 * Buka browser dan akses alamat: http://localhost:8000
💡 Contoh Penggunaan
Untuk mengubah nama toko, kontak, atau menambah produk, Anda hanya perlu mengedit file shop-data.json.
Contoh Menambah Produk Baru: Buka shop-data.json, lalu pada bagian array "products", tambahkan objek produk baru seperti ini:
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
Catatan: Pastikan categoryId cocok dengan ID yang ada di dalam daftar "categories". Untuk panduan lebih lengkap, buka file panduan.html di browser Anda.
🤝 Kontribusi
Kontribusi sangat dipersilakan! Jika Anda ingin memperbaiki bug, menambah fitur, atau meningkatkan tampilan:
 * Lakukan Fork pada repository ini.
 * Buat branch fitur baru Anda: git checkout -b fitur-keren-saya
 * Lakukan commit perubahan Anda: git commit -m 'Menambahkan fitur keren'
 * Push ke branch tersebut: git push origin fitur-keren-saya
 * Buka Pull Request di GitHub.

<div align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%" height="3px">
  <br/>
  <table>
    <tr>
      <td align="center" style="border:none;">
        <h3>✨ Attribution & Development</h3>
        <p>Project ini telah dikembangkan kembali (<b>Redeveloped</b>) dengan penuh dedikasi.</p>
        
        <a href="https://mikorayuki.my.id">
          <img src="https://img.shields.io/badge/Developed%20By-Mikorayuki-FF69B4?style=for-the-badge&logo=rocket&logoColor=white" alt="Mikorayuki Badge">
        </a>
        <p><i>"Based on an Open Source project with significant UI/UX improvements and performance optimization."</i></p>
        <br/>
        <a href="https://mikorayuki.my.id" target="_blank">
          <img src="https://img.shields.io/badge/🌐_Visit_My_Website-mikorayuki.my.id-blue?style=flat-square" alt="Website">
        </a>
      </td>
    </tr>
  </table>
  <br/>
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=30&section=footer" width="100%">
</div>
