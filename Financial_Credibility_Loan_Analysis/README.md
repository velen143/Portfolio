## Project: Analisis Kredibilitas Finansial & Pengambilan Keputusan Pinjaman

## Overview

Proyek ini adalah analisis data komprehensif yang dirancang untuk menggali karakteristik finansial dan demografis dari 10.000 nasabah serta mengidentifikasi pola-pola signifikan yang mempengaruhi skor kredit. Tujuan dari analisis ini adalah mengidentifikasi perbedaan profil finansial dan demografis antara kelompok skor kredit serta mengetahui hubungan antara berbagai variabel ekonomi dan perilaku dengan skor kredit.

## Tools
* Python
* Pandas & Numpy
* Searborn
* Matplotlib
* Scipy

## Alur Kerja 
### 1. Data Understanding (Pemahaman Data)
Tahap awal melibatkan inspeksi mendalam terhadap dataset yang terdiri dari 10.000 baris dan 16 kolom. Ini mencakup pemeriksaan struktur data, tipe data, serta statistik deskriptif untuk setiap variabel. Pemahaman ini sangat penting untuk membentuk dasar analisis yang kuat dan relevan.

### 2. Data Quality (Kualitas Data)
Pemeriksaan kualitas data dilakukan untuk mengetahui adanya missing values dan duplikasi data 

### 3. Data Cleaning (Pembersihan Data)
Variabel-variabel dikelompokkan secara metodis menjadi tipe numerik dan kategorikal, memungkinkan penerapan metode analisis yang paling sesuai untuk setiap jenis data.

### 4. Exploratory Data Analysis (EDA) & Inferential Statistics
Untuk mengidentifikasi pola dan hubungan antar variabel, digunakan kombinasi visualisasi data dan uji statistik inferensial, meliputi:
*   **Uji Chi-squared:** untuk menilai hubungan yang signifikan antara variabel kategorikal dengan skor kredit.
*   **Uji T-test:** untuk membandingkan rata-rata variabel numerik antara dua kelompok skor kredit, memberikan insight tentang perbedaan rata-rata.
*   **Uji Kruskal-Wallis:** membandingkan median variabel numerik di antara beberapa kelompok skor kredit, memberikan gambaran terhadap perbedaan distribusi.
*   **Analisis Korelasi (Heatmap):** mengukur kekuatan dan arah hubungan linear antar variabel numerik dengan skor kredit.

### Hasil Analisis 
* Rata - rata saldo akhir bulan dan masa kerja menunjukkan korelasi positif. Ini mengindikasikan bahwa nasabah dengan kapasitas finansial yang kuat dan stabilitas pekerjaan yang konsisten tinggi memiliki skor kredit lebih baik.
* Rasio Kewajiban terhadap pendapatan, jumlah transaksi perjudian menunjukkan korelasi negatif yang mengindikasikan bahwa beban finansial tinggi dan perilaku keuangan berisiko membuat skor kredit menurun.

### Sumber Data
Dataset: Financial Credibility & Loan Decision Dataset
Source: Kaggle
Author: Hrishit Patil
Link: https://www.kaggle.com/datasets/hrishitpatil/financial-credibility-and-loan-decision-dataset

