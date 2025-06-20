Bab 12: Custom Models and Training with TensorFlow File: 12_custom_models_and_training.ipynb
Tujuan Membangun pemahaman menyeluruh tentang bagaimana merancang model, loss function, dan loop pelatihan kustom menggunakan TensorFlow level rendah dengan tf.GradientTape.
Isi TensorFlow tidak hanya digunakan melalui Keras API, tapi juga memungkinkan kita membangun model dan proses pelatihan dari nol. Ini berguna dalam penelitian atau proyek yang memerlukan fleksibilitas penuh.
tf.GradientTape adalah cara paling penting dalam mendefinisikan loop pelatihan secara manual. Dengan fungsi ini, kita dapat merekam operasi selama forward pass dan menghitung gradien secara otomatis.
Kita juga dapat membuat layer kustom dengan mewarisi tf.keras.layers.Layer, dan membuat model kustom dengan mewarisi tf.keras.Model. Ini memberikan kontrol penuh terhadap forward pass dan struktur arsitektur.
Selain itu, kita belajar membuat loss function kustom dan metrik evaluasi yang tidak tersedia secara default. Bab ini juga membahas cara menyimpan dan memuat model secara manual menggunakan format SavedModel dan HDF5.
Visualisasi pelatihan dilakukan menggunakan TensorBoard, termasuk grafik loss, akurasi, dan arsitektur computational graph.

