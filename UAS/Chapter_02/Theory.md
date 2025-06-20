Bab 2: Proyek Machine Learning End-to-End File: 02_end_to_end_machine_learning_project.ipynb
Tujuan Memberikan gambaran praktis tentang seluruh proses membangun sistem pembelajaran mesin dari awal sampai deployment, melalui studi kasus prediksi harga rumah di California.
Langkah-langkah Proyek
1.	Definisi Masalah: Masalah dipahami sebagai regresi, karena output berupa nilai numerik (harga rumah).
2.	Pengumpulan Data: Data didapat dari sumber terbuka dan dibersihkan dari error atau anomali.
3.	Eksplorasi Data: Statistik deskriptif dilakukan untuk memahami distribusi data. Visualisasi digunakan untuk melihat korelasi antar fitur, seperti antara jumlah kamar dan harga.
4.	Pembagian Data: Data dibagi ke dalam set pelatihan dan pengujian menggunakan train_test_split dan StratifiedShuffleSplit untuk menjaga distribusi yang seimbang.
5.	Prapemrosesan Data:
o	Menangani nilai kosong (missing value) menggunakan imputasi.
o	Encoding data kategorikal menggunakan one-hot encoding.
o	Normalisasi fitur numerik.
o	Pembuatan pipeline otomatis untuk preprocessing agar proses menjadi konsisten dan dapat direproduksi.
6.	Pelatihan Model Awal: Model-model seperti Linear Regression dan Decision Tree dilatih untuk menetapkan baseline performa.
7.	Evaluasi: RMSE digunakan sebagai metrik utama. Cross-validation meningkatkan keandalan evaluasi.
8.	Penyetelan Hyperparameter: Dilakukan menggunakan GridSearchCV atau RandomizedSearchCV.
9.	Evaluasi Akhir: Model terbaik diuji pada test set yang belum pernah dilihat model.
10.	Persiapan Deployment: Model disimpan dalam format siap produksi (misalnya joblib), dan siap digunakan dalam sistem real-time atau batch.
Pendekatan end-to-end ini mencerminkan workflow nyata di industri dan memberikan pemahaman menyeluruh tentang siklus hidup proyek machine learning.
