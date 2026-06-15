# 🎮 Quiz Game — Kelompok 18
**Presentasi Bahasa Inggris · Error Identification · Word Choice · Written Expression**

---

## 📁 File yang Ada
| File | Fungsi |
|------|--------|
| `index_firebase.html` | **File utama** — rename jadi `index.html` sebelum deploy |
| `vercel.json` | Konfigurasi deploy Vercel |
| `README.md` | Panduan ini |

---

## 🔥 STEP 1 — Buat Project Firebase (Gratis)

### 1.1 Buat Project
1. Buka https://console.firebase.google.com
2. Klik "Add project" → beri nama, misal: quiz-kelompok18
3. Klik Continue sampai selesai

### 1.2 Aktifkan Realtime Database
1. Sidebar kiri → Build → Realtime Database
2. Klik "Create database"
3. Pilih lokasi: Singapore (asia-southeast1)
4. Pilih mode: "Start in test mode" → Enable

### 1.3 Salin Firebase Config
1. Klik ikon ⚙️ Project Settings di sidebar kiri
2. Scroll ke bagian "Your apps"
3. Klik ikon </> (Web) → Register app
4. Copy kode firebaseConfig yang muncul

### 1.4 Atur Rules (Izinkan Baca/Tulis)
Di Realtime Database → tab "Rules" → ganti isi jadi:
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
Klik "Publish"

---

## 🚀 STEP 2 — Deploy ke GitHub + Vercel

1. Rename file: mv index_firebase.html index.html
2. Upload ke GitHub:
   git init
   git add .
   git commit -m "Quiz Game Kelompok 18"
   git remote add origin https://github.com/USERNAME/presentasi-games-kelompok18.git
   git push -u origin main
3. Buka vercel.com → New Project → Import repo → Deploy

---

## ⚙️ STEP 3 — Konfigurasi Firebase di Website

1. Buka URL Vercel di browser
2. Halaman pertama = form Firebase config
3. Isi semua kolom dari firebaseConfig yang sudah di-copy
4. Klik "Simpan & Lanjutkan"
5. Config tersimpan di browser, tidak perlu isi ulang

---

## 🎯 STEP 4 — Cara Pakai Saat Presentasi

Laptop (Proyektor) : Buka URL → klik Admin → login admin/password
HP Mahasiswa       : Buka URL → klik Masuk sebagai Mahasiswa → isi Nama, NIM, Prodi

Alur:
1. Admin klik [▶ Mulai Kuis] → Soal 1 tampil di proyektor
2. Mahasiswa klik A/B/C/D di HP → Nama muncul real-time di layar admin
3. Admin klik [💡 Bahas] → Pembahasan tampil
4. Admin klik [Berikutnya →] → Soal berikutnya
5. Setelah soal ke-20 → Admin klik [🏆 Hasil] → Leaderboard

---

## 📊 Sistem Skor
- Jawaban benar : 1000 poin
- Bonus kecepatan: 0-500 poin (makin cepat makin banyak, max 30 detik)
- Jawaban salah : 0 poin

---

## 🔐 Akun Admin
Username : admin
Password : password

---

## 📝 Jawaban Soal
1-C  2-C  3-C  4-C  5-C  6-D  7-A
8-B  9-B  10-C  11-C  12-B  13-A
14-C  15-C  16-B  17-C  18-D  19-C  20-C

---

Kelompok 18 · Alifah Lisy Safa'ah · Annas Thoyibin · Hafidz Muftadin Amri
