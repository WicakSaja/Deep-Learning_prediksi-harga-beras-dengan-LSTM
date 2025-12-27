📈 Prediksi Harga Beras Harian di Jakarta Menggunakan LSTM
📌 Deskripsi Proyek

Proyek ini bertujuan untuk menerapkan metode Deep Learning Long Short-Term Memory (LSTM) dalam melakukan peramalan (forecasting) harga beras harian di Jakarta berdasarkan data historis periode 2024–2025.
LSTM dipilih karena kemampuannya dalam mempelajari pola pada data time series yang memiliki ketergantungan antar waktu.

Proyek ini dibuat sebagai Tugas Besar (TUBES) Deep Learning.

🎯 Tujuan

Memprediksi harga beras harian berdasarkan data historis

Menerapkan konsep Deep Learning menggunakan LSTM

Menganalisis performa model melalui visualisasi dan metrik evaluasi

Menyajikan hasil dalam bentuk notebook, grafik, dan analisis

🗂️ Dataset

Jenis data: Time Series (Numerik)

Objek: Harga beras harian di Jakarta

Periode: 2024 – 2025

Kolom utama:

date : Tanggal

price : Harga beras

Dataset telah melalui tahap preprocessing, meliputi:

Pembersihan data

Pengurutan berdasarkan waktu

Normalisasi menggunakan Min-Max Scaling

🧠 Metode yang Digunakan

Long Short-Term Memory (LSTM)

Alasan penggunaan LSTM:

Cocok untuk data berurutan (time series)

Mampu mengingat pola jangka pendek dan jangka panjang

Lebih stabil dibanding RNN biasa

🏗️ Arsitektur Model

Arsitektur LSTM yang digunakan:

Input (7 hari terakhir)
↓
LSTM (50 units)
↓
Dense (1 neuron)
↓
Output (Harga Prediksi)


Window size: 7 hari

Optimizer: Adam

Loss Function: Mean Squared Error (MSE)

🔄 Alur Pengerjaan

Import library

Load dataset hasil preprocessing

Visualisasi data awal

Normalisasi data

Pembentukan data time series (sliding window)

Split data training dan validation

Pembangunan model LSTM

Training model

Visualisasi loss training & validation

Prediksi harga

Evaluasi model (MAE & MSE)

📊 Visualisasi Hasil

Grafik harga beras harian

Grafik training loss dan validation loss

Grafik perbandingan harga aktual vs harga prediksi

Visualisasi digunakan untuk menganalisis performa model dan mendukung interpretasi hasil.

📐 Evaluasi Model

Evaluasi dilakukan menggunakan:

Mean Squared Error (MSE)

Mean Absolute Error (MAE)

Metrik ini digunakan untuk mengukur selisih antara harga aktual dan harga hasil prediksi.

🛠️ Tools & Teknologi

Python

Google Colab

TensorFlow / Keras

Pandas

NumPy

Scikit-learn

Matplotlib

📁 Struktur Repository
📦 lstm-harga-beras-jakarta
 ┣ 📂 dataset
 ┃ ┗ cleaned_comodities_day.csv
 ┣ 📂 notebook
 ┃ ┗ LSTM_DeepLearning.ipynb
 ┣ 📄 README.md

📌 Kesimpulan

Model LSTM mampu mempelajari pola harga beras harian di Jakarta dan menghasilkan prediksi yang mengikuti tren data aktual. Meskipun masih terdapat selisih pada fluktuasi ekstrem, model ini sudah cukup baik untuk digunakan sebagai pendekatan peramalan harga komoditas.

🔗 Referensi

Dataset: Kaggle / hasil preprocessing pribadi

Dokumentasi TensorFlow & Keras

👤 Author

Bayu Wicaksono
Tugas Besar Deep Learning
📌 Google Colab | GitHub | LinkedIn
