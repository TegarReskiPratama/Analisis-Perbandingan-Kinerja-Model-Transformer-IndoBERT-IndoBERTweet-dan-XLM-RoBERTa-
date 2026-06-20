# Analisis Perbandingan Kinerja Model Transformer IndoBERT, IndoBERTweet, dan XLM-RoBERTa dalam Deteksi Promosi Judi Online Berbahasa Indonesia

## Deskripsi

Repository ini berisi implementasi penelitian mengenai perbandingan kinerja tiga model Transformer, yaitu **IndoBERT**, **IndoBERTweet**, dan **XLM-RoBERTa**, dalam mendeteksi promosi judi online pada teks berbahasa Indonesia.

Penelitian dilakukan melalui tahapan preprocessing data, eksplorasi data, pelatihan model, evaluasi performa, serta analisis hasil menggunakan metrik Accuracy, Precision, Recall, dan F1-Score.

---

## Struktur Repository

```text
├── data/
│   ├── raw/
│   │   └── dataset_mentah.csv
│   │
│   └── processed/
│       └── dataset_hasil_preprocessing.csv
│
├── notebooks/
│   └── Analisis_Perbandingan_Kinerja_Model_Transformer_IndoBERT,_IndoBERTweet,_dan_XLM_RoBERTa_dalam_Deteksi_Promosi_Judi_Online_Berbahasa_Indonesia.ipynb
│
├── requirements.txt
└── README.md
```

---

## Dataset

Penelitian menggunakan dataset teks berbahasa Indonesia yang berisi:

* Promosi Judi Online (Label = 1)
* Non Judi Online (Label = 0)

Dataset kemudian digabungkan, dibersihkan, diseimbangkan (balancing), dan dibagi menjadi data latih serta data uji.

---

## Library yang Digunakan

* transformers
* datasets
* accelerate
* evaluate
* torch
* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn
* wordcloud
* sentencepiece

---

## Instalasi

### 1. Clone Repository

```bash
git clone https://github.com/username/repository-name.git
```

### 2. Masuk ke Folder Project

```bash
cd repository-name
```

### 3. Install Dependency

```bash
pip install -r requirements.txt
```

---

## Menjalankan Project

Buka Jupyter Notebook atau Google Colab.

```bash
jupyter notebook
```

Kemudian jalankan notebook berikut:

```text
notebooks/
└── Analisis_Perbandingan_Kinerja_Model_Transformer_IndoBERT,_IndoBERTweet,_dan_XLM_RoBERTa_dalam_Deteksi_Promosi_Judi_Online_Berbahasa_Indonesia.ipynb
```

Jalankan seluruh cell secara berurutan dari atas hingga bawah.

---

## Pipeline Penelitian

### 1. Data Preparation

* Membaca dataset
* Menggabungkan dataset
* Memilih kolom yang digunakan

### 2. Data Cleaning

* Menghapus data kosong
* Menghapus duplikasi
* Membersihkan URL
* Membersihkan mention
* Membersihkan simbol dan karakter khusus

### 3. Exploratory Data Analysis (EDA)

* WordCloud Promosi Judi Online
* WordCloud Non Judi Online
* Distribusi Label
* Visualisasi Dataset

### 4. Data Balancing

* Menyeimbangkan jumlah data pada setiap kelas

### 5. Train-Test Split

* Membagi dataset menjadi data latih dan data uji

### 6. Model Training

Model yang dibandingkan:

#### IndoBERT

Model BERT khusus Bahasa Indonesia.

#### IndoBERTweet

Model Transformer yang dilatih menggunakan data media sosial dan Twitter berbahasa Indonesia.

#### XLM-RoBERTa

Model multilingual yang mendukung berbagai bahasa termasuk Bahasa Indonesia.

### 7. Evaluasi Model

Metrik yang digunakan:

* Accuracy
* Precision
* Recall
* F1-Score

### 8. Visualisasi Hasil

* Confusion Matrix IndoBERT
* Confusion Matrix IndoBERTweet
* Confusion Matrix XLM-RoBERTa
* Grafik Perbandingan Performa
* Grafik F1-Score

### 9. Analisis Model Terbaik

Model terbaik ditentukan berdasarkan:

* Accuracy tertinggi
* Precision tertinggi
* Recall tertinggi
* F1-Score tertinggi

---

## Output Penelitian

Output yang dihasilkan:

* Tabel Perbandingan Model
* Confusion Matrix
* Grafik Evaluasi
* Ranking Model
* Analisis Model Terbaik

---

## Author

**Tegar Reski Pratama**

Program Studi Informatika

Universitas Muhammadiyah Malang

2026
