# SIFT-Panoramic 📸

[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/Mystery-World3/SIFT-Panoramic/issues)

Proyek ini mengimplementasikan algoritma **Scale-Invariant Feature Transform (SIFT)** untuk mendeteksi fitur pada gambar dan melakukan *Image Stitching* guna menghasilkan foto panorama yang mulus.

---

## 📖 Deskripsi Proyek
Proyek ini dikembangkan untuk mengeksplorasi teknik *Computer Vision* dalam menyatukan beberapa citra digital. Dengan menggunakan SIFT, sistem dapat mengenali titik-titik kunci (*keypoints*) yang invarian terhadap skala dan rotasi, sehingga proses pencocokan gambar tetap akurat meskipun posisi pengambilan gambar sedikit berbeda.



### Fitur Utama:
* **Feature Detection & Extraction**: Menggunakan SIFT untuk menemukan titik unik pada gambar.
* **Feature Matching**: Menggunakan *Brute-Force Matcher* dengan *Lowe's Ratio Test* untuk menyaring kecocokan fitur yang salah.
* **Image Warping**: Transformasi perspektif menggunakan *Homography matrix*.
* **Stitching**: Menggabungkan gambar menjadi satu kesatuan panorama.

---

## 📂 Struktur Repositori
```text
├── images/             # Folder berisi gambar input (raw images)
├── results/            # Folder hasil output gambar panorama
├── src/                # Kode sumber utama (.py atau .ipynb)
├── docs/               # Laporan Tugas Besar & Presentasi
├── requirements.txt    # Daftar library yang diperlukan
└── README.md           # Dokumentasi proyek

---

## ⚙️ Alur Kerja (Workflow)
Proyek ini mengikuti langkah-langkah standar dalam *Computer Vision* untuk pembuatan panorama:



1. **Preprocessing**: Membaca gambar input dan mengonversinya ke skala abu-abu (*grayscale*).
2. **Detection**: Mencari titik-titik kunci menggunakan SIFT.
3. **Matching**: Menghitung jarak antar deskriptor untuk menemukan pasangan titik yang sama di dua gambar.
4. **Homography**: Menghitung matriks transformasi untuk menyelaraskan perspektif gambar kedua ke gambar pertama.
5. **Blending**: Menggabungkan gambar dan menghaluskan sambungan agar tidak terlihat garis potong (seams).

---

## 🛠️ Instalasi & Persiapan

1. **Clone Repositori**
   ```bash
   git clone [https://github.com/Mystery-World3/SIFT-Panoramic.git](https://github.com/Mystery-World3/SIFT-Panoramic.git)
   cd SIFT-Panoramic

