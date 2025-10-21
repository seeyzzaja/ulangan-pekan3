# How To Start #
1. git clone git@github.com:iqbaljlldn/evaluasi_pekan_3.git
2. cd evaluasi_pekan_3
3. git switch -c about-us
4. git pull origin about-us
5. git remote remove origin
6. git remote add origin (url git repositoriy kalian)

# Misi Perbaikan & Peluncuran Ulang Situs Toko Online "TechStore"

### Skenario & Problem Statement

Selamat! Tim Anda adalah sebuah agensi web profesional yang baru saja ditunjuk untuk mengambil alih proyek "TechStore". Proyek ini sebelumnya dikerjakan oleh seorang developer junior, dan hasilnya masih jauh dari standar profesional. Klien melaporkan bahwa websitenya jelek dan mereka khawatir tentang keamanan proyek.

Tugas utama tim Anda adalah melakukan audit total, memperbaiki semua masalah, merapikan repository agar sesuai standar industri, dan mempersiapkan situs ini untuk peluncuran resminya (Versi 1.0).

### Tugas Utama
#### Fase 1: Investigasi & Audit (CLI & Git Forensics)

Sebelum mengubah apapun, tim Anda harus berperan sebagai detektif digital untuk memahami kekacauan yang ada.

1. Analisis Struktur Aset: Gunakan perintah CLI untuk menavigasi dan memetakan struktur file. Identifikasi file mana saja yang lokasinya tidak standar (misalnya, gambar di root folder, bukan di dalam folder assets).

2. Perburuan Bug Visual: Terjadi bug styling css tidak ter-render dengan benar. Analisis dan temukan penyebabnya.

3. Audit Keamanan & Riwayat:
   - Gunakan perintah Git untuk menelusuri riwayat dan temukan commit spesifik di mana file debug.log pertama kali ditambahkan.

   - Di dalam file log tersebut, identifikasi baris pasti yang mengandung informasi sensitif (API Key).

4. Hasil: Buat sebuah file baru bernama AUDIT_REPORT.md di root directory. Di dalam file ini, jelaskan semua temuan Anda dari poin 1, 2, dan 3 dengan format Markdown yang rapi.

#### Fase 2: Perbaikan & Profesionalisasi (Clean-up & Hotfix)

Sekarang saatnya membersihkan kekacauan. Semua pekerjaan di fase ini harus dilakukan di dalam branch baru bernama hotfix-cleanup.

1. Refaktor Struktur Aset: Buat struktur direktori yang logis.Misalnya pindahkan semua file gambar (.png, .jpg) ke dalam folder assets untuk konsistensi. 

2. Perbaiki bug-bug yang anda temukan

3. Commit Profesional: Lakukan commit untuk setiap perubahan besar dengan menggunakan pesan commit yang konvensional dan deskriptif (misal: fix:, refactor:, docs:).

#### Fase 3: Pengembangan Fitur & Kolaborasi

Situs sudah stabil. Saatnya menambahkan fungsionalitas baru dengan alur kerja tim yang benar.

1. Buat Fondasi Baru: Merge branch hotfix-cleanup ke main. Setelah itu, buat branch baru bernama develop dari main. Semua pengembangan fitur baru harus dimulai dari develop.

2. Buat minimal 3 halaman baru lengkap dengan stylenya (minimal "Tentang Kami", "Produk", dan "Kontak"):
   - Buat branch baru untuk membuat halaman" tersebut dari develop.
3. Setelah halaman-halaman baru selesai dibuat, buat PR ke branch develop.

#### Fase 4: Finalisasi
Fitur baru sudah siap di develop. Sekarang saatnya mempersiapkan peluncuran resmi.

1. Penyelesaian Konflik: Buat PR about-us yang terbengkalai itu ke branch develop (merge lewat github). Solve konfliknya jika ada.

2. Integrasi Final: Setelah konflik selesai dan fitur" yang dibuat terintegrasi, Merge branch develop yang sudah lengkap ke main.

