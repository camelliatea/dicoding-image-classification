# Image Classification Project
Proyek ini adalah implementasi model klasifikasi gambar menggunakan Tensorflow. Model yang dikembangkan dirancang untuk mengenali tiga kelas dalam dataset Parasite, yaitu RBCs, Toxoplasma, dan Trichomonad. Proyek dikembangkan sebagai bagian dari tugas akhir kelas 'Belajar Pengembangan Machine Learning', dengan fokus pada penerapan teknik deep learning untuk membantu analisis data gambar secara otomatis mulai dari tahapan data preprocessing, pelatihan model, evaluasi kinerja, hingga penerapan model untuk prediksi data baru.

---

## Dataset
Dataset yang digunakan dalam proyek ini adalah "🔬Parasite Dataset: Leishmania, Plasmodium & Babesia", yang disediakan oleh Ahmed Alrefaei melalui platform Kaggle. 
Dataset ini terdiri dari 34.298 gambar mikroskopis yang mencakup berbagai jenis parasit dan sel inang (host cells) di bawah perbesaran 400X atau 1000X. Namun, karena distribusi kelas yang tidak merata, proyek ini hanya menggunakan subset dataset yang mencakup tiga kelas utama:
- RBCs,
- Toxoplasma,
- Trichomonad.
Untuk memastikan kualitas pelatihan model, ketiga subset terpilih merupakan subset dengan lebih dari 5.000 sampel data untuk masing-masing kelas.

Original Dataset:
Li, Sen; Zhang, Yang (2020), "Microscopic Images of Parasites Species", Mendeley Data, V3, doi: 10.17632/38jtn4nzs6.3
Dataset asli tersebut telah dikurasi ulang oleh Ahmed Alrefaei, yang membagikan versi baru melalui platform Kaggle: [Parasite Dataset - Kaggle](https://www.kaggle.com/datasets/ahmedxc4/parasite-dataset)
Dataset ini dilisensikan di bawah Creative Commons Attribution 4.0 International (CC BY 4.0), yang memungkinkan pengguna untuk menggunakan, mendistribusikan, dan memodifikasi dataset selama atribusi diberikan kepada pembuatnya.

Kredit penuh diberikan kepada Sen Li dan Yang Zhang, serta Ahmed Alrefaei.

---

## Cara Menjalankan Proyek
1. Instal Dependensi
    `pip install -r requirements.txt`
2. Jalankan Notebook *Submission_Akhir.ipynb*
    Upload file ke Google Colab atau buka melalui VS Code.

---

## Struktur Folder
dicoding-image-classification/

├── saved_model
│   ├── assets
│   ├── variables
│   ├── fingerprint.pb
│   └── saved_model.pb
├── tfjs_model
│   ├── group1-shard1of2.bin
│   ├── group1-shard2of2.bin
│   └── model.json
├── tflite
│   ├── label.txt 
│   └── model.tflite
├── notebook.ipynb
├── README.md
└── requirements.txt

