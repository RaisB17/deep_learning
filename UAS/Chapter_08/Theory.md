Bab 8: Reduksi Dimensi File: 08_dimensionality_reduction.ipynb
Tujuan Menjelaskan cara-cara mengurangi jumlah fitur dalam data tanpa kehilangan informasi penting. Reduksi dimensi sangat bermanfaat untuk visualisasi, mempercepat pelatihan model, dan menghindari overfitting.
Isi Reduksi dimensi membantu menangani curse of dimensionality, yaitu ketika jumlah fitur sangat besar sehingga jarak antar data menjadi tidak berarti.
Teknik yang paling mendasar adalah Principal Component Analysis (PCA), yang mentransformasikan data ke dalam komponen utama (principal components) berdasarkan arah varian terbesar. PCA bersifat linier dan dapat digunakan untuk kompresi data atau sebagai langkah preprocessing.
Untuk kasus non-linear, digunakan Kernel PCA yang menerapkan fungsi kernel (misalnya RBF) untuk memetakAan data ke ruang berdimensi lebih tinggi sebelum dilakukan PCA.
Alternatif lainnya termasuk:
•	t-SNE: sangat baik untuk visualisasi 2D/3D tetapi tidak cocok untuk prediksi karena tidak mempertahankan struktur global
•	LLE (Locally Linear Embedding): cocok untuk pelestarian hubungan lokal
•	Random Projection: teknik yang efisien namun dengan akurasi yang lebih rendah
Semua metode ini bisa diterapkan untuk memahami struktur internal data dan memperbaiki performa model.

