# Learn_Pytorch_using_iris_dataset

Learn PyTorch – Simple Neural Network (Iris Dataset)

Repository ini berisi contoh project Machine Learning sederhana menggunakan PyTorch
untuk klasifikasi Iris Dataset.
Project ini dibuat sebagai latihan dasar untuk memahami alur training Neural Network
di PyTorch dari nol.

📂 Struktur Folder
.
├── Learn-Pytorch-Simple_NN.py   # Script utama training & evaluasi model
├── IRIS.csv                    # Dataset Iris
├── requirements.txt            # Dependency Python
└── README.md                   # Dokumentasi project

🧠 Apa yang Dibuat di Project Ini?
1. Neural Network Model

Model dibuat menggunakan torch.nn.Module dengan arsitektur:

Input layer: 4 fitur

Hidden layer 1: 8 neuron

Hidden layer 2: 9 neuron

Output layer: 3 kelas (Iris Setosa, Versicolor, Virginica)

Activation Function:

ReLU

2. Dataset & Preprocessing

Dataset dibaca menggunakan pandas

Label species diubah dari string ke integer menggunakan LabelEncoder

Data dikonversi ke PyTorch Tensor

Dataset dibagi menjadi:

80% training

20% testing

3. Training Model

Konfigurasi training:

Loss Function: CrossEntropyLoss

Optimizer: Adam

Learning Rate: 0.01

Epochs: 100

Alur training:

Model melakukan forward pass

Loss dihitung

Gradien di-reset

Backpropagation dijalankan

Bobot (weight) diperbarui

Nilai loss disimpan setiap epoch

4. Visualisasi Loss

Loss selama training divisualisasikan menggunakan Matplotlib.

Grafik menunjukkan:

Sumbu X: Epoch

Sumbu Y: Loss / Error

Grafik ini digunakan untuk melihat apakah model benar-benar belajar
(loss menurun seiring waktu).

5. Evaluasi Model

Evaluasi dilakukan menggunakan torch.no_grad() yang berarti:

Model tidak belajar

Gradien tidak dihitung

Lebih hemat memori

Cocok untuk testing / inference

Pada tahap ini:

Model diuji menggunakan data test

Loss evaluasi dihitung

Prediksi dibandingkan dengan label asli

Jumlah prediksi benar dihitung

⚙️ Cara Menjalankan Project

Install dependency:

pip install -r requirements.txt


Jalankan script:

python Learn-Pytorch-Simple_NN.py


Jika GPU tersedia, model akan otomatis menggunakan CUDA.

🎯 Tujuan Project

Project ini dibuat untuk:

Belajar dasar PyTorch

Memahami konsep epoch, loss, optimizer, dan weight

Latihan klasifikasi sederhana

Menjadi fondasi sebelum lanjut ke model yang lebih kompleks

📝 Catatan

Project ini difokuskan untuk pemahaman konsep, bukan optimasi maksimal.
Kode ditulis sederhana agar mudah dipelajari oleh pemula.
