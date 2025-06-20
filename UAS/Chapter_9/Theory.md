Bab 9: Teknik Unsupervised Learning File: 09_unsupervised_learning.ipynb
Tujuan Menjelaskan berbagai metode pembelajaran tanpa label (unsupervised learning), termasuk clustering, estimasi kepadatan, dan deteksi anomali. Teknik ini berguna ketika label tidak tersedia, atau ketika ingin memahami struktur internal data.
Isi Clustering adalah salah satu tugas utama dalam unsupervised learning. Dalam clustering, data dikelompokkan ke dalam klaster berdasarkan kemiripan antar instansinya. Beberapa algoritma populer:
•	K-Means: algoritma sederhana namun efektif, bekerja dengan meminimalkan jarak dalam klaster ke pusat (centroid). Kelemahan utamanya adalah harus menentukan jumlah klaster di awal.
•	DBSCAN: mengelompokkan berdasarkan densitas. Tidak memerlukan jumlah klaster sebelumnya dan bisa mengidentifikasi outlier.
•	Hierarchical Clustering: membentuk pohon hierarki klaster dan dapat divisualisasikan dalam bentuk dendrogram.
Gaussian Mixture Models (GMM) menggunakan pendekatan probabilistik di mana data diasumsikan berasal dari gabungan beberapa distribusi normal. GMM dapat memberikan probabilitas keanggotaan, berbeda dengan K-Means yang keras (hard assignment).
Anomaly Detection digunakan untuk mengidentifikasi data yang tidak sesuai dengan pola umum. Contohnya, mendeteksi penipuan transaksi, kesalahan produksi, atau aktivitas janggal dalam jaringan komputer.

