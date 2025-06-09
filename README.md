# 🧠 Prediksi Performa Siswa (Proyek End-to-End Machine Learning)

Proyek ini bertujuan untuk membangun sebuah pipeline machine learning end-to-end yang lengkap, mulai dari penyiapan data, pelatihan model, hingga deployment sebagai sebuah aplikasi web interaktif. Proyek ini didasarkan pada repository [mlproject oleh Krish Naik](https://github.com/krishnaik06/mlproject) sebagai latihan implementasi konsep MLOps.

---

### 🎯 Pernyataan Masalah

Bagaimana cara memprediksi skor ujian siswa secara akurat berdasarkan faktor-faktor demografis, sosial, dan kebiasaan belajar mereka? Proyek ini mencoba menjawab pertanyaan tersebut dengan membangun model regresi yang kuat dan mudah diakses melalui antarmuka web.

---

### ✨ Fitur Utama

- **Pipeline Prediksi Lengkap:** Proyek ini memiliki pipeline yang mencakup semua tahapan, mulai dari penyiapan data mentah hingga memberikan hasil prediksi. 
- **Aplikasi Web Interaktif:** Dibangun dengan Flask, pengguna dapat memasukkan data siswa melalui formulir web dan langsung mendapatkan prediksi skor. 
- **Struktur Kode Modular:** Kode diorganisir dalam direktori `src`, memungkinkan reusabilitas dan skalabilitas yang lebih baik. Proyek ini juga dapat diinstal sebagai *package* Python berkat adanya file `setup.py`. 
- **Siap untuk Deployment:** Proyek ini sudah dikonfigurasi untuk proses deployment ke platform cloud seperti **AWS Elastic Beanstalk** [cite: 1] dan **Microsoft Azure**. 

---

### 🛠️ Tumpukan Teknologi (Tech Stack)

- **Bahasa:** Python
- **Analisis & Pemodelan:** Pandas, NumPy, Scikit-learn, CatBoost
- **Framework Web:** Flask
- **Deployment:** Docker, AWS Elastic Beanstalk, Azure, Gunicorn

*Untuk daftar lengkap dependensi, silakan lihat file `requirements.txt`.* 

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
├── .ebextensions/       # Konfigurasi deployment untuk AWS Elastic Beanstalk 
├── .github/workflows/   # Konfigurasi CI/CD untuk deployment ke Azure 
├── notebook/            # Berisi Jupyter Notebook untuk analisis data eksplorasi (EDA) 
├── src/                 # Berisi semua source code modular (komponen, pipeline, logger, dll.) 
├── templates/           # Berisi file HTML untuk antarmuka aplikasi web 
├── app.py               # File utama aplikasi Flask 
├── requirements.txt     # Daftar semua dependensi Python 
└── setup.py             # Script untuk membuat proyek ini sebagai package Python 
```
