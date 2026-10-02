### Project : Analisis Kualitas Udara DKI Jakarta

### Overview

Proyek ini melakukan analisis data eksplorasi (EDA) pada data kualitas udara DKI Jakarta untuk mengetahui pola dan karakteristik kualitas udara berdasarkan kategori kualitas udara, parameter pencemar kritis, stasiun pemantauan, dan periode pengamatan. Dataset awal terdiri dari 3.502 data, kemudian setelah melalui proses data cleaning diperoleh 3.480 data yang digunakan untuk analisis.

### Tools

- MySQL
- SQL
- Power BI
- DAX
- phpMyAdmin

### Alur Kerja

1. **Data Understanding (Pemahaman Data)**  
   Tahap awal dilakukan dengan memahami struktur dataset, jumlah data, kolom, tipe data, kategori kualitas udara, parameter pencemar, stasiun pemantauan, serta periode pengamatan.

2. **Data Cleaning (Pembersihan Data)**  
   Proses pembersihan dilakukan menggunakan SQL dengan menghapus data yang tidak valid, melakukan pengecekan missing value dan data duplikat, serta melakukan standardisasi nama stasiun pemantauan. Data diproses melalui tabel air_quality_raw, air_quality_clean, dan air_quality_final.

3. **Exploratory Data Analysis (EDA)**  
   Analisis dilakukan menggunakan SQL untuk mengetahui distribusi kategori kualitas udara, frekuensi parameter pencemar kritis, rata-rata parameter pencemar, kondisi berdasarkan stasiun, nilai MAX tertinggi, serta perubahan nilai MAX berdasarkan periode.

4. **Data Visualization**  
   Hasil analisis divisualisasikan menggunakan Power BI dalam bentuk dashboard interaktif yang menampilkan KPI, distribusi kategori kualitas udara, parameter pencemar, tren bulanan, dan perbandingan antarstasiun.

### Hasil Analisis

- Kategori **SEDANG** merupakan kategori kualitas udara yang paling banyak ditemukan, dengan 2.694 data atau 77,41% dari keseluruhan data yang dianalisis.

- **PM2.5** merupakan parameter pencemar kritis yang paling sering tercatat, dengan 2.955 data atau 84,91% dari keseluruhan data.

- Berdasarkan perhitungan rata-rata parameter, PM2.5 memiliki nilai rata-rata numerik tertinggi sebesar 70,58, diikuti PM10 sebesar 45,47, SO2 sebesar 35,67, NO2 sebesar 26,83, O3 sebesar 23,62, dan CO sebesar 14,97.

- Distribusi kategori kualitas udara berbeda pada setiap stasiun pemantauan. Lima stasiun yang dianalisis adalah DKI1 Bundaran Hotel Indonesia, DKI2 Kelapa Gading, DKI3 Jagakarsa, DKI4 Lubang Buaya, dan DKI5 Kebon Jeruk.

- DKI5 Kebon Jeruk memiliki rata-rata nilai MAX tertinggi sebesar 76,56, sedangkan nilai MAX individu tertinggi sebesar 202 tercatat di DKI3 Jagakarsa pada Februari 2024 dengan kategori **SANGAT TIDAK SEHAT**.

- Rata-rata nilai MAX bulanan tertinggi tercatat pada Juni 2025 dengan nilai 94,83. Hal ini menunjukkan adanya perubahan nilai MAX sepanjang periode pengamatan.

- Dashboard Power BI digunakan untuk membantu melihat distribusi kualitas udara, parameter pencemar kritis, tren nilai MAX, serta perbedaan kondisi antarstasiun secara lebih interaktif.

### Sumber Data

- **Dataset:** Data Kualitas Udara / ISPU DKI Jakarta
- **Source:** Data resmi kualitas udara DKI Jakarta
- **Publisher:** Pemerintah Provinsi DKI Jakarta
- **Link:** https://data.go.id/instantion/provinsi-dki-jakarta?q=ispu&utm_source
