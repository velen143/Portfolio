### Project : Analisis Regresi Linear dengan PySpark

### Overview

Proyek ini menggunakan **PySpark** untuk membangun model regresi linear dalam menganalisis hubungan antara pengeluaran iklan pada beberapa media dengan jumlah penjualan. Analisis dilakukan dengan mempersiapkan data, membagi data menjadi data training dan testing, membangun model regresi linear, serta mengevaluasi hasil prediksi menggunakan beberapa metrik evaluasi.

### Tools

* Python
* PySpark
* Apache Spark
* Google Colab
* Spark MLlib

### Alur Kerja

1. **Data Understanding (Pemahaman Data)**
   Tahap awal dilakukan dengan membaca dataset menggunakan PySpark dan memeriksa struktur serta variabel yang tersedia. Dataset terdiri dari variabel pengeluaran iklan melalui **Handphone, TV, dan Radio**, serta **Penjualan** sebagai variabel target.

2. **Data Preparation (Persiapan Data)**
   Data dipisahkan menjadi variabel independen dan variabel target. Dataset kemudian dibagi menjadi **70% data training** dan **30% data testing** untuk proses pembangunan dan pengujian model.

3. **Feature Engineering**
   Menggunakan `VectorAssembler` untuk menggabungkan variabel **Handphone, TV, dan Radio** menjadi satu feature vector yang dapat digunakan oleh model machine learning PySpark.

4. **Modeling**
   Membangun model **Linear Regression** menggunakan Spark MLlib untuk mempelajari hubungan antara pengeluaran iklan dan penjualan.

5. **Model Evaluation (Evaluasi Model)**
   Model diuji menggunakan data testing dan dievaluasi menggunakan beberapa metrik, yaitu **RMSE, MAE, MSE, dan R²** untuk mengetahui tingkat kesalahan serta kemampuan model dalam menjelaskan variasi penjualan.

### Hasil Analisis

* Model regresi linear dapat digunakan untuk menganalisis hubungan antara pengeluaran iklan pada **Handphone, TV, dan Radio** dengan jumlah penjualan.
* Koefisien regresi yang dihasilkan model menunjukkan arah dan besarnya hubungan masing-masing variabel iklan terhadap penjualan ketika variabel lainnya diperhitungkan dalam model.
* **RMSE dan MAE** digunakan untuk mengetahui rata-rata besarnya kesalahan prediksi model.
* **MSE** digunakan untuk mengukur rata-rata kuadrat kesalahan prediksi, sehingga kesalahan yang lebih besar memiliki pengaruh yang lebih tinggi terhadap nilai evaluasi.
* **R² (R-squared)** digunakan untuk mengetahui seberapa besar variasi pada penjualan yang dapat dijelaskan oleh variabel pengeluaran iklan dalam model.
* Penggunaan **PySpark MLlib** menunjukkan penerapan framework Spark untuk proses machine learning, mulai dari pembentukan fitur, training model, hingga evaluasi hasil prediksi.
