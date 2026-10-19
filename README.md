# Simulasi CAT TKA Mandiri (SMA & SMK)

Aplikasi Web Simulasi Computer-Assisted Test (CAT) mandiri, ringan, zero-dependency, berbasis IndexedDB offline-ready khusus untuk persiapan **Tes Kemampuan Akademik (TKA) jenjang SMA dan SMK**.

## 📌 Bank Soal Terintegrasi (100% Terverifikasi)
1. **TKA SMA (Pakar Soal): Matematika Wajib - Paket 20** (30 Soal HOTS BSKAP)
2. **TKA SMA (Pakar Soal): Bahasa Inggris Wajib - Set 1** (30 Soal Analisis Naratif & Wacana)
3. **TKA SMA (Pakar Soal): Bahasa Indonesia Wajib - Set 20** (30 Soal Literasi Teks Sains Bioremediasi)
4. **TKA BPPP 2026: Penalaran Matematika & Kuantitatif** (25 Soal SNBT/BPPP Resmi)
5. **TKA BPPP 2026: Literasi Bahasa Indonesia** (25 Soal SNBT/BPPP Resmi)
6. **TKA BPPP 2026: Literasi Bahasa Inggris** (25 Soal SNBT/BPPP Resmi)
7. **TKA BPPP 2026: Penalaran Umum & Skolastik** (25 Soal SNBT/BPPP Resmi)
*Total: 7 Paket Ujian (190 Butir Soal Teruji Lengkap dengan Pembahasan)*

## 🚀 Fitur Sistem CAT
- **Live Countdown Timer**: Durasi per sesi (60 atau 45 menit), auto-submit jika habis, alert merah jika < 5 menit.
- **Status Ragu-Ragu (Flagging)**: Tandai soal belum yakin dengan warna kuning di grid drawer.
- **Konversi Nilai CAT**: Nilai akurasi (0-100) dan estimasi skor skala CAT resmi (200 - 800).
- **Pembahasan Lengkap**: Solusi bertahap & konsep kunci di bawah masing-masing butir soal setelah submit.
- **Offline / Local Ready**: Bisa dibuka langsung tanpa server, atau via LAN WiFi sekolah.

## 💻 Menjalankan di LAN / WiFi Sekolah
```bash
cd /home/vb/tka-cbt-mandiri
python3 -m http.server 8080
```
Siswa akses via browser HP: `http://<IP_KOMPUTER_GURU>:8080`

## ☁️ Deploy ke Vercel
1. Buat repository baru di GitHub (misal: `tka-cbt-mandiri`).
2. Jalankan perintah:
```bash
cd /home/vb/tka-cbt-mandiri
git init
git add .
git commit -m "feat: initial commit simulasi CAT TKA mandiri SMA/SMK"
git remote add origin https://github.com/<USERNAME>/tka-cbt-mandiri.git
git push -u origin main
```
3. Import project tersebut di dashboard Vercel ([vercel.com/new](https://vercel.com/new)), project langsung live otomatis!
