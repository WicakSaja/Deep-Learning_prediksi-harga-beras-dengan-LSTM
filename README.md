# 📈 Prediksi Harga Beras Harian di Jakarta dengan LSTM

Proyek ini merupakan penerapan **Deep Learning menggunakan metode Long Short-Term Memory (LSTM)** untuk melakukan **peramalan harga beras harian di Jakarta** berdasarkan data historis periode **2024–2025**.

Proyek ini dibuat sebagai **Tugas Besar Deep Learning**.

---

## 🎯 Tujuan Proyek
- Memprediksi harga beras harian berdasarkan data sebelumnya
- Menerapkan metode LSTM pada data time series
- Menampilkan hasil prediksi dalam bentuk grafik
- Mengevaluasi performa model menggunakan metrik error

---

## 📊 Dataset
- **Jenis data**: Time Series (numerik)
- **Objek**: Harga beras harian di Jakarta
- **Periode**: 2024 – 2025
- **Kolom**:
  - `date`  → tanggal
  - `price` → harga beras

Dataset yang digunakan telah melalui tahap preprocessing:
- Data dibersihkan
- Diurutkan berdasarkan waktu
- Dinormalisasi menggunakan Min-Max Scaling

---

## 🧠 Metode Deep Learning
Metode yang digunakan adalah **Long Short-Term Memory (LSTM)**.

### Alasan menggunakan LSTM:
- Cocok untuk data berurutan (time series)
- Mampu mempelajari pola jangka pendek dan jangka panjang
- Lebih stabil dibandingkan RNN biasa

---

## 🏗️ Arsitektur Model
Arsitektur LSTM yang digunakan dalam proyek ini:

Input (7 hari terakhir)
↓
LSTM (50 units)
↓
Dense (1 neuron)
↓
Output (Harga Prediksi)


- Window size: 7 hari
- Optimizer: Adam
- Loss function: Mean Squared Error (MSE)

---

## 🔄 Alur Pengerjaan
1. Import library
2. Load dataset hasil preprocessing
3. Visualisasi data awal
4. Normalisasi data
5. Membentuk data time series (sliding window)
6. Split data training dan validation
7. Membangun model LSTM
8. Training model
9. Visualisasi training dan validation loss
10. Prediksi harga
11. Evaluasi model

---

## 📈 Visualisasi
Proyek ini menampilkan beberapa visualisasi:
- Grafik harga beras harian
- Grafik training loss dan validation loss
- Grafik perbandingan harga aktual vs harga prediksi

---

## 📐 Evaluasi Model
Evaluasi model dilakukan menggunakan:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)

Metrik ini digunakan untuk mengukur selisih antara nilai aktual dan hasil prediksi.

---

## 🛠️ Tools & Library
- Python
- Google Colab
- TensorFlow / Keras
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## ✅ Kesimpulan
Model LSTM mampu mempelajari pola harga beras harian di Jakarta dan menghasilkan prediksi yang mengikuti tren data aktual. Model ini cukup baik digunakan sebagai pendekatan peramalan harga komoditas berbasis deep learning.

---

## 👤 Author
Bayu Wicaksono  
Tugas Besar Deep Learning
