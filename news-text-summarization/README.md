# Project 2: Liputan6 Text Summarization

### Introduction


### Getting Started
Data yang digunakan dalam project kali ini bersumber dari `content berita` platform liputan6, dengan pembagian data menjadi canonical dan extreme yang menghasilkan sangat banyak berita untuk proses pelatihan dan evaluasi model teks summarization, secara garis besar teks summarization memiliki 2 tipe yaitu ekstraktif dan abstraktif, dimana ekstraktif ialah `teks kesimpulan yang dihasilkan dari kata-kata yang terdapat dalam source data / reference`, sedangkan abstraktif ialah `teks kesimpulan yang dihasilkan dari kata-kata corpus di dalam model machine learning yang bersifat semantik dengan kata-kata yang terdapat dalam source data / reference`.

Model Deep Learning yang digunakan:
  1. Model T5 (Text-to-Text Transfer Transformer):
     Kelebihan:
      a. Fleksibilitas Teks-ke-Teks: T5 dirancang dengan pendekatan "teks-ke-teks", yang berarti itu bisa digunakan untuk berbagai jenis tugas NLP dengan menyajikan masukan dan keluaran dalam format teks. Ini membuatnya lebih fleksibel dalam menangani berbagai macam tugas, termasuk summarisasi.
      b. Pemahaman Konteks Global: T5 dilatih dalam format tugas "pemetaan semua tugas menjadi pemrosesan sekuens ke sekuens", yang memungkinkannya untuk memahami konteks global dari teks yang lebih baik. Ini dapat membantu dalam menghasilkan ringkasan yang lebih baik, dengan mempertimbangkan hubungan antara bagian-bagian teks.
    
     Kekurangan:
      a. Kemungkinan Overfitting: Karena T5 sangat fleksibel dan memiliki banyak parameter, ada kemungkinan overfitting pada dataset kecil jika tidak dilatih dengan benar.
      b. Komputasi Berat: T5 adalah model yang cukup besar dan kompleks, yang dapat memerlukan sumber daya komputasi yang substansial untuk pelatihan dan penerapannya.

  2. Model Pegasus:
     Kelebihan: 
     a. Pendekatan Extractive-Abstractive: Pegasus menggunakan pendekatan campuran ekstraktif-abstraktif dalam summarisasinya. Ini berarti model dapat memilih frasa-frasa penting dari teks sumber (ekstraktif) dan juga menghasilkan kalimat-kalimat baru yang tidak ada dalam teks sumber (abstraktif), menghasilkan ringkasan yang lebih koheren.
     b. Pre-training pada Data Summarisasi Besar: Pegasus dilatih pada korpus besar yang berisi pasangan dokumen-ringkasan, yang memungkinkannya untuk memiliki pemahaman yang baik tentang struktur dan informasi yang relevan dalam teks yang perlu disusun ulang.
 
    Kekurangan:
    a. Ketergantungan pada Data Training: Karena Pegasus dilatih pada data summarisasi tertentu, performanya mungkin lebih baik dalam tugas-tugas summarisasi formal dan berita daripada dalam domain atau jenis teks yang berbeda.
    b. Keterbatasan Informatif Ekstraksi: Pendekatan ekstraktif Pegasus mungkin terbatas dalam mengekstrak informasi yang lebih kompleks atau tersembunyi dalam teks, karena hanya memilih frasa-frasa yang ada dalam teks sumber.

### The Result
Nama Model | Type Summarization | Rouge-1 (Recall) | Rouge-2 (Recall) | Rouge-L (Recall)
--- | --- | --- | --- | ---  
t5-base-indonesian-summarization-cased | Extractive | 92.3 | 76.0 | 92.3

### Contact Person
M. Alif Ramadhan, 19 Tahun (2003) dengan pengalaman professional di bidang Machine Learning 3 tahun.

[Tentang Saya Lebih Lanjut](https://www.dicoding.com/blog/belajar-di-idcamp-untuk-mengasah-skill-machine-learning/)