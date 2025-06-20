Bab 4: Pelatihan Model File: 04_training_models.ipynb
Tujuan Memahami bagaimana melatih model pembelajaran mesin secara efektif, dengan fokus pada regresi linear, optimisasi berbasis gradient descent, regularisasi untuk menghindari overfitting, dan penggunaan logistic regression untuk klasifikasi.
Isi Topik pertama yang dibahas adalah Linear Regression, salah satu model prediktif paling dasar. Dua pendekatan utama untuk pelatihan model ini diperkenalkan:
1.	Normal Equation – solusi eksak berbasis aljabar linier tanpa iterasi, cocok untuk dataset kecil.
2.	Gradient Descent – metode numerik iteratif yang skalabel untuk dataset besar.
Tiga variasi Gradient Descent dibahas:
•	Batch Gradient Descent: Menggunakan seluruh dataset untuk menghitung setiap langkah pembaruan parameter.
•	Stochastic Gradient Descent (SGD): Menggunakan satu contoh secara acak per iterasi. Lebih cepat, tapi hasilnya lebih fluktuatif.
•	Mini-batch Gradient Descent: Kombinasi keduanya, dengan mengambil batch kecil dari data.
Untuk menangani hubungan non-linear, Polynomial Regression diperkenalkan, yang menambah fitur berpangkat ke dalam data. Namun, ini dapat menimbulkan overfitting, sehingga perlu diterapkan regularisasi:
•	Ridge Regression (L2): Menambahkan penalti kuadrat terhadap besarnya koefisien.
•	Lasso Regression (L1): Menambahkan penalti absolut yang mendorong sparsity (beberapa fitur menjadi nol).
•	Elastic Net: Menggabungkan L1 dan L2.
Logistic Regression diperkenalkan sebagai model klasifikasi biner:
•	Menggunakan fungsi sigmoid untuk memetakan output ke dalam probabilitas antara 0 dan 1.
•	Ditraining menggunakan log loss (cross-entropy loss).
•	Softmax Regression (generalization dari logistic regression) digunakan untuk klasifikasi multi-kelas.
Teknik Early Stopping juga dijelaskan, yaitu menghentikan pelatihan saat performa validasi mulai memburuk. Ini berguna untuk menghindari overfitting saat menggunakan algoritma iteratif seperti Gradient Descent.
