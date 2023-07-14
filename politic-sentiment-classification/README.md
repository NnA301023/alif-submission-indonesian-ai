# Project 1: Politic Sentiment Analysis

### Introduction 
Pada tahun 2019 terdapat pemilihan umum presiden yang terdiri dari 2 oposisi yaitu kubu Jokowi dan kubu Prabowo, twitter sebagai salah satu platform sosial media yang memiliki banyak pengguna, juga turut serta membahas issue politik tersebut. 

Pada project kali ini, penulis akan menerapkan salah satu cabang keilmuan machine learning di bidang Natural Language Processing (NLP) yaitu Sentiment Analisis dengan menggunakan model machine learning dan deep learning di library `sklearn` dan `tensorflow` dengan tujuan untuk observasi sentiment pengguna twitter terkait issue pemilu yang terjadi di tahun 2019 yang harapannya dapat berguna bagi kedua pasangan calon presiden di tahun tersebut untuk mengevaluasi / memperbaiki citra sosial di masyarakat sehingga memperbesar peluang calon presiden dalam memenangkan pemilu di tahun 2019.

### Getting Started
Data yang digunakan pada project kali ini bersumber dari `data twitter` dengan keyword terkait `pemilu presiden 2019` dengan modul scrapping berupa tweepy dari free version API yang menghasilkan sekitar 1.815 baris data yang telah di lakukan pelabelan sentimen secara manual dari tim `indonesian-ai` dengan cakupan sentiment berupa: `positif`, `negatif`, dan `netral`.

Model machine learning dan deep learning yang digunakan yakni:
  1. Random Forest
     Kelebihan dan Kekurangan dari model Random Forest untuk kasus teks klasifikasi, 
     Kelebihan:
      - Performa dari Teknik Ensemble
      - Toleransi pada Label Imbalance (tidak seimbang)
      - Kemampuan Menangani Fitur Non-Relevant 
      - Skalabilitas

     Kekurangan:
      - Interpretasi yang Minim
      - Sensitif pada Data Noise
  2. Long Short Term Memory (LSTM)
     Kelebihan:
      - Pemahaman secara Kontekstual
      - Handling Relasi Entitas Teks
      - Fleksibilitas
    
     Kekurangan:
      - Cost Komputasi Tinggi
      - Membutuhkan Data yang Banyak
      - Rawan Overfitting
      - Interpretasi yang Minim

Pada tahap awal sesuai dengan alur dari data science life cycle, yaitu melakukan analisis data, salah satu insight yang paling krusial adalah meninjau distribusi label sentiment dan distribusi kata-kata yang mayoritas di setiap jenis sentiment.

Tahap selanjutnya yakni melakukan pemrosesan data, dikarenakan data kali ini berupa teks, dan mesin hanya memahami angka, maka penulis menerapkan metode `Count Vectorization` untuk mengubah teks menjadi angka dan `One Hot Encoder` untuk mengubah label sentiment menjadi indeks kategori.

Tahap modeling, dikarenakan perbandingan yang dilakukan mengaitkan aspek klasifikasi antara algoritma machine learning dan deep learning, maka salah satu metriks yang penulis gunakan dalam menentukan performa model yang paling optimal adalah dari metriks `akurasi uji` dikarenakan pada kasus ini label nya berupa `klasifikasi`.

### The Result
Nama Model | Parameters | Akurasi Latih (%) | Akurasi Uji (%)
---|---|---|---
Random Forest Baseline | Default | 100 | 59
Random Forest Tuning | `max depth = 15`, `n_estimators = 500`, `max_features = 'auto'` | 90 | 60
Bidirectional LSTM | 2,661,667 Trainable Parameters | 89.94 | 96.97

### Contact Person
M. Alif Ramadhan, 19 Tahun (2003) dengan pengalaman professional di bidang Machine Learning 3 tahun.

[Tentang Saya Lebih Lanjut](https://www.dicoding.com/blog/belajar-di-idcamp-untuk-mengasah-skill-machine-learning/)