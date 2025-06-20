Bab 15: Processing Sequences using RNNs and CNNs File: 15_processing_sequences_using_rnns_and_cnns.ipynb
Tujuan Mempelajari bagaimana model deep learning mengolah data sekuensial seperti teks, time-series, dan sinyal audio menggunakan RNN, LSTM, GRU, serta CNN satu dimensi.
Isi Model sekuens digunakan untuk prediksi data waktu (time-series) atau data yang urutannya penting.
Recurrent Neural Networks (RNN) mengolah input satu per satu sambil mempertahankan state tersembunyi antar langkah. Namun RNN klasik mengalami vanishing gradient.
Untuk mengatasinya:
•	LSTM (Long Short-Term Memory) dan GRU (Gated Recurrent Unit) digunakan untuk menangkap dependensi jangka panjang dengan mekanisme gating.
•	CNN 1D juga efektif untuk ekstraksi fitur lokal dari data sekuensial.
Topik lain:
•	Sequence padding dan masking untuk mengatasi panjang input yang bervariasi.
•	Forecasting time series dengan sliding window dan strategi prediksi multi-langkah.
Model dapat dievaluasi dengan metrik seperti MAE, RMSE, atau klasifikasi label sekuens.

