Bab 14: Computer Vision dengan CNN File: 14_deep_computer_vision_with_cnns.ipynb
Tujuan Mengeksplorasi arsitektur Convolutional Neural Networks (CNNs) untuk pengolahan citra, serta bagaimana menerapkannya dalam klasifikasi gambar, deteksi objek, dan segmentasi.
Isi CNN dirancang khusus untuk memproses data grid seperti gambar. Komponen utamanya meliputi:
•	Convolutional layer: mengekstraksi fitur lokal seperti tepi dan pola
•	Pooling layer: mengurangi dimensi spasial dan mempercepat komputasi
•	Padding: menjaga ukuran output agar tetap konsisten
Beberapa arsitektur CNN yang dijelaskan antara lain:
•	LeNet-5: struktur klasik untuk MNIST
•	AlexNet: jaringan dalam pertama yang sukses di ImageNet
•	VGGNet: memperkenalkan konvolusi 3x3 bertumpuk
•	ResNet: memperkenalkan residual connections yang memungkinkan pelatihan jaringan sangat dalam
Transfer learning juga dibahas, yaitu memanfaatkan model pra-latih dan menyempurnakannya (fine-tuning) pada dataset baru. Teknik ini sangat berguna saat dataset kecil atau pelatihan dari awal terlalu mahal.
Untuk tugas lebih lanjut seperti deteksi objek, dikenalkan pendekatan seperti R-CNN dan YOLO.

