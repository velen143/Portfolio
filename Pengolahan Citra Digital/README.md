### Computer Vision & Image Processing Projects

### Overview

Repository ini berisi kumpulan proyek akademik yang berfokus pada pengolahan citra (*image processing*), segmentasi gambar (*image segmentation*), ekstraksi fitur, dan pencocokan citra menggunakan Python.

Proyek-proyek ini mengeksplorasi berbagai teknik pemrosesan gambar untuk mengidentifikasi objek, memisahkan area gambar, menganalisis karakteristik visual, dan melakukan pencarian citra berdasarkan kemiripan fitur.

### Projects

### 1. Analisis dan Segmentasi Gambar dengan Mahotas dan Scikit-image

Proyek ini mengeksplorasi berbagai teknik pengolahan dan segmentasi citra menggunakan pustaka Mahotas dan Scikit-image.

**Proses yang dilakukan:**
- Mengurangi noise dan melakukan thresholding pada gambar.
- Mendeteksi serta memberi label pada objek yang saling terhubung.
- Mengeksplorasi filter untuk menonjolkan struktur pada gambar retina.
- Melakukan segmentasi gambar menggunakan metode Felzenszwalb, SLIC, Quickshift, dan Watershed.
- Membandingkan hasil segmentasi melalui visualisasi.

**Tools:** Python, NumPy, Mahotas, Scikit-image, Matplotlib, SciPy.

### 2. Color-based Nearest Neighbors Image Retrieval

Proyek ini menerapkan pencarian citra berdasarkan kemiripan karakteristik warna dengan studi kasus identifikasi nominal uang kertas.

**Proses yang dilakukan:**
- Memuat citra referensi dan citra yang akan diuji.
- Mengekstraksi fitur warna berupa rata-rata kanal RGB dan fitur HSV.
- Menghitung jarak antara fitur citra uji dan citra referensi menggunakan Euclidean distance.
- Mengurutkan hasil berdasarkan jarak dan mengambil lima kandidat terdekat menggunakan pendekatan nearest neighbors.

**Tools:** Python, OpenCV, NumPy, Pandas, Matplotlib.

### 3. Deteksi Koin Menggunakan Segmentasi Gambar

Proyek ini bertujuan untuk mendeteksi dan menghitung jumlah koin pada gambar melalui teknik segmentasi citra.

**Proses yang dilakukan:**
- Mengubah gambar menjadi citra biner menggunakan Otsu thresholding.
- Memperbaiki hasil segmentasi dengan operasi morfologi.
- Menghilangkan objek yang menyentuh tepi gambar.
- Melakukan pelabelan objek dan menyaring objek berdasarkan luas area.
- Menghitung jumlah koin serta menampilkan bounding box dan nomor pada objek yang terdeteksi.

**Tools:** Python, NumPy, Matplotlib, Scikit-image, Pillow.

### Skills Demonstrated

- Image Processing
- Image Segmentation
- Feature Extraction
- Color-Based Image Retrieval
- Object Detection and Counting
- Image Visualization
- Python Programming
- Exploratory Experimentation with Image Processing Algorithms

### Conclusion

Ketiga proyek ini menunjukkan penerapan berbagai teknik Computer Vision dan Image Processing menggunakan Python, mulai dari segmentasi area gambar dan penghitungan objek hingga ekstraksi fitur warna dan pencarian citra berdasarkan kemiripan.

Repository ini menjadi dokumentasi pembelajaran dan eksperimen dalam memahami algoritma pengolahan citra serta penerapannya pada beberapa studi kasus.

