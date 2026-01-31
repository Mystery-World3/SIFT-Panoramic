# 📸 SIFT-Panoramic: Image Stitching & Feature Matching

> **Project:** Implementasi Scale-Invariant Feature Transform (SIFT) untuk Pembuatan Gambar Panorama.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![OpenCV](https://img.shields.io/badge/Library-OpenCV-green)
![NumPy](https://img.shields.io/badge/Library-NumPy-orange)

Proyek ini adalah sistem **Computer Vision** yang dikembangkan untuk menggabungkan beberapa gambar menjadi satu tampilan panorama yang utuh. Menggunakan algoritma **SIFT**, sistem mampu mendeteksi fitur yang kuat terhadap perubahan skala maupun rotasi.



## 📋 Fitur Utama

Sistem ini melakukan pemrosesan citra melalui beberapa tahapan utama:
1. 🌟 **Feature Detection:** Mendeteksi titik kunci (*keypoints*) unik menggunakan algoritma SIFT.
2. 🔍 **Feature Matching:** Mencocokkan deskriptor antar gambar menggunakan *Brute-Force Matcher*.
3. 📐 **Homography Estimation:** Menghitung matriks transformasi menggunakan metode RANSAC untuk penyelarasan perspektif.
4. 🖼️ **Image Stitching:** Menggabungkan gambar dan melakukan *warping* untuk menghasilkan output panorama.

**Kelebihan Proyek:**
* **Scale Invariant:** Tetap akurat meskipun gambar memiliki resolusi atau jarak fokus yang berbeda.
* **Rotation Invariant:** Mampu mencocokkan fitur meskipun posisi kamera berputar.
* **Automated Blending:** Hasil sambungan gambar yang lebih halus.

## 📂 Struktur Direktori

Pastikan struktur folder Anda terlihat seperti ini:

```text
├── docs/
│   └── Laporan_Tugas_Besar_SIFT.pdf
├── images/
│   ├── input1.jpg
│   └── input2.jpg
├── results/
│   └── panorama_final.jpg
├── src/
│   ├── main.py
│   ├── stitching.py
│   └── utils.py
├── requirements.txt
└── README.md
```
## 🚀 Cara Instalasi

1. **Clone Repository ini:**
```bash
git clone [https://github.com/Mystery-World3/SIFT-Panoramic.git](https://github.com/Mystery-World3/SIFT-Panoramic.git)
cd SIFT-Panoramic
```

