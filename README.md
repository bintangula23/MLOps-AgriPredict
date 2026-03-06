# MLOps-AgriPredict

## Deskripsi Proyek

**AgriPredict** merupakan proyek pembelajaran MLOps yang bertujuan untuk membangun sistem prediksi harga cabai di Indonesia menggunakan data dari Pusat Informasi Harga Pangan Strategis (PIHPS) milik Bank Indonesia.

Proyek ini dirancang untuk menerapkan praktik dasar MLOps mulai dari pengambilan data, preprocessing data, eksplorasi data, pelatihan model machine learning, hingga pengelolaan kode secara terstruktur menggunakan GitHub.

Komoditas yang menjadi fokus analisis pada proyek ini adalah cabai merah besar dan cabai rawit merah. Data harga diambil secara berkala dari PIHPS dan digunakan untuk membangun model prediksi berbasis data historis harga.

Melalui proyek ini diharapkan dapat dihasilkan sistem prediksi sederhana yang dapat membantu memahami pola fluktuasi harga cabai.

---

## Tujuan Proyek

Tujuan dari proyek AgriPredict adalah:

* Mengambil data harga cabai dari PIHPS secara otomatis
* Melakukan proses preprocessing dan pembersihan data
* Melakukan eksplorasi data untuk memahami pola harga
* Melatih model machine learning untuk memprediksi harga cabai
* Menerapkan praktik dasar MLOps seperti version control, reproducibility, dan struktur proyek yang terstandar

---

## Struktur Direktori Proyek

Struktur proyek mengikuti konvensi **Cookiecutter Data Science** agar kode mudah dipahami, terorganisir, dan mudah dikembangkan di masa depan.

```
MLOps-AgriPredict
│
├── data
│   ├── raw
│   │   └── data mentah yang diambil dari sumber eksternal
│   │
│   └── processed
│       └── data yang telah melalui proses pembersihan dan transformasi
│
├── models
│   └── penyimpanan model machine learning yang telah dilatih
│
├── notebooks
│   └── notebook eksplorasi data dan eksperimen model
│
├── src
│   ├── data
│   │   └── script pengambilan dan pemrosesan data
│   │
│   ├── features
│   │   └── script untuk feature engineering
│   │
│   └── models
│       └── script training dan evaluasi model
│
├── config
│   └── file konfigurasi proyek
│
├── requirements.txt
│   └── daftar dependency Python
│
└── README.md
    └── dokumentasi proyek
```

Struktur ini memisahkan data, kode, dan eksperimen sehingga pengembangan proyek menjadi lebih terorganisir.

---

## Teknologi yang Digunakan

Beberapa teknologi utama yang digunakan dalam proyek ini antara lain:

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Requests
* Jupyter Notebook
* Git & GitHub
* GitHub Codespaces

Teknologi tersebut digunakan untuk mendukung proses pengambilan data, analisis data, pelatihan model, dan pengelolaan kode proyek.

---

## Setup Lingkungan Pengembangan

Proyek ini menggunakan **GitHub Codespaces** untuk memastikan lingkungan pengembangan dapat dijalankan secara konsisten di berbagai perangkat.

Langkah menjalankan proyek menggunakan Codespaces:

1. Buka repositori ini melalui GitHub.
2. Klik tombol **Code** pada halaman repositori.
3. Pilih **Open with Codespaces**.
4. Tunggu hingga lingkungan Codespaces selesai dibuat.
5. Install dependency Python dengan perintah berikut pada terminal:

```
pip install -r requirements.txt
```

Setelah instalasi selesai, proyek siap digunakan untuk eksplorasi data maupun pengembangan model.

---

## Branching Strategy

Proyek ini menggunakan **GitHub Flow** sebagai strategi pengelolaan kode.

Alur pengembangan dilakukan sebagai berikut:

1. Branch **main** digunakan sebagai branch utama yang berisi kode stabil.
2. Pengembangan fitur atau eksperimen dilakukan pada branch terpisah.
3. Contoh branch eksperimen:

```
feat/initial-eda
```

4. Setelah eksperimen selesai dan telah divalidasi, perubahan akan diajukan melalui **Pull Request** untuk digabungkan ke branch **main**.

Pendekatan ini membantu menjaga stabilitas kode serta memudahkan pelacakan perubahan dalam proyek.

---

## Sumber Data

Data harga pangan diperoleh dari:

Pusat Informasi Harga Pangan Strategis (PIHPS)
Bank Indonesia

Website resmi:
https://www.bi.go.id/hargapangan

Data tersebut menyediakan informasi harga komoditas pangan di berbagai wilayah Indonesia yang dapat digunakan untuk analisis dan pemodelan prediksi harga.

---

## Catatan

Proyek ini dikembangkan sebagai bagian dari pembelajaran **Machine Learning Operations (MLOps)** dengan fokus pada penerapan praktik pengelolaan proyek machine learning yang terstruktur dan reproducible menggunakan GitHub dan GitHub Codespaces.
