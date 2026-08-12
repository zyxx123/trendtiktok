# 🌀 Retrolens - Hand Tracking Filter & Portal

Selamat datang di **Retrolens**! Aplikasi kamera interaktif masa depan yang digerakkan sepenuhnya oleh gestur tangan (hand tracking) menggunakan MediaPipe dan OpenCV. 

Bawa pengalaman augmented reality ke layar Anda: tarik panah imajiner untuk menyiram layar dengan efek keren, buat portal antar-dimensi dengan jari, dan ganti filter seperti seorang penyihir! 🪄

---

## ✨ Fitur Interaktif (Gestur)

Retrolens memiliki fitur deteksi gestur tangan yang sangat responsif. Cobalah gerakan-gerakan berikut di depan kamera:

- 🏹 **Jurus Memanah (Full Screen Effect):** 
  - *Cara:* Buka kedua telapak tangan lebar-lebar 👉 Cubit (satukan jempol dan telunjuk) seolah sedang menarik tali busur panah 👉 Lebarkan jari kembali untuk melepaskan tembakan!
  - *Efek:* Layar akan diselimuti secara penuh dengan filter yang sedang aktif, memberikan efek memukau ke seluruh visual Anda.

- ✊ **Jurus Menggenggam (Membersihkan Layar):**
  - *Cara:* Buka telapak tangan Anda lebar-lebar 👉 Kepalkan semua jari menjadi genggaman erat.
  - *Efek:* Menghapus efek memanah (layar penuh) dan mengembalikan tampilan normal dengan cepat.

- 🔲 **Jurus Portal (Filter Dimensi):**
  - *Cara:* Gunakan ujung telunjuk dan jempol dari **kedua** tangan Anda di depan kamera (total 4 jari). Pastikan Anda tidak sedang mengepal.
  - *Efek:* Sebuah portal dinamis akan terbentuk mengikuti pergerakan jari Anda. Area di dalam portal akan menampilkan filter aktif beserta kilauan partikel kosmis!

- 🔄 **Jurus Ganti Filter:**
  - *Cara:* Lakukan gerakan mencubit (satukan jempol dan telunjuk) pada **kedua tangan secara bersamaan**.
  - *Efek:* Berganti ke filter selanjutnya. Tersedia 11 filter estetik: `MONO`, `DUAL-TONE`, `PIXELATE`, `INVERT`, `SEPIA`, `BLUR`, `THERMAL`, `SKETCH`, `GLITCH`, `NEON`, dan `GALAXY`.

---

## 🛠️ Persyaratan Sistem
- Python 3.7+
- Webcam dengan resolusi yang memadai

## 🚀 Cara Install dan Menjalankan

### 1. Clone Repository
Unduh kode ini ke komputer Anda melalui terminal/command prompt:
```bash
git clone https://github.com/zyxx123/trendtiktok.git
cd trendtiktok
```

### 2. Buat Virtual Environment (Sangat Disarankan)
Gunakan virtual environment agar dependencies (library) proyek ini tidak bentrok dengan proyek Python Anda yang lain.
```bash
# Untuk Windows
python -m venv venv
.\venv\Scripts\activate

# Untuk macOS / Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
Install library yang dibutuhkan (seperti OpenCV, MediaPipe, dan Numpy):
```bash
pip install -r requirements.txt
```

### 4. File Model
Aplikasi ini sudah menggunakan dua model bawaan dari MediaPipe:
- `hand_landmarker.task` (Deteksi sendi & kerangka tangan)
- `selfie_segmenter.tflite` (Segmentasi background, khusus untuk filter *Galaxy*)
*Pastikan kedua file tersebut berada di folder yang sama dengan `main.py`.*

### 5. Mulai Keajaibannya!
Jalankan perintah berikut:
```bash
python main.py
```
*(Tekan tombol **`q`** pada keyboard dengan jendela aplikasi aktif untuk menutup aplikasi secara aman).*

---
**💡 Tips Pro:** Pastikan ruangan Anda memiliki pencahayaan yang cukup agar deteksi kerangka jari dari kamera bisa bekerja dengan sangat akurat dan mulus tanpa jeda!