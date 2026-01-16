# 🚀 QC-Tools 2025: Markas Rahasia BPH QC

## Introduction
Selamat datang di repositori resmi Google Colab QC 2025! Tempat di mana data maba yang berantakan disulap menjadi laporan rapi tanpa perlu menguras air mata (dan kuota).

## 💌 Pesan Spesial dari Sesepuh
"Halo Rek! Selamat ya sudah resmi terpilih menjadi BPH QC yang baru! 🎉 Semoga amanah dalam menjalankan tugas, tetap solid sebagai tim, dan yang paling penting... ENJOY prosesnya kedepannya! Jangan lupa istirahat di sela-sela rekap data ya! 😂"

– Vqhyi & Qjybq ❤️

---

## 🚀 Cara Penggunaan Singkat
1. Buka file .ipynb yang ingin kamu gunakan di repositori ini.
2. Klik tombol "Open in Colab" di bagian atas (jika tersedia).
3. Jalankan sel kode dengan menekan tombol Play atau Ctrl + F9.
4. Ikuti instruksi di bawah ini untuk setiap alatnya.

---

## 🛠️ Panduan Detail Alat (Senjata Rahasia)

### 📂 1. Program Clustering Maba.ipynb
**Alias:** Si Pembagi Nasib Adil ⚖️
**Fungsi:** Membagi ribuan mahasiswa baru ke dalam 25 Cluster dan kelompok kecil dengan komposisi Program Studi dan Jenis Kelamin yang seimbang (Stratified).

* **Persiapan Data:**
    * Siapkan 1 file (Excel/CSV) data seluruh mahasiswa.
    * **Wajib ada kolom:** `STATUS AKTIF`, `PROGRAM STUDI`, `JENIS KELAMIN`, `NIM`, `NAMA`, `NO HP`.
    * Pastikan `STATUS AKTIF` berisi "Terdaftar" untuk mahasiswa yang akan diproses.
* **Cara Menggunakan:**
    1.  Jalankan program dan klik tombol upload.
    2.  Pilih file data mahasiswa.
    3.  Program otomatis memfilter status "Terdaftar" dan membagi ke 25 Cluster (tiap cluster dibagi lagi jadi 4 Kelompok).
    4.  Hasil otomatis terunduh dengan nama: `pembagian_kelompok_final.csv`.

### 🌀 2. Program Kelompok Fusion.ipynb
**Alias:** Si Pengaduk Prodi (Anti-Ansos) 🧪
**Fungsi:** Membuat kelompok lintas jurusan ("Fusion") dalam setiap Cluster. Satu kelompok dijamin berisi prodi yang berbeda-beda.

* **Persiapan Data:**
    * Siapkan file CSV (biasanya hasil output dari Program No. 1).
    * **Wajib ada kolom:** `CLUSTER`, `NIM`, `NAMA`, `PROGRAM STUDI`.
* **Cara Menggunakan:**
    1.  Jalankan program dan upload file CSV.
    2.  Sistem akan mendeteksi jumlah mahasiswa per cluster (Normalnya 40-41 orang dibagi 14 kelompok).
    3.  Algoritma akan mendistribusikan nomor kelompok secara urut berdasarkan prodi untuk meminimalkan teman se-jurusan.
    4.  Hasil otomatis terunduh dengan nama: `pembagian_kelompok_fusion_final.csv`.

### 📝 3. Penghitung Presensi Maba.ipynb
**Alias:** Si Detektif Bolos 🕵️‍♂️
**Fungsi:** Menghitung nilai kehadiran dari data log presensi mentah berdasarkan target (threshold) pertemuan.

* **Persiapan Data:**
    * **File Data Maba:** Excel/CSV berisi daftar nama (Wajib ada kolom `NIM`).
    * **File Presensi:** Excel/CSV berisi log kehadiran (Wajib ada kolom `NIM`). Satu NIM bisa muncul berkali-kali sesuai jumlah hadirnya.
* **Cara Menggunakan:**
    1.  Jalankan program.
    2.  Ketik angka **Threshold** (Target minimal hadir untuk nilai 100), lalu Enter.
    3.  Upload **File Data Maba** saat diminta.
    4.  Upload **File Presensi** saat diminta.
    5.  Program menghitung: `(Jumlah Hadir / Threshold) * 100`.
    6.  Hasil otomatis terunduh dengan nama: `hasil_presensi_final.xlsx`.

### 📊 4. Penilaian Kelulusan Streak Email Maba 2025.ipynb
**Alias:** Si Mak Comblang Data (All-in-One) 💘
**Fungsi:** Alat serbaguna untuk menggabungkan data mahasiswa dengan data nilai, streak, atau email. Memiliki 3 mode:

**A. Mode Kelulusan/Sertifikasi**
* **Cara:** Upload 2 file (File Mahasiswa & File Nilai). Program otomatis menggabungkan berdasarkan NIM. Mahasiswa tanpa nilai akan dianggap 0.
* **Output:** `hasil_nilai_maba.xlsx`.

**B. Mode Nilai Streak**
* **Cara:** Upload 2 file. Program otomatis membersihkan nama kolom (menghapus spasi & kapitalisasi) agar lebih akurat membaca kolom `NIM` dan `NILAI`.
* **Output:** `hasil_rekap_nilai_fix.xlsx`.

**C. Mode Pencocokan Email**
* **Cara:** Upload 2 file (File Acuan Urutan & File Sumber Data Lengkap). Program akan mencari kolom `email` di salah satu file dan menempelkannya ke File Acuan berdasarkan NIM, tanpa merusak urutan baris acuan.
* **Output:** `hasil_nim_email.xlsx`.

---

### 🎨 Visualisasi Mood BPH QC
      Data Maba Berantakan              Pake Script QC 2025
          (╯°□°）╯︵ ┻━┻                      (✿◠‿◠)
        [WADUH GIMANA INI]               [SANTUY, REK!]
