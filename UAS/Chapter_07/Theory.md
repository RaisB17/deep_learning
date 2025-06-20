Bab 7: Ensemble Learning dan Random Forests File: 07_ensemble_learning_and_random_forests.ipynb
Tujuan Memperkenalkan konsep ensemble learning, yakni strategi untuk menggabungkan beberapa model lemah menjadi satu model kuat yang lebih akurat dan stabil. Teknik ini telah terbukti meningkatkan performa hampir semua jenis algoritma dasar.
Isi Ensemble learning terdiri dari dua pendekatan utama: Bagging dan Boosting.
Bagging (Bootstrap Aggregating) adalah metode di mana beberapa model dilatih secara paralel pada subset data yang berbeda, biasanya diambil dengan pengambilan sampel acak (bootstrap). Hasil dari semua model digabungkan untuk membuat prediksi akhir. Contoh paling terkenal dari metode ini adalah Random Forest.
Random Forest merupakan kumpulan decision tree yang dilatih dengan bagging, ditambah dengan pemilihan subset fitur secara acak saat pemisahan pada setiap node. Hal ini mengurangi korelasi antar pohon dan meningkatkan generalisasi. Random Forest secara default menghitung feature importance, menyediakan metrik untuk memahami seberapa penting masing-masing fitur terhadap hasil prediksi.
Boosting, di sisi lain, melatih model secara berurutan di mana setiap model berikutnya berusaha memperbaiki kesalahan model sebelumnya. Algoritma populer dalam boosting meliputi AdaBoost dan Gradient Boosting. Boosting lebih rentan terhadap overfitting, namun jika disetel dengan baik bisa sangat kuat.
Selain itu, stacking adalah metode ensemble yang melatih model meta di atas prediksi model dasar. Ini memungkinkan penggunaan kekuatan berbagai algoritma secara bersamaan.

