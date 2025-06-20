Bab 16: NLP dengan RNN dan Attention File: 16_natural_language_processing_with_rnns_and_attention.ipynb
Tujuan Membangun sistem Natural Language Processing (NLP) modern yang memanfaatkan embedding kata, RNN, dan attention mechanism, dengan aplikasi utama dalam machine translation.
Isi NLP menangani teks dan bahasa alami. Teknik awal seperti one-hot encoding digantikan oleh word embedding (Word2Vec, GloVe) untuk representasi vektor yang padat dan bermakna.
Arsitektur Sequence-to-Sequence (Seq2Seq) digunakan untuk machine translation:
•	Encoder membaca seluruh input dan menghasilkan konteks (state)
•	Decoder menghasilkan output secara bertahap dari konteks tersebut
Bahdanau Attention memungkinkan decoder untuk fokus pada bagian input yang relevan di setiap langkah. Ini mengatasi keterbatasan Seq2Seq standar yang menyimpan semua informasi hanya dalam satu vektor konteks.
Teknik lainnya:
•	Masking untuk input/output dengan panjang berbeda
•	Beam search untuk decoding yang lebih optimal

