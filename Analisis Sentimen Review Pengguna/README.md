### Project : Analisis Sentimen Review Pengguna Wattpad dan Fizzo Novel

### Overview

Proyek ini melakukan analisis sentimen terhadap ulasan pengguna **Wattpad dan Fizzo Novel** yang diperoleh dari Google Play Store. Analisis bertujuan untuk memahami distribusi sentimen pengguna, membandingkan kedua aplikasi, mengidentifikasi kata atau frasa yang sering muncul, serta membangun model klasifikasi sentimen menggunakan machine learning.

### Tools

* Python
* Pandas
* NLTK
* Sastrawi
* Scikit-learn
* Matplotlib
* WordCloud
* Google Play Scraper

### Alur Kerja

1. **Data Collection (Pengumpulan Data)**
   Mengambil data ulasan pengguna Wattpad dan Fizzo Novel dari Google Play Store menggunakan `google-play-scraper`. Data yang dikumpulkan mencakup isi komentar dan rating pengguna.

2. **Data Cleaning & Text Preprocessing (Pembersihan Data)**
   Membersihkan data teks dengan menghapus emoji, URL, karakter yang tidak diperlukan, stopwords, serta melakukan normalisasi kata slang dan stemming Bahasa Indonesia menggunakan Sastrawi.

3. **Sentiment Labeling (Pelabelan Sentimen)**
   Memberikan label sentimen berdasarkan rating pengguna:

   * Rating 1–2 → Negatif
   * Rating 3 → Netral
   * Rating 4–5 → Positif

   Label kemudian divalidasi menggunakan kamus sentimen untuk membandingkan hasil berdasarkan rating dengan isi komentar.

4. **Exploratory Data Analysis (EDA)**
   Menganalisis distribusi sentimen sebelum dan sesudah validasi serta membandingkan karakteristik sentimen antara Wattpad dan Fizzo Novel. Hasil analisis divisualisasikan menggunakan bar chart.

5. **Text Analysis**
   Menggunakan **WordCloud** dan analisis **4-gram** untuk mengidentifikasi kata serta kombinasi kata yang sering muncul pada masing-masing kategori sentimen.

6. **Machine Learning**
   Mengubah teks menjadi representasi numerik menggunakan **TF-IDF**, kemudian membangun model **Multinomial Naive Bayes** untuk melakukan klasifikasi sentimen. Model dievaluasi menggunakan accuracy dan classification report.

7. **Hyperparameter Tuning**
   Melakukan tuning terhadap parameter `alpha` pada model Multinomial Naive Bayes menggunakan **GridSearchCV** untuk memperoleh model dengan konfigurasi yang lebih sesuai.

### Hasil Analisis

* Analisis menghasilkan distribusi sentimen pengguna Wattpad dan Fizzo Novel berdasarkan rating serta validasi menggunakan isi komentar.
* Perbandingan sebelum dan sesudah validasi menunjukkan adanya perubahan pada sebagian label sentimen ketika rating dibandingkan dengan hasil analisis berbasis kamus.
* WordCloud digunakan untuk melihat kata-kata yang sering muncul pada sentimen positif, netral, dan negatif.
* Analisis 4-gram digunakan untuk menemukan kombinasi empat kata yang sering muncul dalam masing-masing kategori sentimen.
* Model **Multinomial Naive Bayes** digunakan untuk mengklasifikasikan ulasan pengguna berdasarkan fitur TF-IDF.
* Model kemudian dilakukan **hyperparameter tuning menggunakan GridSearchCV** untuk membandingkan performa model sebelum dan sesudah tuning.

