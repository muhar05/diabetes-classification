# 📋 Instruksi Menjalankan Workspace Diabetes Prediction

## 🚀 Quick Start

### 1. Buka VS Code

Navigasi ke folder workspace diabetes:

```
e:\muhar\Tugas Matkul\S5\MACHINE LEARNING\uts\diabetes_prediction\
```

### 2. Install Dependencies

Buka terminal di VS Code dan jalankan:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter ipython
```

### 3. Jalankan Notebook

- Buka file `diabetes_classification.ipynb`
- Pilih Python interpreter yang sesuai
- Jalankan semua cell secara berurutan (Ctrl+Shift+P → "Run All")

---

## 📊 Dataset

Dataset `diabetes.csv` sudah disediakan dengan 768 sampel data pasien dan 9 kolom:

- **8 fitur medis**: Pregnancies, Glucose, BloodPressure, dll.
- **1 target**: Outcome (0=tidak diabetes, 1=diabetes)

---

## 🔍 Struktur Analisis

1. **Import & Load Data**
2. **Exploratory Data Analysis (EDA)**
3. **Preprocessing & Scaling**
4. **Train-Test Split**
5. **5 Model Machine Learning**:
   - Logistic Regression
   - Decision Tree
   - K-Nearest Neighbors
   - Support Vector Machine (tuned)
   - Random Forest (tuned)
6. **Evaluasi Komprehensif**
7. **Perbandingan Model**

---

## 📈 Output yang Dihasilkan

- Statistik deskriptif dan visualisasi distribusi
- Confusion matrix untuk setiap model
- Metrik evaluasi (Accuracy, Precision, Recall, F1-score, AUC)
- ROC Curve untuk semua model
- Tabel perbandingan dan heatmap performa
- Insight dan rekomendasi model terbaik

---

## 🎯 Hasil yang Diharapkan

Dataset diabetes akan menunjukkan:

- Performa model yang lebih realistis (70-85% accuracy)
- Perbedaan yang lebih signifikan antar algoritma
- Pentingnya hyperparameter tuning
- Trade-off antara precision dan recall dalam konteks medis

---

## 📝 Tips

- **Jalankan cell satu per satu** untuk memahami setiap langkah
- **Perhatikan interpretasi medis** dari hasil model
- **Bandingkan AUC score** untuk menilai kemampuan diskriminasi
- **Fokus pada recall** untuk mengurangi missed diagnosis

---

Selamat mencoba! 🎉
