Bab 5: Support Vector Machines (SVM) File: 05_support_vector_machines.ipynb
Tujuan Memahami teori dan penerapan algoritma SVM untuk klasifikasi dan regresi, termasuk konsep margin maksimum, kernel trick, dan implementasi untuk data non-linear.
Isi SVM bekerja Bab 4: Pelatihan Model File: 04_training_models.ipynb
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
________________________________________
dengan prinsip margin maksimal, yaitu mencari hyperplane yang memisahkan kelas dengan jarak sejauh mungkin dari data terdekat (disebut support vectors). Dalam Soft Margin Classification, model diizinkan membuat sedikit kesalahan klasifikasi untuk mendapatkan margin yang lebih luas dan lebih general.
Parameter C mengontrol tingkat kompromi antara margin dan error:
•	C besar → lebih sedikit toleransi kesalahan → margin sempit
•	C kecil → lebih banyak toleransi kesalahan → margin lebih lebar
Untuk data non-linearly separable, digunakan teknik kernel trick, yang memproyeksikan data ke dimensi lebih tinggi tanpa eksplisit menghitung koordinat tersebut. Beberapa kernel yang umum digunakan:
•	Polynomial Kernel: Cocok untuk data dengan batas keputusan melengkung.
•	Radial Basis Function (RBF): Menangani berbagai macam data non-linear.
Selain klasifikasi, SVM juga dapat digunakan untuk regresi melalui Support Vector Regression (SVR). Dalam SVR, model memprediksi nilai dengan mempertahankan margin toleransi tertentu (epsilon) dari nilai aktual.
Implementasi praktis:
•	Untuk dataset kecil hingga menengah: gunakan SVC, SVR dengan kernel.
•	Untuk dataset besar: gunakan LinearSVC atau SGDClassifier karena lebih efisien.
SVM sangat sensitif terhadap skala fitur, sehingga normalisasi fitur sangat penting sebelum pelatihan.

