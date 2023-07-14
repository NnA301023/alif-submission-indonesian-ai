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

Pada tahap awal sesuai dengan alur dari data science life cycle, yaitu melakukan analisis data, salah satu insight yang paling krusial adalah meninjau distribusi label sentiment.
...

Kemudian disertai beberapa visualisasi wordcloud per masing-masing label sentiment
... 

Dari insight yang dimiliki ...

Tahap selanjutnya yakni melakukan pemrosesan data, dikarenakan data kali ini berupa teks, dan mesin hanya memahami angka, maka penulis menerapkan metode `Count Vectorization` untuk mengubah teks menjadi angka seperti yang terlihat pada gambar ...
![](https://www.researchgate.net/publication/354354484/figure/fig2/AS:1080214163595268@1634554534648/Illustration-of-count-vectorization.jpg)
<p align=center>hai</p>

### The Result


### Contact Person


## Dataset Information

Source dataset on this project is from twitter content about "Pelaksanaan Pilpres 2019", total rows of datsets is 1,815 row and contains sentiment `Positive`, `Negative`, and `Neutral`.

## Objective Outcome

Engineering should experiment with several preprocessing and vectorization algorithm then implement machine learning model such as random forest and LSTM with hyperparameter tuning.

## Project Breakdown

- [x] Objective Understanding
- [x] Apply Exploratory Data Analysis
- [x] Apply Several Preprocessing Algorithm
- [x] Apply ML Modeling and Benchmarking
- [x] Create Presentation Project