Bab 17: Autoencoders dan GANs File: 17_autoencoders_and_gans.ipynb
Tujuan Menjelaskan dua pendekatan generatif: autoencoders untuk merekonstruksi input dan GAN (Generative Adversarial Networks) untuk membuat data baru.
Isi Autoencoder terdiri dari:
•	Encoder: mengubah input ke representasi laten
•	Decoder: merekonstruksi kembali input dari representasi tersebut
Variasi:
•	Denoising Autoencoder: belajar merekonstruksi input dari versi yang terdistorsi
•	Variational Autoencoder (VAE): menambahkan elemen probabilistik pada representasi laten, cocok untuk generasi konten baru
GAN terdiri dari dua jaringan:
•	Generator: menghasilkan data tiruan
•	Discriminator: membedakan mana data asli dan mana yang palsu
Keduanya dilatih secara bersamaan dalam permainan dua pemain (minimax game). GAN digunakan untuk image synthesis, style transfer, dan augmentasi data.

