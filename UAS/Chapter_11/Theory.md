Bab 11: Training Deep Neural Networks File: 11_training_deep_neural_networks.ipynb
Tujuan Membahas tantangan dan teknik praktis dalam melatih jaringan saraf dalam (deep neural networks/DNN), termasuk masalah inisialisasi bobot, vanishing/exploding gradients, dan strategi regularisasi untuk meningkatkan performa model.
Isi Semakin dalam jaringan saraf, semakin besar pula tantangan dalam pelatihannya. Salah satu masalah klasik adalah vanishing gradient, yaitu saat nilai gradien menjadi sangat kecil sehingga tidak bisa mengupdate bobot di lapisan awal. Sebaliknya, exploding gradient membuat bobot menjadi sangat besar sehingga pelatihan menjadi tidak stabil.
Untuk mengatasi hal ini, digunakan metode He initialization dan Glorot/Xavier initialization yang menyesuaikan nilai awal bobot berdasarkan ukuran lapisan.
Batch Normalization juga diperkenalkan sebagai teknik untuk menstabilkan distribusi input ke setiap layer. Ini dilakukan dengan menormalisasi input layer terhadap mean dan standard deviation dalam mini-batch, lalu di-scale dan di-shift menggunakan parameter yang dapat dilatih.
Regularisasi seperti Dropout digunakan untuk mengurangi overfitting. Dropout secara acak menonaktifkan sejumlah neuron selama pelatihan agar jaringan tidak terlalu bergantung pada satu jalur informasi.
Selain itu, teknik learning rate scheduling seperti Time-based decay dan Exponential decay membantu menemukan dan mempertahankan kecepatan pelatihan optimal.
Berbagai optimizer canggih juga diperkenalkan, seperti Adam, RMSProp, dan Nadam yang menyatukan kelebihan momentum dan adaptasi learning rate otomatis.
Callback seperti ReduceLROnPlateau dan EarlyStopping membantu otomatisasi dalam pengendalian pelatihan.

