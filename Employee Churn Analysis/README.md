### Analisis Karakteristik dan Faktor Penentu Karyawan yang Resign (Employee Churn Analysis)

### Overview

Proyek ini bertujuan untuk menganalisis karakteristik karyawan dan mengidentifikasi faktor-faktor yang berkaitan dengan keputusan karyawan untuk meninggalkan perusahaan (*employee churn*). Analisis dilakukan menggunakan Python untuk memahami distribusi data, membandingkan karakteristik karyawan yang bertahan dan resign, serta menguji hubungan antara variabel demografis dan pekerjaan dengan keputusan resign.

### Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

### Alur Kerja

1. **Data Understanding**  
   Memahami struktur dataset, tipe data, jumlah data, serta distribusi variabel target `LeaveOrNot`.

2. **Data Quality Checking**  
   Memeriksa nilai yang hilang (*missing values*) dan meninjau kelengkapan data pada variabel target maupun atribut lainnya.

3. **Exploratory Data Analysis (EDA)**  
   Menganalisis distribusi variabel numerik menggunakan histogram, membandingkan usia karyawan berdasarkan status resign menggunakan boxplot, serta mengeksplorasi karakteristik karyawan berdasarkan tingkat pendidikan.

4. **Statistical Hypothesis Testing**  
   Menggunakan independent t-test untuk membandingkan karakteristik numerik antara karyawan yang bertahan dan resign, serta uji Chi-Square untuk mengevaluasi hubungan antara tingkat pendidikan dan status karyawan.

5. **Correlation Analysis**  
   Menganalisis korelasi antarvariabel numerik untuk mengidentifikasi variabel yang memiliki hubungan linear dengan keputusan resign.

6. **Insight & Conclusion**  
   Merangkum hasil analisis untuk memahami karakteristik karyawan yang berkaitan dengan employee churn dan memberikan dasar bagi evaluasi strategi retensi karyawan.

### Hasil Analisis

1. **Payment Tier:** Tingkat pembayaran menjadi salah satu variabel yang perlu diperhatikan dalam analisis keputusan resign berdasarkan hasil korelasi yang diperoleh.
2. **Education:** Tingkat pendidikan menunjukkan hubungan dengan status resign berdasarkan analisis yang dilakukan. Perbedaan tingkat resign perlu dievaluasi menggunakan proporsi pada setiap kelompok pendidikan.
3. **Age:** Perbedaan usia antara karyawan yang bertahan dan resign dievaluasi menggunakan uji statistik untuk mengetahui apakah perbedaannya signifikan.
4. **Employee Retention:** Hasil analisis dapat menjadi bahan pertimbangan awal bagi perusahaan untuk mengevaluasi kebijakan kompensasi dan strategi mempertahankan karyawan.

