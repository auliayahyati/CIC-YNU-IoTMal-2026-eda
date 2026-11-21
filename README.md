# 🛡️ Exploratory Data Analysis: IoT Malware Network Traffic (ARM Architecture)

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

## 📌 Project Overview
Proyek ini melakukan **Exploratory Data Analysis (EDA)** terhadap lalu lintas jaringan (*network traffic*) malware IoT pada arsitektur **ARM** menggunakan dataset **CIC-YNU-IoTMal 2026** dari Canadian Institute for Cybersecurity (UNB) & Yunnan University.

Tujuan utama analisis ini adalah memahami pola komunikasi jaringan malware IoT, mengidentifikasi *class imbalance* antar keluarga malware, serta menemukan fitur jaringan paling relevan sebelum tahap *feature selection* dan pemodelan *Machine Learning*.

---

## 📊 Dataset Summary
* **Sumber Dataset:** [CIC-YNU-IoTMal 2026 (UNB)](https://www.unb.ca/cic/datasets/ynu-iot-2026.html)
* **Subset Fokus:** Arsitektur CPU **ARM**
* **Skala Data:** ~737.651 baris (*records*), 36 fitur numerik *network traffic*, 5.599 *unique hashes*, dan 8 kelas *malware family*.

---

## 🔍 Key Findings & Visualizations

### 1. Severe Class Imbalance pada Malware Family
Distribusi kelas menunjukkan ketimpangan ekstrem antara keluarga malware mayoritas dan minoritas. Hal ini mengindikasikan bahwa metrik *Accuracy* saja tidak cukup untuk evaluasi model nantinya (perlu *Balanced Accuracy* atau *Macro-F1*).

![Distribusi Kelas Malware](images/class_distribution.png)

### 2. Korelasi Fitur Network Traffic
Analisis korelasi menunjukkan adanya beberapa fitur yang memiliki multikolinearitas tinggi (*redundant features*), yang menjadi kandidat kuat untuk direduksi pada tahap *feature selection*.

![Heatmap Korelasi](images/correlation_heatmap.png)

---

## 🛠️ Tech Stack
* **Bahasa:** Python 3.x
* **Manipulasi Data:** `pandas`, `numpy`
* **Visualisasi:** `matplotlib`, `seaborn`

---

## 🚀 How to Run
1. Clone repositori ini:
   ```bash
   git clone [https://github.com/USERNAME_KAMU/NAMA_REPO_KAMU.git](https://github.com/USERNAME_KAMU/NAMA_REPO_KAMU.git)
