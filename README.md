# MeowCare

## Aplikasi Manajemen Penitipan & Grooming Kucing Berbasis Android

MeowCare merupakan aplikasi Android yang dirancang untuk membantu pengelolaan operasional usaha penitipan dan grooming kucing. Aplikasi ini berfokus pada pengelolaan data pelanggan, profil kucing, layanan, reservasi, serta pencatatan kondisi dan aktivitas kucing selama masa penitipan.

Proyek ini dikembangkan sebagai tugas akhir mata kuliah **Pengembangan Aplikasi Mobile (PAM)**.

## Tujuan

- Mempermudah pengelolaan data pelanggan dan kucing.
- Mengorganisir informasi layanan grooming dan penitipan.
- Membantu pencatatan dan pemantauan reservasi.
- Mendokumentasikan kondisi dan aktivitas kucing selama masa penitipan.
- Menyediakan pengelolaan data yang terstruktur melalui aplikasi Android.

## Ruang Lingkup

MeowCare ditujukan untuk penggunaan operasional oleh satu Pemilik akun. Pelanggan dicatat sebagai data di dalam aplikasi dan tidak memiliki akun atau akses aplikasi.

Data operasional utama dikelola melalui backend dan database cloud. Catatan Harian beserta foto opsionalnya disimpan sebagai file lokal pada perangkat Android.

## Fitur Utama

| Fitur | Deskripsi | Status |
|---|---|---|
| Autentikasi & Profil | Registrasi, login, pengelolaan sesi token, dan profil Pemilik | Direncanakan |
| Manajemen Pelanggan | Tambah, lihat, ubah, hapus, dan cari data pelanggan | Direncanakan |
| Manajemen Hewan | Mengelola profil kucing yang terhubung dengan pelanggan | Direncanakan |
| Manajemen Layanan | Mengelola layanan grooming dan penitipan beserta tarif | Direncanakan |
| Manajemen Reservasi | Mengelola reservasi, status, pencarian, dan perhitungan total biaya | Direncanakan |
| Catatan Harian | Mencatat kondisi dan aktivitas kucing per tanggal serta foto opsional secara lokal | Direncanakan |

Fitur CRUDS mencakup Create, Read, Update, Delete, dan Search (Tambah, Lihat, Ubah, Hapus, dan Cari).

## Teknologi

### Aplikasi Android
- Kotlin
- Jetpack Compose
- Material 3
- Navigation Compose
- MVVM Architecture
- StateFlow

### Backend dan Database
- Node.js
- Express
- REST API
- JSON
- PostgreSQL (cloud)
- Supabase

### Autentikasi
- JWT Access Token
- JWT Refresh Token

### Penyimpanan Lokal
- File lokal Android untuk Catatan Harian dan foto terkait

## Gambaran Arsitektur

MeowCare direncanakan menggunakan arsitektur yang memisahkan aplikasi Android, backend REST API, dan database cloud.

- **Android Application:** menangani antarmuka, navigasi, state, validasi input, komunikasi API, dan file lokal.
- **Backend REST API:** menangani request, validasi, autentikasi, otorisasi, dan operasi data.
- **Cloud Database:** menyimpan data akun serta data operasional yang terhubung.
- **Local Storage:** menyimpan Catatan Harian dan foto dokumentasi pada perangkat.

Operasi data cloud membutuhkan koneksi internet. Backend membatasi akses data berdasarkan identitas akun Pemilik yang terautentikasi.

## Gambaran Data

MeowCare direncanakan memiliki entitas utama berikut:

| Entitas | Keterangan |
|---|---|
| User | Data akun Pemilik |
| Pelanggan | Informasi pelanggan |
| Hewan | Profil kucing yang terhubung dengan pelanggan |
| Layanan | Data layanan grooming atau penitipan |
| Reservasi | Catatan penggunaan layanan oleh seekor kucing |
| Catatan Harian | Dokumentasi kondisi dan aktivitas kucing yang disimpan lokal |

## Dokumentasi

- [Software Requirements Specification (SRS)](docs/SRS.md) — akan disusun

## Progres Pengembangan

Proyek saat ini berada pada tahap inisialisasi repository dan perencanaan kebutuhan.

| Tahapan | Status |
|---|---|
| Inisialisasi repository GitHub | Selesai |
| README | Selesai (perlu pembaruan progres berkala) |
| Penyusunan SRS | Draft v0.3; kebutuhan dan analysis models sedang ditinjau |
| Analisis dan desain sistem | Analysis models awal tersedia di Appendix B SRS |
| Perancangan database | Belum dimulai |
| UI/UX Design | Belum dimulai |
| Pengembangan Android dan backend | Belum dimulai |
| Pengujian | Belum dimulai |

### Catatan Progres Mingguan

Progres akan diperbarui berdasarkan pekerjaan yang benar-benar dilakukan dan dicatat melalui commit repository.

- **21 November 2026:** Inisialisasi repository dan penyusunan dokumentasi awal proyek.

## Informasi Proyek

| Informasi | Detail |
|---|---|
| Nama Proyek | MeowCare |
| Platform | Android |
| Mata Kuliah | Pengembangan Aplikasi Mobile (PAM) |
| Pengembang | Aurelia Citra Pangukir |
| NIM | 20240140240 |
| Status | Perencanaan dan analisis kebutuhan |

---

*MeowCare — Mempermudah Pengelolaan Penitipan dan Grooming Kucing.*
