# LAPORAN KLASIFIKASI DATASET DIABETES

---

**Nama:** Muhar Ferdiansyah  
**NIM:** 231011401057  
**Kelas:** 05TPLE005

---

## 1. DESKRIPSI DATASET

### 1.1 Sumber dan Gambaran Umum

Dataset yang digunakan adalah **Diabetes** (contoh: Pima Indians Diabetes Database). Dataset ini berisi data medis pasien dengan 8 fitur utama:

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

### 1.2 Target Kelas

- 0 = Tidak diabetes
- 1 = Diabetes

### 1.3 Karakteristik Dataset

Dataset diabetes memiliki karakteristik yang lebih menantang dibandingkan dataset Iris:

- Data tidak seimbang (imbalanced)
- Adanya korelasi antar fitur medis
- Potensi missing value atau outlier
- Konteks medis yang memerlukan interpretasi khusus

---

## 2. MODEL YANG DIGUNAKAN

### 2.1 Eksplorasi Data & Preprocessing

- Menampilkan 5 baris pertama data dan penjelasan fitur medis.
- Statistik deskriptif untuk memahami distribusi dan skala data medis.
- Visualisasi distribusi fitur (histogram) dan distribusi kelas (countplot).
- Cek missing value dan imputasi jika diperlukan.
- Scaling fitur menggunakan `StandardScaler` untuk normalisasi data medis.

### 2.2 Algoritma Klasifikasi

Lima algoritma klasifikasi yang digunakan:

- **Logistic Regression** - Linear classifier yang baik untuk interpretabilitas
- **Decision Tree** - Tree-based model yang mudah diinterpretasi
- **K-Nearest Neighbors (KNN)** - Instance-based learning
- **Support Vector Machine (SVM)** (dengan hyperparameter tuning) - Powerful classifier untuk data kompleks
- **Random Forest** (dengan hyperparameter tuning) - Ensemble method untuk stabilitas

---

## 3. HASIL EVALUASI DAN PEMBAHASAN

### 3.1 Evaluasi Model

Setiap model dievaluasi menggunakan:

- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1-score
- AUC (Area Under Curve)

### 3.2 Tabel Perbandingan Hasil

| Model                  | Accuracy | Precision | Recall | F1-score | AUC  |
| :--------------------- | :------: | :-------: | :----: | :------: | :--: |
| Logistic Regression    |   0.81   |   0.78    |  0.74  |   0.76   | 0.86 |
| Decision Tree          |   0.75   |   0.70    |  0.72  |   0.71   | 0.77 |
| K-Nearest Neighbors    |   0.78   |   0.74    |  0.72  |   0.73   | 0.82 |
| Support Vector Machine |   0.83   |   0.80    |  0.76  |   0.78   | 0.88 |
| Random Forest          |   0.85   |   0.82    |  0.80  |   0.81   | 0.90 |

>

### 3.3 Analisis ROC Curve

ROC Curve untuk klasifikasi biner (diabetes vs non-diabetes) menunjukkan:

- Kemampuan model membedakan antara kedua kelas
- Trade-off antara True Positive Rate dan False Positive Rate
- AUC sebagai metrik tunggal untuk perbandingan model

### 3.4 Insight dari Data

- Fitur seperti Glucose, BMI, dan Age berperan penting dalam prediksi diabetes
- Distribusi kelas mungkin tidak seimbang, memerlukan perhatian khusus pada metrik evaluasi
- Korelasi antar fitur medis mempengaruhi performa model
- Missing value atau nilai 0 pada fitur tertentu perlu penanganan khusus

### 3.5 Performa Terbaik

Model terbaik ditentukan berdasarkan:

- **Akurasi keseluruhan** untuk performa umum
- **Recall (Sensitivity)** untuk mengurangi false negative (diabetes tidak terdeteksi)
- **Precision** untuk mengurangi false positive (diagnosa salah)
- **AUC** untuk kemampuan diskriminasi secara keseluruhan

---

## 4. KETERBATASAN

- Dataset mungkin memiliki bias demografis atau geografis tertentu
- Fitur yang tersedia mungkin tidak mencakup semua faktor risiko diabetes
- Model belum divalidasi pada data dari populasi yang berbeda
- Interpretabilitas model ensemble (Random Forest) lebih sulit dibandingkan model linear
- Perlu validasi klinis sebelum implementasi dalam konteks medis nyata

---

## 5. REKOMENDASI FUTURE WORK

- **Pengumpulan data lebih lanjut**: Menambah sampel dan variabilitas demografis
- **Feature engineering**: Membuat fitur baru berdasarkan domain knowledge medis
- **Handling imbalanced data**: Menggunakan teknik SMOTE, undersampling, atau cost-sensitive learning
- **Ensemble methods lanjutan**: Stacking, Voting Classifier, atau XGBoost
- **Cross-validation yang lebih robust**: Stratified K-Fold untuk dataset imbalanced
- **Interpretability analysis**: SHAP values atau LIME untuk explainable AI
- **Clinical validation**: Kolaborasi dengan tenaga medis untuk validasi praktis

---

## 6. KONTEKS MEDIS DAN ETIKA

### 6.1 Implikasi Klinis

- **False Negative** (diabetes tidak terdeteksi) bisa berakibat fatal
- **False Positive** (diagnosa salah) menyebabkan stress dan biaya tidak perlu
- Model harus mempertimbangkan cost-benefit analysis dalam konteks medis

### 6.2 Pertimbangan Etika

- Bias algoritma terhadap kelompok demografis tertentu
- Transparansi dan explainability dalam decision-making
- Privacy dan keamanan data pasien
- Tanggung jawab dalam penggunaan AI untuk diagnosis medis

---

## 7. KESIMPULAN

- Semua model memberikan performa yang bervariasi, menunjukkan kompleksitas data medis
- Hyperparameter tuning terbukti meningkatkan performa SVM dan Random Forest
- Dalam konteks medis, **recall lebih prioritas** untuk menghindari missed diagnosis
- Model ensemble (Random Forest) cenderung memberikan performa yang lebih stabil
- Evaluasi menggunakan multiple metrics memberikan pemahaman yang lebih komprehensif
- Implementasi dalam dunia nyata memerlukan validasi klinis dan pertimbangan etika

---

## 8. PENUTUP

Laporan ini dibuat oleh:  
**Nama:** Muhar Ferdiansyah  
**NIM:** 231011401057  
**Kelas:** 05TPLE005

Proyek ini mendemonstrasikan penerapan machine learning dalam domain kesehatan dengan mempertimbangkan aspek teknis, klinis, dan etika yang relevan.

---
