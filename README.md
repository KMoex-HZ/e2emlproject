# 🧠 Prediksi Performa Siswa (Proyek End-to-End Machine Learning)

Proyek ini bertujuan untuk membangun sebuah pipeline machine learning end-to-end yang lengkap, mulai dari penyiapan data, pelatihan model, hingga deployment sebagai sebuah aplikasi web interaktif. Proyek ini didasarkan pada repository [mlproject oleh Krish Naik](https://github.com/krishnaik06/mlproject) sebagai latihan implementasi konsep MLOps.

---

### 🎯 Pernyataan Masalah

Bagaimana cara memprediksi skor ujian siswa secara akurat berdasarkan faktor-faktor demografis, sosial, dan kebiasaan belajar mereka? Proyek ini mencoba menjawab pertanyaan tersebut dengan membangun model regresi yang kuat dan mudah diakses melalui antarmuka web.

---

### ✨ Fitur Utama

- [cite_start]**Pipeline Prediksi Lengkap:** Proyek ini memiliki pipeline yang mencakup semua tahapan, mulai dari penyiapan data mentah hingga memberikan hasil prediksi. [cite: 2, 8]
- [cite_start]**Aplikasi Web Interaktif:** Dibangun dengan Flask, pengguna dapat memasukkan data siswa melalui formulir web dan langsung mendapatkan prediksi skor. [cite: 8, 10]
- [cite_start]**Struktur Kode Modular:** Kode diorganisir dalam direktori `src`, [cite: 6] memungkinkan reusabilitas dan skalabilitas yang lebih baik. [cite_start]Proyek ini juga dapat diinstal sebagai *package* Python berkat adanya file `setup.py`. [cite: 12]
- [cite_start]**Siap untuk Deployment:** Proyek ini sudah dikonfigurasi untuk proses deployment ke platform cloud seperti **AWS Elastic Beanstalk** [cite: 1] [cite_start]dan **Microsoft Azure**. [cite: 2]

---

### 🛠️ Tumpukan Teknologi (Tech Stack)

- **Bahasa:** Python
- **Analisis & Pemodelan:** Pandas, NumPy, Scikit-learn, CatBoost
- **Framework Web:** Flask
- **Deployment:** Docker, AWS Elastic Beanstalk, Azure, Gunicorn

[cite_start]*Untuk daftar lengkap dependensi, silakan lihat file `requirements.txt`.* [cite: 11]

---

### 🚀 Instalasi & Cara Menjalankan Secara Lokal

Untuk menjalankan proyek ini di komputermu, ikuti langkah-langkah berikut:

**Langkah 1: Clone Repository**
```bash
git clone [https://github.com/KMoex-HZ/e2emlproject.git](https://github.com/KMoex-HZ/e2emlproject.git)
cd e2emlproject
```

**Langkah 2: Buat Virtual Environment (Opsional tapi Direkomendasikan)**
```bash
python -m venv venv
source venv/bin/activate  # Untuk Windows: venv\Scripts\activate
```

**Langkah 3: Instal Dependensi**
```bash
pip install -r requirements.txt
```

**Langkah 4: Jalankan Aplikasi Web**
```bash
python app.py
```

**Langkah 5: Buka di Browser**
Buka browser dan akses alamat `http://127.0.0.1:5000` untuk melihat aplikasi berjalan.

---

### 📂 Struktur Proyek

```
[cite_start]├── .ebextensions/       # Konfigurasi deployment untuk AWS Elastic Beanstalk [cite: 1]
[cite_start]├── .github/workflows/   # Konfigurasi CI/CD untuk deployment ke Azure [cite: 2]
[cite_start]├── notebook/            # Berisi Jupyter Notebook untuk analisis data eksplorasi (EDA) [cite: 5]
[cite_start]├── src/                 # Berisi semua source code modular (komponen, pipeline, logger, dll.) [cite: 6]
[cite_start]├── templates/           # Berisi file HTML untuk antarmuka aplikasi web [cite: 7]
[cite_start]├── app.py               # File utama aplikasi Flask [cite: 10]
[cite_start]├── requirements.txt     # Daftar semua dependensi Python [cite: 11]
[cite_start]└── setup.py             # Script untuk membuat proyek ini sebagai package Python [cite: 12]
```
