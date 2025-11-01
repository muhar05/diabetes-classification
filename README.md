# 🩺 Klasifikasi Dataset Diabetes

**Nama:** Muhar Ferdiansyah  
**NIM:** 231011401057  
**Kelas:** 05TPLE005

Notebook ini membahas proses klasifikasi dataset **diabetes** menggunakan lima algoritma: **Logistic Regression**, **Decision Tree**, **K-Nearest Neighbors (KNN)**, **Support Vector Machine (SVM)**, dan **Random Forest**. Evaluasi dilakukan menggunakan confusion matrix, metrik akurasi, precision, recall, F1-score, serta ROC Curve. Hyperparameter tuning sederhana juga diterapkan pada SVM dan Random Forest.

---

## 📖 Deskripsi Proyek

Proyek ini bertujuan untuk membandingkan performa beberapa algoritma klasifikasi populer dalam memprediksi risiko diabetes pada pasien berdasarkan fitur-fitur medis. Hasil evaluasi dapat digunakan sebagai referensi pemilihan model untuk kasus deteksi penyakit.

---

## 🛠️ Teknologi yang Digunakan

- Python 3.x
- Jupyter Notebook / Visual Studio Code
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 📁 Struktur File

```
diabetes_prediction/
├── diabetes_classification.ipynb    # Notebook utama
├── data/
│   └── diabetes.csv                 # Dataset Diabetes
├── LAPORAN_KLASIFIKASI_DIABETES.MD  # Laporan singkat
└── README.md                        # Petunjuk & deskripsi proyek
```

---

## 🚀 Cara Menjalankan

1. **Pastikan Python sudah terinstall.**
2. Install library yang dibutuhkan:
   ```sh
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. **Download dataset diabetes** dan simpan sebagai `data/diabetes.csv`
   - Bisa menggunakan Pima Indians Diabetes Database dari Kaggle
   - Atau dataset diabetes lainnya dengan format yang sesuai
4. Buka file `diabetes_classification.ipynb` di Jupyter Notebook atau Visual Studio Code.
5. Jalankan setiap cell secara berurutan.

---

## 📊 Deskripsi Dataset

Dataset **Diabetes** berisi data medis pasien dengan fitur-fitur seperti:

| Fitur                    | Deskripsi                       |
| ------------------------ | ------------------------------- |
| Pregnancies              | Jumlah kehamilan                |
| Glucose                  | Konsentrasi glukosa plasma      |
| BloodPressure            | Tekanan darah diastolik (mm Hg) |
| SkinThickness            | Ketebalan kulit trisep (mm)     |
| Insulin                  | Insulin serum 2 jam (mu U/ml)   |
| BMI                      | Body Mass Index                 |
| DiabetesPedigreeFunction | Fungsi silsilah diabetes        |
| Age                      | Usia (tahun)                    |

**Target Kelas:**

- 0 = Tidak diabetes
- 1 = Diabetes

---

## 🤖 Model yang Digunakan

- **Logistic Regression**
- **Decision Tree**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machine (SVM)** (dengan hyperparameter tuning)
- **Random Forest** (dengan hyperparameter tuning)

---

## 📝 Evaluasi

- Confusion Matrix
- Accuracy, Precision, Recall, F1-score
- ROC Curve dan AUC
- Tabel perbandingan hasil model
- Visualisasi heatmap performa

---

## ✨ Hasil Singkat

| Model                  | Accuracy | Precision | Recall | F1-score | AUC |
| :--------------------- | :------: | :-------: | :----: | :------: | :-: |
| Logistic Regression    |   ---    |    ---    |  ---   |   ---    | --- |
| Decision Tree          |   ---    |    ---    |  ---   |   ---    | --- |
| K-Nearest Neighbors    |   ---    |    ---    |  ---   |   ---    | --- |
| Support Vector Machine |   ---    |    ---    |  ---   |   ---    | --- |
| Random Forest          |   ---    |    ---    |  ---   |   ---    | --- |

> _Nilai akan diisi otomatis setelah menjalankan notebook._

**Konteks Medis:**

- **Precision tinggi**: Mengurangi diagnosa diabetes yang salah (false positive)
- **Recall tinggi**: Mengurangi kasus diabetes yang tidak terdeteksi (false negative)
- **Balance**: Dalam konteks medis, recall lebih penting untuk menghindari missed diagnosis

---

## 📄 Laporan

Laporan lengkap dapat dibaca pada file [`LAPORAN_KLASIFIKASI_DIABETES.MD`](./LAPORAN_KLASIFIKASI_DIABETES.MD).

---

## 🔗 Dataset

Dataset yang disarankan:

- [Pima Indians Diabetes Database - Kaggle](https://www.kaggle.com/datasets/uciml/pima-Indians-diabetes-database)
- Format: CSV dengan kolom Outcome sebagai target (0/1)

---

## 👤 Author & Lisensi

- **Author:** Muhar Ferdiansyah (231011401057)
- **Lisensi:** Untuk keperluan akademik (Academic Use Only)

---
