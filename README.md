🌿 Smart Lapor
**Aplikasi Mobile Pelaporan Masalah Lingkungan & Fasilitas Publik Lokal**
**Smart Lapor** adalah aplikasi Android yang dirancang untuk memfasilitasi masyarakat
dalam melaporkan kerusakan lingkungan maupun fasilitas publik di sekitar mereka secara cepat dan terstruktur. 
Aplikasi ini juga menyediakan alur pemantauan status dan tindak lanjut yang transparan
antara masyarakat sebagai pelapor dan admin/petugas sebagai pengelola.

# Laporan Riwayat Perubahan

**Proyek:** Smart Lapor (Aplikasi Pelaporan Masalah Lingkungan & Ekosistem Lokal)

**Navigasi:** [SRS Revision History](#-srs-revision-history) | [Week 1](#-week-1) | [Week 2](#-week-2) | [Week 3](#-week-3)

---

## 📄 SRS Revision History

Riwayat revisi dokumen **Software Requirement Specification (SRS)** proyek Smart Lapor:

| Date | Version | Description | Author(s) |
| :--- | :--- | :--- | :--- |
| 13/11/2026 | 0.1 | Draft Version inisialisasi dokumen SRS, penentuan konsep, serta penyusunan Bab 1.1 (*Purpose*) | Bilkis Qilatusshakila |
| 20/11/2026 | 0.2 | Penyelesaian Bab 1 (*Introduction*): penambahan 1.2 *Document Conventions*, 1.3 *Intended Audience and Reading Suggestions*, 1.4 *Project Scope*, 1.5 *References*, dan 1.6 *Acronyms and Abbreviations* | Bilkis aQilatusshakila |
| 24/11/2026 | 0.3 | Penyelesaian SRS Bab 3 (*Functional Requirements*), Bab 4 (*External Interfaces*), dan Bab 5 (*Nonfunctional Requirements*); perancangan ERD Notasi Chen; serta revisi *Activity Diagram* | Bilkis Qilatusshakila |
| 25/11/2026 | 0.4 | Penyelesaian SRS Bab 6 (*Other Requirements* / Lampiran) | Bilkis Qilatusshakila |

## 📌 Week 1

### Ringkasan Eksekutif Week 1

Pada Week 1, pengerjaan proyek **Smart Lapor** berfokus pada perancangan konsep awal dan inisialisasi dokumentasi SRS:

1. **Perancangan Konsep Aplikasi:** Penentuan tema Lingkungan & Sosial, pemetaan 4 entitas data utama (*User, Category, Report, Response*), dan perancangan 5 modul CRUDS wajib.
2. **Penyusunan SRS Bab 1.1 (*Purpose*):** Penulisan latar belakang, gambaran ruang lingkup sistem, dan tujuan penyusunan dokumen SRS.
3.**Konvensi Dokumen (1.2 *Document Conventions*):** Penetapan aturan penomoran hierarkis, kode identifikasi kebutuhan (`REQ-FUN` dan `REQ-NF`), serta standar format penulisan istilah teknis.
4. **Target Pembaca (1.3 *Intended Audience and Reading Suggestions*):** Pemetaan sasaran pembaca dokumen (Dosen Pengampu, Asisten Praktikum, dan Pengembang Aplikasi) beserta panduan urutan pembacaan.
## 📌 Week 2

### Ringkasan Eksekutif Week 2

Pada Week 2, pengerjaan proyek **Smart Lapor** berfokus pada penyelesaian dokumen **SRS Bab 1 (*Introduction*)** serta penyelarasan ruang lingkup fitur dengan persyaratan proyek akhir:

1. **Ruang Lingkup Proyek (1.4 *Project Scope*):** Penjabaran spesifikasi teknis (Kotlin, Jetpack Compose, MVVM, REST API, MySQL/PostgreSQL), sistem autentikasi JWT & *Role-Based UI*, 4 entitas utama (*User, Category, Report, Response*), 5 modul CRUDS penuh, dan fitur *Local File Storage*.
2. **Referensi & Akronim (1.5 *References* & 1.6 *Acronyms and Abbreviations*):** Pencantuman daftar acuan standar (IEEE 830, dokumentasi Android/Compose, RFC JWT) serta tabel daftar singkatan teknis.
3. **Dokumentasi Repositori:** Pembaruan `README.md` untuk pencatatan riwayat revisi SRS dan progres mingguan.
4. **Inisialisasi Proyek & Repositori:** Pembuatan repositori GitHub proyek **Smart Lapor** (`Initial commit`).
5. **Perancangan Konsep Aplikasi:** Penentuan tema Lingkungan & Sosial, pemetaan 4 entitas data utama (*User, Category, Report, Response*), dan perancangan 5 modul CRUDS wajib.

### 📜 Daftar Riwayat Commit (Week 2)
| No | Hash Commit | Pesan Commit |
| :--- | :--- | :--- |
| 1 | `d76d821` | `Initial commit` |

## 📌 Week 3

### Ringkasan Eksekutif Week 3

Pada Week 3, pengerjaan proyek **Smart Lapor** berfokus pada penyelesaian dokumen **SRS Bab 3, Bab 4, dan Bab 5** serta penyempurnaan perancangan diagram sistem sesuai arahan asisten praktikum:

1. **Penyusunan SRS Bab 3 (*Functional Requirements*):** Penjabaran lengkap kebutuhan fungsional seluruh fitur peran Masyarakat dan Admin (3.1 – 3.6) beserta alur logika sistem.
2. **Penyusunan SRS Bab 4 (*External Interfaces*):** Pendefinisian antarmuka perangkat keras, perangkat lunak, dan antarmuka komunikasi (REST API, JSON, JWT, HTTPS/TLS).
3. **Penyusunan SRS Bab 5 (*Nonfunctional Requirements*):** Penyelesaian kebutuhan *Performance*, *Safety*, *Security* (kebijakan *password* `bcrypt`, proteksi *SQL Injection*, kerahasiaan `.env`, RBAC 403), serta *Software Quality Attributes*.
4. **Perancangan ERD (Notasi Chen):** Pembuatan *Entity Relationship Diagram* menggunakan Notasi Chen yang mencakup entitas `users`, `categories`, `reports`, `responses`, dan `announcements`.
5. **Revisi *Activity Diagram*:** Penyesuaian *Activity Diagram* (Registrasi, Login & *Role-Based UI*, Verifikasi & Ubah Status Laporan) dengan pola interaksi timbal balik antar *swimlane*, penyatuan satu *Final Node* (`End`), alur otomatis ke Beranda pasca-registrasi, serta pemecahan *Activity Diagram* Kelola Tanggapan (Admin) menjadi 4 diagram CRUD terpisah (`GET`, `POST`, `PUT`, `DELETE`).
6. 6. **Penyusunan SRS Bab 6 (*Other Requirements*):** Penyelesaian bagian akhir dokumen SRS beserta kelengkapan lampiran dokumentasi.

### 📜 Daftar Riwayat Commit (Week 3)

| No | Hash Commit | Pesan Commit |
| --- | --- | --- |
| 1 | `isi-hash` | `docs: update SRS Bab 3-5, ERD, dan revisi Activity Diagram` |
| 2 | `isi-hash-2` | `docs: tambah SRS Bab 6` |
