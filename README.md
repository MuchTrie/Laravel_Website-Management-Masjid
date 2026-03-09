```
███╗   ███╗ █████╗ ███████╗     ██╗██╗██████╗ 
████╗ ████║██╔══██╗██╔════╝     ██║██║██╔══██╗
██╔████╔██║███████║███████╗     ██║██║██║  ██║
██║╚██╔╝██║██╔══██║╚════██║██   ██║██║██║  ██║
██║ ╚═╝ ██║██║  ██║███████║╚█████╔╝██║██████╔╝
╚═╝     ╚═╝╚═╝  ╚═╝╚══════╝ ╚════╝ ╚═╝╚═════╝ 
   ╔══════════════════════════════════════════╗
   ║    Sistem Manajemen Masjid Al-Ikhlas    ║
   ╚══════════════════════════════════════════╝
```

<div align="center">

**Sistem manajemen terintegrasi untuk masjid — dibangun dengan Laravel 12**

![Laravel](https://img.shields.io/badge/Laravel-12-FF2D20?style=flat-square&logo=laravel)
![PHP](https://img.shields.io/badge/PHP-8.2+-777BB4?style=flat-square&logo=php)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat-square&logo=mysql)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?style=flat-square&logo=bootstrap)

</div>

---

## 📚 Panduan Instalasi

- 📖 **[PANDUAN_INSTALASI_DAN_PENGGUNAAN.md](PANDUAN_INSTALASI_DAN_PENGGUNAAN.md)** — Panduan step-by-step lengkap dengan troubleshooting
- ⚡ **[QUICK_START.md](QUICK_START.md)** — Panduan cepat untuk yang sudah familiar dengan Laravel

---

## ✨ Modul & Fitur

| Modul | Deskripsi |
|-------|-----------|
| 📅 **Event Management** | Kelola event, approval DKM, pendaftaran peserta, status draft/published/cancelled |
| 📦 **Inventaris / Aset** | Manajemen aset, jadwal & laporan perawatan, QR Code tracking, archive |
| 👥 **Kegiatan & Donasi** | Kegiatan masjid, program donasi, tracking donatur, kategori jamaah |
| 🐑 **Program Kurban** | Pendaftaran hewan kurban, dokumentasi, riwayat kurban |
| 💰 **ZIS Management** | Zakat, Infaq, Shadaqah — data muzakki, mustahik, dan penyaluran |
| 🕌 **Manajemen Takmir** | Struktur organisasi, jabatan, jadwal tugas, riwayat jabatan |
| 🕐 **Jadwal Sholat** | Integrasi API jadwal sholat real-time |
| 📊 **Dashboard Unified** | Statistik terintegrasi dari semua modul |

---

## 🔐 Login Credentials

| Role | Username | Password | Akses |
|------|----------|----------|-------|
| Admin | `admin` | `admin123` | Full access semua modul |
| DKM | `dkm` | `dkm123` | Approval & management |
| Panitia | `Hasan` | `panitia123` | Buat event & kegiatan |
| Jemaah | `jamaah` | `jamaah123` | Lihat & daftar event/kegiatan |

---

## 🚀 Instalasi

### 1. Install Dependencies
```bash
composer install
npm install
```

### 2. Setup Environment
```bash
cp .env.example .env
php artisan key:generate
```

### 3. Konfigurasi Database
Edit `.env` sesuai konfigurasi database, lalu:
```bash
php artisan migrate
php artisan db:seed
```

### 4. Jalankan Aplikasi
```bash
php artisan serve
npm run dev
```

Buka browser: `http://127.0.0.1:8000`

---

## 📂 Struktur Modul

```
├── 📅 Event Management
│   ├── Events, Sessions, Participants
│   └── Approval workflow (Panitia → DKM/Admin)
│
├── 📦 Inventaris / Aset
│   ├── Aset & QR Code tracking
│   ├── Jadwal & Laporan Perawatan
│   └── Log Aktivitas & Archive
│
├── 👥 Kegiatan & Donasi
│   ├── Kategori Jamaah & Kegiatan
│   └── Program Donasi & Riwayat Donasi
│
├── 🐑 Program Kurban
│   └── Pendaftaran & Dokumentasi Kurban
│
├── 💰 ZIS Management
│   └── Muzakki, Mustahik, ZIS Masuk, Penyaluran
│
└── 🕌 Manajemen Takmir
    ├── Struktur Organisasi & Jabatan
    └── Jadwal Tugas & Riwayat Jabatan
```

---

## 🎯 Role & Permission

| Role | Akses |
|------|-------|
| 🔴 **Admin** | Full access — kelola users, semua modul, log aktivitas |
| 🟠 **DKM** | Approve event, kelola kegiatan, donasi, inventaris |
| 🟡 **Panitia** | Buat & edit event sendiri, lihat kegiatan |
| 🟢 **Jemaah** | Lihat & daftar event/kegiatan, submit & lihat riwayat donasi |

---

## 🛠️ Tech Stack

| Komponen | Teknologi |
|----------|-----------|
| Framework | Laravel 12 |
| Language | PHP 8.2+ |
| Database | MySQL / MariaDB |
| Frontend | Bootstrap (SB Admin 2), Tailwind CSS |
| Build Tool | Vite |
| Icons | Font Awesome |
| PDF Export | DomPDF |
| QR Code | Simple QR Code |
| API | Jadwal Sholat (MyQuran) |

---

## ✅ Status Integrasi

| Modul | Status |
|-------|--------|
| Event Management | ✅ Terintegrasi |
| Inventaris / Aset | ✅ Terintegrasi |
| Kegiatan Masjid | ✅ Terintegrasi |
| Program Donasi | ✅ Terintegrasi |
| Program Kurban | ✅ Terintegrasi |
| ZIS Management | ✅ Terintegrasi |
| Manajemen Takmir | ✅ Terintegrasi |
| Jadwal Sholat (API) | ✅ Terintegrasi |
| Dashboard Unified | ✅ Terintegrasi |
| Role-Based Access | ✅ Terintegrasi |
| Export PDF | ✅ Terintegrasi |

---

## 📖 Dokumentasi

- 📖 **[PANDUAN_INSTALASI_DAN_PENGGUNAAN.md](PANDUAN_INSTALASI_DAN_PENGGUNAAN.md)** — Panduan instalasi & penggunaan lengkap
- ⚡ **[QUICK_START.md](QUICK_START.md)** — Quick start guide
- 📋 **[INTEGRASI_LENGKAP.md](INTEGRASI_LENGKAP.md)** — Dokumentasi teknis lengkap (struktur DB, routes, integrasi modul)

---

<div align="center">
  <sub>Dibuat dengan ❤️ untuk Masjid Al-Ikhlas &nbsp;·&nbsp; Laravel 12 &nbsp;·&nbsp; 2025</sub>
</div>
