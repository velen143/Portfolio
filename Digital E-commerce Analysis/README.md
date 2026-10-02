### Project : Analisis Digitalisasi Usaha E-Commerce Indonesia

### Overview

Proyek ini melakukan analisis data eksplorasi (EDA) terhadap usaha e-commerce di Indonesia berdasarkan data Statistik E-Commerce 2023 dari Badan Pusat Statistik (BPS). Analisis dilakukan untuk memahami pola penggunaan kanal penjualan, metode pembayaran, penggunaan marketplace, serta perbandingan antara pembayaran tunai dan pembayaran digital di berbagai provinsi di Indonesia.

### Tools

* Microsoft Excel
* Pivot Table
* Power BI
* DAX

### Alur Kerja

1. **Data Understanding (Pemahaman Data)**
   Tahap awal dilakukan dengan memahami struktur dataset, variabel yang tersedia, serta informasi mengenai kanal penjualan dan metode pembayaran usaha e-commerce berdasarkan provinsi.

2. **Data Validation & Cleaning (Validasi dan Pembersihan Data)**
   Melakukan pemeriksaan jumlah data, missing value, data duplikat, serta nilai yang berada di luar rentang yang sesuai. Data kemudian disiapkan untuk proses analisis tanpa mengubah nilai yang tidak tersedia menjadi nol.

3. **Data Transformation (Transformasi Data)**
   Membuat beberapa variabel tambahan untuk mendukung analisis, seperti Digital Payment, Cash vs Digital Payment, Marketplace Rank, dan Digital Payment Rank. Digital Payment dihitung berdasarkan gabungan Bank Transfer, Card, E-Wallet, dan QRIS.

4. **Exploratory Data Analysis (EDA)**
   Melakukan analisis terhadap rata-rata penggunaan kanal penjualan dan metode pembayaran serta membandingkan penggunaan marketplace dan digital payment antarprovinsi.

5. **Data Visualization & Dashboard**
   Hasil analisis divisualisasikan menggunakan Pivot Table, grafik, dan dashboard interaktif Power BI. Dashboard mencakup rata-rata penggunaan marketplace, digital payment, cash, instant messaging, kanal penjualan, metode pembayaran, serta perbandingan antarprovinsi.

### Hasil Analisis

- Instant Messaging menjadi kanal penjualan yang paling banyak digunakan dengan rata-rata sebesar 94,82%, diikuti oleh Social Media dengan penggunaan sekitar 50%.
- Marketplace memiliki rata-rata penggunaan sebesar 13,21%, lebih rendah dibandingkan Instant Messaging dan Social Media.
- Cash menjadi metode pembayaran yang paling dominan dengan rata-rata sebesar 79,96%, menunjukkan bahwa pembayaran tunai masih banyak digunakan oleh usaha e-commerce.
- Bank Transfer menjadi salah satu metode pembayaran digital yang cukup banyak digunakan, sedangkan E-Wallet, QRIS, dan Card memiliki penggunaan yang lebih rendah.
- Penggunaan marketplace menunjukkan variasi antarprovinsi. Sumatera Barat, Sulawesi Utara, dan Sumatera Selatan terlihat berada pada kelompok provinsi dengan penggunaan marketplace yang relatif tinggi.
- Secara umum, data menunjukkan bahwa usaha e-commerce lebih banyak memanfaatkan Instant Messaging dan Social Media sebagai kanal penjualan, sementara Cash masih mendominasi metode pembayaran.
  
### Sumber Data

* **Dataset:** Statistik E-Commerce 2023
* **Source:** Badan Pusat Statistik (BPS)
* **Publication:** Statistik E-Commerce 2023, Volume 6, 2025
* **Link:** https://www.bps.go.id/id/publication/2025/01/30/d52af11843aee401403ecfa6/statistik
