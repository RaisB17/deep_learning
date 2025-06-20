Bab 6: Decision Trees File: 06_decision_trees.ipynb
Tujuan Bab ini bertujuan menjelaskan dasar-dasar decision tree sebagai algoritma yang sangat intuitif namun cukup kuat untuk tugas klasifikasi dan regresi. Decision tree digunakan untuk membagi dataset menjadi subset yang lebih kecil berdasarkan fitur tertentu agar prediksi dapat dilakukan dengan baik.
Isi Decision tree bekerja dengan membagi data secara rekursif pada titik-titik yang memaksimalkan "impurity reduction". Impurity dapat dihitung menggunakan Gini impurity atau Entropy. Pemilihan fitur dan nilai split dilakukan secara greedy, yaitu pada setiap node dipilih split terbaik tanpa mempertimbangkan dampak ke seluruh struktur pohon.
Keunggulan utama decision tree adalah kemudahannya untuk diinterpretasikan dan divisualisasikan. Namun, jika tidak dikontrol, decision tree sangat rentan terhadap overfitting karena bisa membelah data sampai sempurna pada training set.
Untuk mencegah overfitting, beberapa parameter digunakan seperti:
•	max_depth: membatasi kedalaman maksimal pohon
•	min_samples_split: jumlah minimum sampel untuk melakukan split
•	min_samples_leaf: jumlah minimum sampel yang harus ada pada sebuah daun pohon
Selain itu, pruning dapat dilakukan setelah pohon dilatih, yaitu memangkas cabang yang tidak memberikan kontribusi berarti pada akurasi validasi.
Scikit-Learn menyediakan visualisasi dan ekspor struktur pohon melalui fungsi plot_tree dan export_graphviz, serta parameter lain untuk eksplorasi dan penyetelan model lebih lanjut.

