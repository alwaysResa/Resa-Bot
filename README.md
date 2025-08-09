
# Bot WhatsApp Multifungsi oleh RENZY

![Versi](https://img.shields.io/badge/version-2.0.0-blue)
![Fitur](https://img.shields.io/badge/fitur-900%2B-brightgreen)
![Status](https://img.shields.io/badge/status-aktif-brightgreen)
![Lisensi](https://img.shields.io/badge/license-Proprietary-red)

Bot WhatsApp canggih yang dibangun dengan Node.js. Dirancang untuk menjadi cepat, stabil, dan kaya fitur dengan desain yang *user-friendly*. Dengan arsitektur berbasis plugin, bot ini siap memenuhi segala kebutuhan Anda, mulai dari hiburan hingga alat bantu produktivitas.

## 🌟 Keunggulan

* ✅ **900+ Fitur Aktif:** Lebih baik memiliki 900+ fitur yang berjalan sempurna daripada 1000 fitur yang penuh error. 🤭
* 📁 **35+ Submenu Aktif:** Semua menu telah dikelompokkan dengan rapi agar mudah diakses.
* 🎀 **User Friendly:** Desain antarmuka yang lucu, imut, dan mudah digunakan oleh siapa saja.
* ⚡ **Respon Cepat:** Dibangun untuk memberikan respon yang cepat dan stabil, tanpa lemot.
* 💎 **Semi Scrape:** Menggunakan lebih dari 70% metode *scraping* untuk memastikan data dan fungsionalitas fitur selalu akurat.
* 🔒 **Anti Bad Sesi:** Sistem yang lebih stabil untuk mencegah sesi koneksi yang korup atau terputus tiba-tiba.
* 🔄 **GRATIS UPDATE:** Dapatkan pembaruan fitur dan perbaikan secara berkala tanpa biaya tambahan (dengan paket tertentu).

---

## 🏆 Top Fitur

Bot ini dilengkapi dengan fitur-fitur modern dan canggih untuk memberikan pengalaman terbaik.

* ✨ **Artificial Intelligence (AI)**
    Dukungan berbagai model AI untuk kreativitas tanpa batas:
    - `txt2img`: Membuat gambar dari teks.
    - `txt2video`: Membuat video dari teks.
    - `txt2music`: Membuat musik dari teks.
    - `img2text`: Mendeskripsikan isi gambar.
    - ...dan banyak lagi!

* 🎥 **Veo 3 AI Model**
    Gunakan model AI *state-of-the-art* Veo 3 untuk menghasilkan video viral langsung dari WhatsApp.

* 💫 **Tools Produktivitas**
    Berbagai alat untuk mendukung kegiatan sehari-hari Anda:
    - `HD Image`: Meningkatkan resolusi gambar menjadi HD.
    - `Pertajam Gambar/Video`: Membuat media Anda lebih jelas dan tajam.
    - `Hapus Background`: Menghilangkan latar belakang gambar secara otomatis.
    - `Hapus Noise`: Menghilangkan noise pada audio atau media.

* 🌐 **Multi Downloader**
    Fitur *All-in-One Downloader* yang mendukung unduhan dari hampir semua platform media sosial (YouTube, TikTok, Instagram, dll).

* 👾 **Game & RPG**
    Tersedia 50+ game seru yang bisa Anda mainkan bersama teman-teman langsung di grup WhatsApp.

* 😍 **Search Engine**
    Dilengkapi mesin pencari internal untuk menemukan informasi apa pun dengan lebih cepat dan mudah.

* 📆 **Sistem Otomatis**
    Atur jadwal untuk berbagai tugas:
    - `Auto Reminder`: Pengingat otomatis untuk jadwal pribadi atau grup.
    - `Auto Open/Close Group`: Mengatur grup untuk buka/tutup pada waktu yang ditentukan.

* 💓 **Store Support**
    Fitur `Addlist` yang memungkinkan Anda membuat daftar menu atau katalog produk kustom, sangat cocok untuk membantu bisnis online Anda.

---

## 💰 Harga Script

Dapatkan script bot ini dan wujudkan impian Anda sekarang!

| Paket | Harga | Keterangan |
| :--- | :--- | :--- |
| **Paket Lengkap (Free Update)** | ~Rp 150.000~ **Rp 100.000** | Dapatkan script dan semua pembaruan fitur gratis selamanya. |
| **Paket Basic (No Update)** | **Rp 50.000** | Dapatkan script versi saat ini tanpa pembaruan di masa depan. |

---

## 🚀 Cara Menjalankan

### 1. Konfigurasi
Edit file `config.js`. Isi semua informasi yang diperlukan seperti nomor owner, nama bot, dan pengaturan lainnya.

### 2. Menjalankan Bot
Jalankan bot dengan perintah dasar:
```bash
node .
````

Scan kode QR yang muncul di terminal menggunakan WhatsApp Anda, dan bot siap digunakan\!

### 3\. Opsi Lanjutan (Arguments)

Anda dapat menjalankan bot dengan argumen tambahan untuk mengaktifkan mode atau fitur tertentu.
Sintaks: `node . [--options] [<session name>]`
Contoh: `node . --pairing`

| Argumen | Deskripsi |
| :--- | :--- |
| `--pairing` | Menghubungkan perangkat menggunakan kode pairing (lebih aman). |
| `--mobile` | Menghubungkan perangkat via captcha mobile (rawan ban). |
| `--self` | **Mode Self-Host:** Bot hanya bisa digunakan oleh nomor bot & owner. |
| `--pconly` | **Private Chat Only:** Bot hanya merespon di chat pribadi (kecuali user premium). |
| `--gconly` | **Group Only:** Bot hanya merespon di grup (kecuali user premium). |
| `--swonly` | **Status Only:** Bot hanya akan merespon dari status WhatsApp. |
| `--server` | Mode server, cocok untuk deployment di Heroku/Railway atau scan via website. |
| `--restrict` | Mengaktifkan plugin terbatas yang berisiko **BANNED** jika sering digunakan (mis: `add`, `kick`). |
| `--img` | Menampilkan pratinjau gambar yang diterima langsung di terminal. |
| `--autoread` | Bot akan otomatis membaca (centang biru) semua pesan yang masuk. |
| `--autocleartmp` | Otomatis menghapus file-file di dalam folder `tmp` secara berkala. |
| `--nyimak` | **Mode Simak:** Bot tidak merespon, hanya menampilkan pesan di konsol dan menyimpan user ke database. |
| `--test` | **Mode Development:** Untuk keperluan testing oleh developer. |
| `--db <url>` | Terhubung ke database eksternal seperti MongoDB. Jika tidak diisi, akan menggunakan `database.json`. |

-----

## 📂 Struktur Direktori Bot

Proyek ini disusun dengan struktur folder yang jelas untuk memisahkan setiap komponen sesuai fungsinya.

```
.
├── backend/
├── lib/
├── media/
├── plugins/
├── src/
├── views/
├── config.js
├── database.json
├── Dockerfile
├── handler.js
├── index.js
├── package.json
└── ...
```

-----

## 📞 Kontak

Tertarik? Hubungi saya untuk pembelian dan informasi lebih lanjut\!

  * **Owner:** [Hubungi via WhatsApp](https://wa.me/6285117070328)

Dibuat dengan ❤️ oleh **RENZY**.
