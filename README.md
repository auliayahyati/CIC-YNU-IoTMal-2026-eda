# 🛡️ Exploratory Data Analysis: IoT Malware Network Traffic (ARM Architecture)

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)

## 📌 Project Overview
Proyek ini melakukan **Exploratory Data Analysis (EDA)** terhadap lalu lintas jaringan (*network traffic*) perangkat IoT pada arsitektur **ARM** menggunakan modalitas **PCAP** dari **CIC-YNU-IoTMal Dataset 2026**. Tujuan utamanya adalah memahami struktur, kualitas data, distribusi fitur, serta mengidentifikasi pola lalu lintas jaringan yang membedakan aktivitas normal (*benign*) dan berbahaya (*malware*) sebagai dasar pengembangan model klasifikasi *Machine Learning*.

## 📊 Dataset Summary
| Komponen | Keterangan |
| :--- | :--- |
| **Nama Dataset** | CIC-YNU-IoTMal Dataset 2026 |
| **Penyedia** | Canadian Institute for Cybersecurity (CIC) & Yokohama National University |
| **Arsitektur & Modalitas** | ARM — PCAP (Packet Capture) |
| **Format File** | Parquet |
| **Ukuran Data** | 737.651 *records* & 40 fitur |
| **Sumber Resmi** | [UNB CIC Dataset Page](https://www.unb.ca/cic/datasets/ynu-iot-2026.html) |

## 🎯 Tipe Masalah & Metrik Evaluasi
* **Tipe Masalah:** *Supervised Learning* — Klasifikasi Biner (*Benign* vs *Malware*) yang dapat diperluas ke *Multiclass* berdasarkan keluarga malware.
* **Metrik Prioritas:** **Recall** dan **F1-Score** (mengantisipasi *class imbalance* dan meminimalkan ancaman yang tidak terdeteksi), didukung oleh *Accuracy*, *Precision*, dan *Confusion Matrix*.

## 🔍 Tahapan EDA yang Dilakukan
1. **Inspeksi Struktur & Statistik Deskriptif:** Pemeriksaan dimensi, tipe data, *mean, median, modus*, standar deviasi, dan varians.
2. **Peninjauan Kualitas Data:** Pengecekan *missing values* (`missingno`), data duplikat, deteksi *outliers* dengan metode IQR, serta konsistensi nilai (*infinity* & kolom konstan).
3. **Eksplorasi Visual:** Analisis distribusi fitur (*Histogram & KDE*), hubungan antarvariabel (*Scatter Plot*, *Boxplot* per kelas, dan *Pearson Correlation Heatmap*).

## 📈 Visualisasi Utama
*(Ganti nama file gambar di bawah sesuai dengan gambar yang kamu unggah ke folder `images/`)*

### Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)

## 📂 Struktur Repositori
* `notebooks/` — File Jupyter Notebook (`.ipynb`) berisi seluruh kode EDA dan outputnya.
* `images/` — Kumpulan grafik visualisasi hasil EDA (`.png`).
* `docs/` — Laporan lengkap proyek dalam format PDF.
