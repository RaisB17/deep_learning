Bab 19: Training and Deploying at Scale
File: 19_training_and_deploying_at_scale.ipynb
Tujuan
Membahas cara mengelola pelatihan model berskala besar dan men-deploy-nya ke sistem produksi secara efisien dan aman, termasuk proses versioning, monitoring, hingga pelatihan terdistribusi.
Isi
Pelatihan dan deployment model machine learning tidak hanya tentang akurasi tinggi di notebook. Model harus dapat digunakan dalam aplikasi nyata dan skalabel sesuai kebutuhan sistem produksi.
Terdapat dua cara umum deployment:
•	Batch inference: model dijalankan pada sejumlah besar data dalam siklus (harian/mingguan). Misalnya, memprediksi skor kredit bulanan.
•	Online inference: model disajikan sebagai web service (REST API) untuk prediksi real-time, seperti sistem rekomendasi produk.
Tantangan utama deployment:
•	Model versioning: memastikan model dapat dilacak, dikembalikan (rollback), dan dikelola secara aman di sistem produksi.
•	Monitoring performa: melacak akurasi, latency, error rate, dan drift distribusi input/output.
•	A/B testing dan Canary deployment: untuk mengevaluasi dua versi model secara bersamaan tanpa mengganggu seluruh sistem.
•	Latency dan Throughput: mempertahankan kecepatan tinggi dalam merespons permintaan prediksi.
Tool dan Teknologi:
•	TensorFlow Serving: sistem siap pakai untuk menyajikan model TensorFlow dalam produksi.
o	Mendukung hot swapping model (tanpa downtime).
o	API REST dan gRPC.
•	Vertex AI (Google Cloud):
o	Mendukung pelatihan besar-besaran dan hyperparameter tuning.
o	Fitur deployment otomatis, monitoring, dan MLOps terintegrasi.
•	TensorFlow.js: memungkinkan menjalankan model langsung di browser tanpa server (client-side inference).
•	TFLite dan Edge deployment: untuk perangkat mobile dan embedded (misalnya IoT), memungkinkan inferensi ringan dan efisien.
Pelatihan Skala Besar:
•	Distributed training:
o	Data parallelism: salinan model dilatih secara paralel di beberapa perangkat, masing-masing dengan subset data.
o	Model parallelism: model dibagi ke beberapa perangkat (berguna untuk model sangat besar).
•	Framework seperti PipeDream, Horovod, dan Pathways dari Google membantu mendistribusikan pelatihan dan inference secara efisien.
Best Practice Deployment:
•	Monitoring drift dan alert otomatis
•	Dokumentasi API model
•	Audit trail dan reproducibility
•	CI/CD untuk pipeline ML (MLOps)
Kesimpulan
Machine learning bukan hanya eksperimen, tetapi sistem produksi yang kompleks. Kesuksesan deployment tergantung pada kemampuan teknis dalam skalabilitas, monitoring, dan kolaborasi antar tim software engineering dan data science.

