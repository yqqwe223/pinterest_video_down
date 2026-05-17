# Alat Informasi Video Pinterest 🎬

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-1.0.0-green.svg)](https://twittervideodownloaderx.com/pinterest_downloader_in)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen)](https://twittervideodownloaderx.com/pinterest_downloader_in)

> ⚠️ **Penting**: Proyek ini dirancang khusus untuk tujuan pendidikan dan penelitian. Harap selalu patuhi [Ketentuan Penggunaan Pinterest](https://policy.pinterest.com/id-id/terms-of-service) serta undang-undang hak cipta yang berlaku di yurisdiksi Anda.

---

## 📋 Deskripsi Proyek

**Alat Informasi Video Pinterest** adalah aplikasi web ringan yang dikembangkan untuk menganalisis dan mengakses metadata dari konten video yang **dapat diakses secara publik** di platform Pinterest. Alat ini membantu pengguna, peneliti, dan pengarsip digital dalam memperoleh informasi teknis mengenai video—seperti judul, deskripsi, durasi, resolusi yang tersedia, informasi pembuat konten, dan tanggal publikasi—tanpa mengganggu infrastruktur platform atau melewati mekanisme keamanan apa pun.

### ✨ Fitur Utama

- 🔍 **Analisis URL**: Dukungan untuk memasukkan tautan video Pinterest yang dapat diakses publik (Pin dan Idea Pin) guna mengakses metadata terkait
- 📊 **Tampilan Metadata**: Penyajian jelas mengenai judul, deskripsi, durasi, resolusi tersedia, informasi pembuat, dan stempel waktu publikasi
- 🌐 **Antarmuka Bahasa Indonesia**: Dukungan penuh bahasa Indonesia dengan desain UI/UX profesional dan mudah dipahami untuk pengguna di Indonesia dan komunitas berbahasa Indonesia di seluruh dunia
- 📱 **Desain Responsif**: Pengalaman pengguna yang optimal di perangkat desktop, tablet, dan ponsel pintar
- ⚡ **Pemrosesan Efisien**: Validasi sisi klien dikombinasikan dengan komunikasi API yang dioptimalkan untuk waktu respons cepat
- 🔒 **Privitas Diutamakan**: Tidak ada penyimpanan data pengguna, riwayat kueri, atau konten video pada tahap apa pun

---

## 🚀 Memulai dengan Cepat

### Penggunaan Online (Direkomendasikan)

Akses langsung antarmuka web kami—tanpa perlu instalasi:

👉 [https://twittervideodownloaderx.com/pinterest_downloader_in](https://twittervideodownloaderx.com/pinterest_downloader_in)

### Implementasi Lokal (Untuk Pengembang)

```bash
# Klon repositori
git clone https://github.com/NamaPengguna/pinterest-video-info.git
cd pinterest-video-info

# Instal dependensi (contoh untuk versi Node.js)
npm install

# Jalankan server pengembangan
npm run dev
```

> 💡 Catatan: Implementasi lokal hanya direkomendasikan untuk tujuan penelitian teknis dan pembelajaran. Untuk penggunaan produksi, kami menyarankan layanan hosting resmi.

---

## 🛠️ Stack Teknologi

| Komponen | Teknologi |
|----------|-----------|
| Frontend | HTML5 + CSS3 + Vanilla JavaScript / React (opsional) |
| Backend | Python Flask / Node.js Express (dapat dikonfigurasi) |
| Komunikasi API | Permintaan HTTPS RESTful dengan rotasi User-Agent yang sesuai |
| Implementasi | Hosting file statis / Kompatibel dengan arsitektur serverless |
| Lisensi | Lisensi MIT |

---

## 📖 Panduan Penggunaan

1. Salin URL video atau Idea Pin Pinterest yang **dapat diakses secara publik**
2. Tempelkan URL ke dalam kolom input pada antarmuka web alat ini
3. Klik "Analisis" untuk mengambil metadata yang tersedia
4. Gunakan informasi yang ditampilkan sebagai referensi pribadi, untuk penelitian akademis, kurasi konten, atau pengelolaan media digital yang sesuai dengan peraturan

> ⚠️ Alat ini hanya berfungsi dengan konten yang dapat diakses secara publik tanpa memerlukan autentikasi. Pin yang dilindungi oleh pengaturan privasi, memerlukan login, atau dibatasi untuk grup pengguna tertentu tidak dapat diproses karena keterbatasan teknis dan persyaratan kepatuhan regulasi.

---

## ⚖️ Pernyataan Kepatuhan dan Batasan Penggunaan

Proyek ini mematuhi prinsip-prinsip berikut secara ketat:

- ✅ Menghormati pedoman `robots.txt` dan kebijakan crawler Pinterest
- ✅ Hanya memproses metadata yang dapat diakses secara publik tanpa memerlukan autentikasi
- ✅ Tidak menyimpan dalam cache, meneruskan, atau menyimpan file video maupun data perilaku pengguna
- ✅ Dibatasi pada skenario penelitian non-komersial: pendidikan, studi akademis, humaniora digital, analisis konten
- ✅ Tidak menyediakan fungsionalitas untuk melewati kontrol izin platform atau mekanisme keamanan

**Penting**: Pengguna bertanggung jawab penuh untuk memastikan bahwa penggunaan mereka mematuhi hukum yang berlaku (termasuk regulasi hak cipta dan perlindungan data pribadi) serta Ketentuan Layanan Pinterest. Pengembang alat ini tidak bertanggung jawab atas penyalahgunaan atau penggunaan yang tidak sesuai.

---

## 🤝 Cara Berkontribusi

Kontribusi dari komunitas sangat kami sambut! Sebelum mengirimkan Pull Request, ikuti langkah-langkah berikut:

1. Fork repositori ke akun pribadi Anda
2. Buat branch untuk fitur Anda: `git checkout -b feat/nama-fitur-anda`
3. Commit perubahan Anda: `git commit -m 'feat: deskripsi fitur Anda'`
4. Push branch tersebut: `git push origin feat/nama-fitur-anda`
5. Buka Pull Request di GitHub dengan deskripsi perubahan yang jelas dan rekomendasi pengujian

> 📌 Untuk perubahan besar, kami menyarankan untuk mendiskusikannya terlebih dahulu melalui Issues guna memastikan keselarasan arah teknis dan persyaratan kepatuhan.

---

## ❓ Pertanyaan yang Sering Diajukan

**T: Apakah penggunaan alat ini gratis?**  
J: Ya, sepenuhnya gratis. Proyek ini dirilis di bawah lisensi sumber terbuka MIT, dan kami menyambut penggunaan yang sah dan sesuai untuk pembelajaran serta penelitian.

**T: Apakah file video disimpan sementara di server?**  
J: Tidak. Seluruh proses murni berupa kueri metadata; tidak ada file media yang ditransmisikan, disimpan dalam cache, atau disimpan pada tahap apa pun.

**T: Apakah alat ini mendukung Pin pribadi atau Idea Pin dengan pembatasan akses?**  
J: Tidak. Karena alasan kelayakan teknis dan kepatuhan hukum, hanya konten yang sepenuhnya publik yang didukung.

**T: Apakah dokumentasi API tersedia untuk integrasi?**  
J: Spesifikasi API internal dapat disediakan sebagai materi referensi teknis atas permintaan resmi dari institusi akademis atau penelitian yang terakreditasi. Silakan hubungi tim pemeliharaan untuk detail lebih lanjut.

**T: Apakah alat ini berfungsi dengan semua format video Pinterest?**  
J: Alat ini mendukung format video publik yang umum di Pinterest, termasuk Pin standar dan Idea Pin. Format baru terus dievaluasi dan diintegrasikan ketika memungkinkan secara teknis.

---

## 📄 Lisensi

Proyek ini didistribusikan di bawah **Lisensi MIT**. Lihat file [LICENSE](LICENSE) untuk ketentuan lengkap penggunaan dan redistribusi.

---

## 🙏 Ucapan Terima Kasih

- Kepada komunitas sumber terbuka atas inspirasi teknis dan komponen fundamental
- Kepada semua kontributor yang meluangkan waktu untuk meningkatkan keamanan dan stabilitas proyek ini
- Kepada pendidik, peneliti, dan kurator konten yang menjelajahi alat ini dalam kerangka kerja yang sah dan sesuai

---

## 🔗 Tautan Berguna

- 📘 [Panduan Pengembang Pinterest](https://developers.pinterest.com/)
- ⚖️ [Ketentuan Penggunaan Pinterest](https://policy.pinterest.com/id-id/terms-of-service)
- 🔐 [Kebijakan Privasi Pinterest](https://policy.pinterest.com/id-id/privacy-policy)
- 🤖 [robots.txt Pinterest](https://www.pinterest.com/robots.txt)

---

> 🌐 **Alat Online**: [https://twittervideodownloaderx.com/pinterest_downloader_in](https://twittervideodownloaderx.com/pinterest_downloader_in)  
> 🐛 **Laporkan Masalah**: [Issues](https://github.com/NamaPengguna/pinterest-video-info/issues)  
> 💡 **Ajukan Fitur**: [Discussions](https://github.com/NamaPengguna/pinterest-video-info/discussions)

---

*Dikembangkan dengan ❤️ untuk komunitas pengembang berbahasa Indonesia dan ekosistem penelitian akademis*