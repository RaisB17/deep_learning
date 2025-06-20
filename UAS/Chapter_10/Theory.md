Bab 10: Jaringan Saraf Tiruan dengan Keras File: 10_neural_nets_with_keras.ipynb
Tujuan Menyediakan pengantar ke jaringan saraf tiruan (Artificial Neural Networks/ANN) dan cara membangunnya menggunakan library Keras di TensorFlow.
Isi ANN terdiri dari unit-unit sederhana (neuron buatan) yang mengalirkan informasi dari input ke output melalui lapisan-lapisan tersembunyi (hidden layers). Model ini bersifat universal dan mampu menangkap hubungan non-linear yang kompleks.
Fungsi aktivasi memainkan peran penting:
•	ReLU (Rectified Linear Unit) mempercepat konvergensi dan mencegah vanishing gradient.
•	Sigmoid digunakan untuk output biner, sedangkan softmax untuk klasifikasi multi-kelas.
Keras menyediakan tiga cara membangun model:
1.	Sequential API: cocok untuk model linear satu arah dari input ke output
2.	Functional API: memungkinkan model dengan arsitektur bercabang atau berulang
3.	Model Subclassing: memberikan fleksibilitas penuh dalam desain arsitektur dan proses training
Model dikompilasi dengan compile() yang menentukan loss function dan optimizer. Pelatihan dilakukan dengan fit(), evaluasi dengan evaluate(), dan prediksi dengan predict().
Fasilitas callback seperti EarlyStopping dan ModelCheckpoint memungkinkan kontrol pelatihan agar berhenti saat validasi memburuk atau menyimpan model terbaik secara otomatis. Visualisasi menggunakan TensorBoard memberikan wawasan tentang proses pelatihan secara real-time.

