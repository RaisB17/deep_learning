Bab 18: Reinforcement Learning
File: 18_reinforcement_learning.ipynb
Tujuan
Membahas pendekatan pembelajaran berdasarkan interaksi agen dengan lingkungan melalui sistem reward dan punishment. Reinforcement Learning (RL) merupakan salah satu cabang AI yang paling mendekati cara belajar manusia dan hewan.
Isi
Pembelajaran penguatan digunakan ketika solusi tidak diketahui secara eksplisit, dan agen harus belajar sendiri dari pengalaman. RL digunakan dalam berbagai bidang seperti robotika, game (misalnya AlphaGo), pengendalian sistem, dan sistem rekomendasi adaptif.
Komponen utama RL:
•	Environment: dunia tempat agen beroperasi.
•	Agent: entitas yang mengambil keputusan.
•	State (s): representasi dari kondisi lingkungan saat ini.
•	Action (a): tindakan yang bisa diambil oleh agen.
•	Reward (r): umpan balik dari lingkungan berdasarkan tindakan agen.
•	Policy (π): strategi yang menentukan tindakan berdasarkan state.
•	Value function: estimasi total reward jangka panjang dari state tertentu.
Strategi pembelajaran dalam RL dibagi dua:
1.	Value-based methods: agen mempelajari nilai dari setiap state atau pasangan state-action.
o	Contoh: Q-Learning, yang belajar memaksimalkan expected reward melalui Q-Table.
o	SARSA (State-Action-Reward-State-Action): mirip Q-Learning tapi lebih konservatif karena update berdasarkan aksi yang benar-benar diambil.
2.	Policy-based methods: agen langsung mempelajari kebijakan (policy) tanpa eksplisit menghitung nilai.
o	Contoh: REINFORCE algorithm, Policy Gradient.
o	Cocok untuk ruang aksi kontinu dan masalah kompleks.
Penggabungan kedua pendekatan dikenal sebagai Actor-Critic, di mana actor mengarahkan aksi, dan critic mengevaluasi kualitas aksi tersebut.
Deep Reinforcement Learning memperluas konsep RL dengan menggunakan jaringan saraf dalam untuk mendekati fungsi nilai dan kebijakan.
•	Deep Q-Network (DQN): menggabungkan Q-Learning dengan CNN, digunakan misalnya dalam permainan Atari.
•	Teknik tambahan: Experience Replay (buffer data masa lalu), Target Network (mengurangi osilasi).
Untuk eksperimen praktis, framework TF-Agents dari TensorFlow menyediakan tools RL siap pakai untuk berbagai environment simulasi.
Tantangan dalam RL:
•	Sparse rewards (reward hanya didapat jarang)
•	Trade-off eksplorasi vs eksploitasi
•	Stabilitas pelatihan
•	Efisiensi sampel
RL merupakan bidang yang terus berkembang dengan aplikasi yang sangat luas dan membutuhkan kombinasi pemodelan cerdas dan pelatihan yang efisien.

