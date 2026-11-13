# Analisis Sentimen Ulasan Subway Surfers

## Deskripsi Proyek

Proyek ini bertujuan untuk menganalisis ulasan pengguna game Subway Surfers yang diperoleh dari Google Play Store. Analisis dilakukan menggunakan Python untuk memahami tanggapan pengguna, mengidentifikasi keluhan yang sering muncul, dan memberikan rekomendasi perbaikan berdasarkan hasil pengolahan data.

## Tujuan Analisis

- Mengumpulkan ulasan pengguna dari Google Play Store.
- Melakukan pembersihan dan preprocessing teks.
- Mengelompokkan ulasan berdasarkan rating menjadi sentimen positif dan negatif.
- Mengidentifikasi kata-kata yang sering muncul pada ulasan positif dan negatif.
- Menyajikan hasil analisis dalam bentuk visualisasi.
- Memberikan rekomendasi untuk meningkatkan pengalaman pengguna.

## Dataset

Dataset diperoleh melalui proses scraping ulasan game Subway Surfers pada Google Play Store Indonesia.

Jumlah data yang dikumpulkan: 200 ulasan.

Kolom utama yang digunakan:
- `ulasan`: Teks ulasan yang ditulis oleh pengguna.
- `label`: Rating pengguna dalam skala 1–5.
- `sentimen`: Kategori sentimen berdasarkan rating.

## Tools dan Teknologi

- Python
- Pandas dan NumPy
- Google Play Scraper
- NLTK
- Sastrawi
- Matplotlib
- Seaborn
- WordCloud

## Tahapan Analisis

### 1. Pengambilan Data

Mengumpulkan 200 ulasan pengguna Subway Surfers menggunakan library Google Play Scraper.

### 2. Case Folding

Mengubah seluruh teks ulasan menjadi huruf kecil agar format teks menjadi seragam.

### 3. Cleaning

Menghapus tanda baca dari teks ulasan untuk membantu proses pengolahan teks.

### 4. Tokenisasi

Memisahkan kalimat menjadi kata-kata menggunakan NLTK.

### 5. Stopword Removal

Menghapus kata-kata yang termasuk dalam daftar stopword bahasa Indonesia.

### 6. Stemming

Mengubah kata menjadi bentuk dasarnya menggunakan library Sastrawi.

### 7. Kategorisasi Sentimen

Mengelompokkan ulasan berdasarkan rating:
- Rating 1–2: Negatif.
- Rating 3–5: Positif.

Kategorisasi ini mengikuti aturan yang digunakan dalam kode analisis.

### 8. Visualisasi Data

Membuat WordCloud untuk melihat kata-kata yang sering muncul pada ulasan positif dan negatif, serta diagram batang untuk menampilkan 20 kata yang paling sering muncul pada ulasan negatif.

## Hasil dan Insight

Analisis ini digunakan untuk mengeksplorasi tanggapan pengguna terhadap permainan, termasuk kemungkinan keluhan mengenai performa game, penyimpanan progres dan koin, serta kebutuhan akan fitur atau inovasi baru.

Temuan tersebut perlu diperiksa kembali berdasarkan ulasan asli dan hasil visualisasi sebelum dijadikan kesimpulan akhir.

## Rekomendasi

Berdasarkan tema keluhan yang ditemukan, beberapa rekomendasi yang dapat dipertimbangkan adalah:

1. Melakukan evaluasi dan perbaikan bug untuk meningkatkan stabilitas permainan.
2. Memeriksa mekanisme penyimpanan progres permainan dan koin agar data pengguna tidak hilang.
3. Mengevaluasi masukan pengguna untuk mengembangkan fitur dan event yang lebih menarik.

## Keterbatasan Analisis

- Dataset hanya terdiri dari 200 ulasan sehingga belum tentu mewakili seluruh pengguna.
- Kategori sentimen ditentukan berdasarkan rating, bukan melalui model machine learning yang memprediksi sentimen dari isi teks.
- Rating 3 dimasukkan ke kategori positif sesuai aturan pada kode.
- Frekuensi kata tidak selalu menunjukkan tingkat keparahan suatu keluhan.

## Kesimpulan

Proyek ini menunjukkan penerapan Python untuk mengumpulkan dan mengolah data ulasan, melakukan preprocessing teks, mengidentifikasi kata yang sering muncul, serta menghasilkan insight awal mengenai pengalaman pengguna. Hasil analisis dapat
