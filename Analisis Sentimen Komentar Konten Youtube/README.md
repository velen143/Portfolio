# Analisis Sentimen Komentar YouTube: Tingkat Kepercayaan Masyarakat terhadap Purbaya Yudhi Sadewa

## Deskripsi Proyek

Proyek ini bertujuan untuk mengeksplorasi tanggapan masyarakat terhadap Menteri Keuangan Purbaya Yudhi Sadewa melalui komentar pada video YouTube KompasTV yang membahas rapat perdana bersama DPR.

Analisis dilakukan menggunakan Python untuk mengumpulkan komentar, melakukan preprocessing teks, mengelompokkan sentimen berdasarkan kamus kata sederhana, serta mengidentifikasi kata dan frasa yang sering muncul melalui visualisasi data.

Proyek ini merupakan penerapan analisis teks untuk memperoleh gambaran awal mengenai opini masyarakat berdasarkan komentar yang dianalisis.

## Tujuan Analisis

- Mengumpulkan komentar masyarakat dari video YouTube KompasTV.
- Melakukan pembersihan dan normalisasi teks komentar berbahasa Indonesia.
- Mengelompokkan komentar ke dalam kategori sentimen berdasarkan kamus kata sederhana.
- Mengidentifikasi kata, bigram, dan trigram yang sering muncul.
- Menyajikan hasil analisis dalam bentuk grafik dan WordCloud.
- Menyusun insight awal sebagai bahan eksplorasi opini masyarakat.

## Sumber Data

Data diperoleh dari komentar pada video YouTube berikut:

- Kanal: KompasTV
- Topik: Rapat perdana Menteri Keuangan Purbaya Yudhi Sadewa bersama DPR
- Tautan video: https://www.youtube.com/watch?v=qQ-8TpS56to

Pengumpulan komentar dilakukan menggunakan library `youtube-comment-downloader`.

Jumlah komentar yang dianalisis mengikuti hasil scraping dan proses pembersihan data yang dijalankan.

## Tools dan Teknologi

- Python
- Pandas
- Matplotlib
- Seaborn
- NLTK
- Sastrawi
- Scikit-learn
- WordCloud
- YouTube Comment Downloader

## Metodologi

### 1. Scraping Data

Mengumpulkan komentar dari video YouTube KompasTV menggunakan Python dan menyimpannya ke dalam DataFrame untuk diproses lebih lanjut.

### 2. Case Folding

Mengubah seluruh teks komentar menjadi huruf kecil agar format teks menjadi seragam.

### 3. Analisis Sentimen Awal

Menggunakan kamus kata positif dan negatif sederhana untuk memberikan label sentimen pada komentar.

Kategori yang digunakan dalam kode awal:
- **Percaya:** skor kata lebih dari nol.
- **Kurang Percaya:** skor kata nol atau kurang.

Skor dihitung dengan menambahkan nilai untuk kata yang terdapat dalam kamus positif dan mengurangi nilai untuk kata dalam kamus negatif.

### 4. Preprocessing Teks

Tahapan preprocessing meliputi:

- Penghapusan emoji.
- Penghapusan tanda baca.
- Penghapusan spasi berlebih.
- Penghapusan stopword bahasa Indonesia.

### 5. Normalisasi Teks

Normalisasi dilakukan untuk membantu menyeragamkan teks komentar, meliputi:

- Stemming menggunakan Sastrawi.
- Penghapusan singkatan tertentu.
- Penghapusan stopword.
- Penghapusan kata berulang dalam satu komentar.
- Penghapusan komentar duplikat.

### 6. Analisis Frekuensi Kata dan Frasa

Menggunakan `CountVectorizer` dari Scikit-learn untuk menghitung frekuensi:

- **WordCloud:** visualisasi kata yang sering muncul dalam kumpulan komentar.
- **Bigram:** analisis frekuensi pasangan dua kata.
- **Trigram:** analisis frekuensi rangkaian tiga kata.

### 7. Visualisasi Data

Hasil analisis divisualisasikan menggunakan Matplotlib dan disimpan dalam format PDF, meliputi WordCloud, grafik 10 bigram teratas, dan grafik 10 trigram teratas.

## Insight yang Ingin Digali

Analisis ini digunakan untuk mengeksplorasi:

- Kecenderungan tanggapan masyarakat terhadap Purbaya Yudhi Sadewa.
- Kata dan frasa yang sering muncul dalam komentar.
- Tema pembicaraan yang dominan pada komentar.
- Perbedaan antara komentar yang terindikasi mendukung dan komentar yang terindikasi meragukan.

Insight akhir perlu disusun berdasarkan hasil grafik dan pemeriksaan komentar asli. Hasil analisis tidak otomatis mewakili tingkat kepercayaan seluruh masyarakat Indonesia.

## Keterbatasan Analisis

- Data berasal dari satu video YouTube sehingga tidak mewakili seluruh opini masyarakat.
- Komentar YouTube merupakan data yang tidak dipilih secara acak.
- Klasifikasi sentimen menggunakan kamus kata sederhana sehingga belum mampu memahami konteks, sarkasme, negasi, dan ironi secara akurat.
- Kamus kata perlu dievaluasi karena beberapa kata dapat memiliki makna berbeda sesuai konteks.
- Penghapusan kata dan normalisasi dapat mengubah makna komentar jika tidak dilakukan secara hati-hati.
- Frekuensi kata tidak selalu menunjukkan tingkat dukungan atau kepercayaan seseorang.

Oleh karena itu, hasil analisis sebaiknya dipahami sebagai eksplorasi awal terhadap komentar yang dikumpulkan, bukan sebagai pengukuran langsung tingkat kepercayaan seluruh masyarakat.

## Kesimpulan

Proyek ini menunjukkan penerapan Python untuk pengumpulan data komentar YouTube, preprocessing teks bahasa Indonesia, analisis sentimen berbasis kamus, serta visualisasi frekuensi kata dan frasa.

Hasilnya dapat membantu mengidentifikasi tema pembicaraan dan kecenderungan opini dalam kumpulan komentar yang dianalisis. Pengembangan selanjutnya dapat dilakukan dengan memperbaiki kamus sentimen, memvalidasi hasil klasifikasi secara manual, dan menggunakan metode analisis sentimen yang lebih kontekstual.

## Penulis

Proyek Portofolio Data Analyst

