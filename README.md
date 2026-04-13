# Analisis Tipologi Lumbung Padi Jawa Tengah (K-Medoids Clustering) 🌾

[![R-Version](https://img.shields.io/badge/R-4.5.1-blue.svg)](https://www.r-project.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

Repository ini berisi proyek analisis data statistika untuk mengidentifikasi karakteristik tipologi wilayah lumbung padi di Provinsi Jawa Tengah menggunakan algoritma **K-Medoids Clustering**.

## 📌 Ringkasan Proyek
Penelitian ini memetakan 35 kabupaten/kota di Jawa Tengah berdasarkan 4 indikator utama:
1. **UTP (Unit Tani Pangan)**
2. **Total Produksi Padi (Ton)**
3. **Luas Irigasi Teknis (Ha)**
4. **Luas Irigasi Non-Teknis (Ha)**

Analisis ini bertujuan untuk memberikan dasar bagi pemerintah dalam menentukan strategi ketahanan pangan yang tepat sasaran berdasarkan karakteristik unik tiap wilayah.

## 🛠️ Metodologi & Tahapan
- **Preprocessing:** Standarisasi data menggunakan *Z-Score*.
- **Uji Asumsi:** Uji Multikolinearitas (VIF) untuk memastikan independensi variabel.
- **Optimasi Klaster:** Penentuan jumlah $k$ optimal menggunakan metode *Silhouette Coefficient*.
- **Clustering:** Implementasi algoritma **PAM (Partitioning Around Medoids)** yang lebih *robust* terhadap outlier data pertanian.

## 📊 Hasil Utama
Dihasilkan 5 Klaster Tipologi Wilayah:
- **Klaster 1:** Wilayah Lumbung Padi Utama (Maha-Lumbung)
- **Klaster 2:** Wilayah Lumbung Padi Penyangga (Sentra Utama)
- **Klaster 3:** Wilayah Lumbung Padi Mandiri (Sentra Potensial)
- **Klaster 4:** Wilayah Lumbung Padi Adaptif (Sentra Terbatas)
- **Klaster 5:** Wilayah Lumbung Padi Marginal (Sentra Perkotaan)

## 📂 Struktur File
- `kmedoids_lumbung_padi.Rmd`: Script utama analisis dalam format R Markdown.
- `DATASET LUMBUNG PADI FIKS.xlsx`: Dataset riil indikator pertanian Jawa Tengah.
- `kmedoids_lumbung_padi.html`: Output laporan final yang interaktif dan responsif.

## 🚀 Cara Menjalankan
1. Clone repository ini.
2. Pastikan library `tidyverse`, `cluster`, `factoextra`, dan `corrplot` sudah terinstall.
3. Buka `Clustering K-Medoids.Rproj`.
4. Run/Knit file `kmedoids_lumbung_padi.Rmd`.

---
**Kontributor:** Rafi Abdul Rosid (Statistika Undip)
