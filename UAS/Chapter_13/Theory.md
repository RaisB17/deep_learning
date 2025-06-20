Bab 13: Loading and Preprocessing Data with TensorFlow File: 13_loading_and_preprocessing_data.ipynb
Tujuan Mengajarkan cara membangun pipeline data yang efisien dan scalable menggunakan tf.data, TFRecord, serta teknik augmentasi data untuk meningkatkan performa model.
Isi Agar pelatihan deep learning berjalan cepat dan efisien, data perlu dimuat dan diproses secara optimal. tf.data API menyediakan cara membangun pipeline input dari berbagai sumber, seperti CSV, TFRecord, atau generator Python.
Langkah umum dalam pipeline ini meliputi:
•	Membaca data dari file (misalnya dengan tf.data.TFRecordDataset)
•	Parsing dan decoding (misalnya dari format Protobuf)
•	Augmentasi (rotasi, flipping, cropping, dsb.)
•	Normalisasi data
•	Shuffling, batching, dan prefetching
Dengan menggabungkan teknik ini, kita dapat menciptakan input pipeline yang tidak menjadi bottleneck pelatihan. Data augmentation juga memperluas dataset secara virtual, membantu model menjadi lebih robust.

