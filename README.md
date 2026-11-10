# Single Layer Perceptron (SLP) - Iris Binary Classification

Tugas Mata Kuliah: **Kecerdasan Buatan Lanjut**  
Penyusun: **Muhammad Zaki Wiryawan**  

---

## Deskripsi Proyek
Repositori ini berisi implementasi **Single Layer Perceptron (SLP)** dari dasar (*from scratch*) untuk menyelesaikan binary classification pada dataset Iris (**Iris-setosa = 0** vs **Iris-versicolor = 1**). Perhitungan pada kode Python selama **5 Epoch** dengan metode learning **Stochastic Gradient Descent (SGD)**.

---

##  Spesifikasi & Hyperparameter
- **Dataset:** Iris Dataset (100 sampel: 50 Setosa, 50 Versicolor)
- **Target Encoding:** Setosa = `0`, Versicolor = `1`
- **Data Split (80 Training / 20 Validation):**
  - **Training Set (80 sampel):** 40 Setosa pertama (No 1–40) + 40 Versicolor pertama (No 51–90)
  - **Validation Set (20 sampel):** 10 Setosa terakhir (No 41–50) + 10 Versicolor terakhir (No 91–100)
- **Bobot Awal (*Initial Weights*):** $\text{bias} = 0.5, \theta_1 = 0.5, \theta_2 = 0.5, \theta_3 = 0.5, \theta_4 = 0.5$
- **Learning Rate ($\eta$):** `0.1`
- **Epochs:** 5 Epoch

---

## 📊 Hasil Evaluasi per Epoch

| Epoch | Training Loss (SSE) | Validation Loss (SSE) | Training Accuracy | Validation Accuracy | Final Bias |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **1** | 0.449889 | 0.328951 | 52.50% | 50.00% | 0.380336 |
| **2** | 0.037452 | 0.247289 | 95.00% | 50.00% | 0.342472 |
| **3** | 0.024372 | 0.175892 | 97.50% | 50.00% | 0.310418 |
| **4** | 0.017357 | 0.119381 | 97.50% | 85.00% | 0.282274 |
| **5** | 0.012740 | 0.081581 | 98.75% | 100.00% | 0.257720 |

---

## 📁 Struktur Berkas dalam Repositori
- `M Zaki Wiryawan_SLP.ipynb`: Jupyter Notebook lengkap berisi pemrosesan data, pelatihan model SLP, cetakan tabel No 1–20 per epoch, dan visualisasi.
- `Dataset Iris`: Dataset Iris untuk pelatihan SLP
- `chart accuracy gsheet.png` & `page3_python_accuracy.png`: Grafik kurva akurasi.
- `chart loss gsheet.png` & `page5_python_loss.png`: Grafik konvergensi loss.
