# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding
Jaya Jaya Institut merupakan salah satu institusi pendidikan perguruan yang telah berdiri sejak tahun 2000. Hingga saat ini ia telah mencetak banyak lulusan dengan reputasi yang sangat baik. Akan tetapi, terdapat banyak juga siswa yang tidak menyelesaikan pendidikannya alias dropout.

Jumlah dropout yang tinggi ini tentunya menjadi salah satu masalah yang besar untuk sebuah institusi pendidikan. Oleh karena itu, Jaya Jaya Institut ingin mendeteksi secepat mungkin siswa yang mungkin akan melakukan dropout sehingga dapat diberi bimbingan khusus.

---

### Permasalahan Bisnis
- Mengidentifikasi faktor-faktor utama penyebab tingginya nilai dropout yang terjadi.
- Mengembangkan model machine learning untuk memprediksi kemungkinan siswa melakukan dropout
- Memberikan insight berbasis data untuk membantu manajemen menggambil keputusan
- Membuat business dashboard interaktif untuk memonitor siswa secara real-time, sehingga dapat mendukung pengambilan keputusan berbasis data.

---

### Cakupan Proyek
1. **Data Understanding & Statistic Analysis**
   - Memahami data secara keseluruhan, mencari anomaly, dan melihat pola yang terjadi pada data
2. **Exploratory Data Analysis (EDA)**  
   - Visualisasi dan analisis statistik untuk menemukan pola dan insight.
3. **Data Preprocessing & Feature Engineering**  
   - Membersihkan data, menangani missing values, dan encoding fitur kategorikal.  
4. **Model Machine Learning**  
   - Membangun model klasifikasi untuk memprediksi kemungkinan siswa dropout menggunakan base tree model.  
5. **Evaluasi Model**  
   - Menggunakan metrik evaluasi seperti Confusion Matrix, Classification Report, dan ROC-AUC.
6. **Membangun Prototype Machine Learning**
   - Membangun aplikasi prototype berbasis machine learning  
6. **Dashboard Interaktif**  
   - Membuat aplikasi interaktif berbasis **Looker Studio** untuk memudahkan manajamen mengambil keputusan.  

---

### Persiapan

Sumber data: (https://github.com/dicodingacademy/dicoding_dataset/blob/main/students_performance/data.csv)

### Setup environment:

Pastikan Anda mengikuti langkah-langkah berikut agar proyek dapat dijalankan dengan baik:

#### 1. Clone Repository

```bash
git clone https://github.com/Nauviii/Student-Dropout-Prediction-System.git
cd Student-Dropout-Prediction-System
```

#### 2. Membuat dan Mengaktifkan Virtual Environment

Agar lingkungan pengembangan terisolasi dan stabil, buat virtual environment (venv):

* **Windows**:

```bash
python -m venv venv
venv\Scripts\activate
```

* **macOS/Linux**:

```bash
python3 -m venv venv
source venv/bin/activate
```

#### 3. Install Dependencies

```bash
pip install -r requirements.txt
```
---
## Business Dashboard

🔗 Akses Dashboard: (https://lookerstudio.google.com/reporting/2ad7f54a-989f-47e3-bb37-bbeeb1d44a43) 

### 🎓 Students Performance Dashboard

### Komponen Utama yang Tampil
- **KPI (Key Performance Indicators):**
  - **Record Count:** 4.424 → jumlah mahasiswa.
  - **Application Order:** 7.6K → total pendaftaran.
- **Distribusi Status Mahasiswa:**
  - Graduate (49.9%), Dropout (32.1%), Enrolled (17.9%).
- **Faktor yang Mempengaruhi:**
  - Usia pendaftaran.
  - Beasiswa.
  - Status keuangan (debtor & tuition fees).
  - Kondisi khusus (displaced).

### Fungsi Dashboard
- **Monitoring**: memantau tren dropout, kelulusan, dan enrollment secara cepat.  
- **Diagnosis**: menemukan faktor penyebab dropout (misalnya keuangan, tidak ada beasiswa, atau usia masuk lebih tua).  
- **Decision Support**: membantu pihak kampus mengambil keputusan seperti:
  - Apakah perlu memperbanyak program beasiswa?
  - Apakah perlu intervensi finansial bagi debtor?
  - Bagaimana strategi dukungan mahasiswa usia >23 tahun?

---

## Menjalankan Sistem Machine Learning

Reviewer dapat menjalankan prototype sistem machine learning ini dengan langkah-langkah berikut:  

### 🔹 1. Setup Environment
1. Clone repository:
   ```bash
   git clone https://github.com/Nauviii/Student-Dropout-Prediction-System.git
   cd Student-Dropout-Prediction-System
   ```
2. Membuat dan Mengaktifkan Virtual Environment

* **Windows**:

```bash
python -m venv venv
venv\Scripts\activate
```

* **macOS/Linux**:

```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install Dependencies

```bash
pip install -r requirements.txt
```

4. Menjalankan prototype machine learning
```bash
streamlit run main.py
```

---

## Conclusion
Proyek ini berhasil mengimplementasikan sistem machine learning untuk memprediksi kemungkinan mahasiswa melakukan *dropout* di Jaya Jaya Institut.  
Melalui tahapan **data understanding, exploratory data analysis, preprocessing, model building, evaluasi, deployment, serta visualisasi di Looker Studio**, sistem ini mampu memberikan solusi yang dapat langsung dimanfaatkan oleh pihak institusi.

Beberapa poin penting yang dapat disimpulkan:
1. **Model Machine Learning (XGBoost)** memberikan performa yang baik dalam mengklasifikasikan status mahasiswa dengan menggunakan 14 fitur utama.  
2. **Faktor-faktor penting** yang mempengaruhi prediksi dropout di antaranya adalah nilai akademik, status keuangan (pembayaran biaya kuliah), serta faktor beasiswa.  
3. **Dashboard interaktif berbasis Looker Studio** mempermudah stakeholder untuk:
   - Mengeksplorasi data performa mahasiswa secara visual,  
   - Mengidentifikasi tren dropout, graduate, dan enrollment,  
   - Menemukan faktor risiko utama secara cepat,  
   - Mendukung pengambilan keputusan berbasis data.  
4. Sistem ini dapat menjadi **alat bantu strategis** bagi manajemen dalam melakukan *early intervention* terhadap mahasiswa yang berpotensi dropout.  

---

## Future Work
Untuk pengembangan ke depan, sistem ini masih dapat ditingkatkan, antara lain:
- Menambahkan lebih banyak data historis untuk meningkatkan akurasi model,  
- Mengintegrasikan data real-time dari sistem informasi akademik,  
- Mengembangkan sistem rekomendasi yang lebih personalisasi untuk mahasiswa berisiko tinggi,  
- Mengimplementasikan MLOps agar model dapat terus diperbarui secara otomatis dengan data terbaru.  

Dengan adanya sistem ini, diharapkan tingkat dropout mahasiswa di Jaya Jaya Institut dapat ditekan, serta memberikan pengalaman belajar yang lebih baik bagi mahasiswa.

---

### Rekomendasi Action Items

#### 1. Jika Mahasiswa Terindikasi Akan Melakukan Dropout, Maka Direkomendasikan untuk:

- **Berikan bimbingan akademik intensif**  
  Mahasiswa yang memiliki performa akademik rendah perlu mendapatkan sesi bimbingan tambahan, baik berupa tutoring, kelas remedial, atau mentoring dari dosen agar kesulitan belajar dapat segera diatasi.

- **Monitor progress secara berkala**  
  Pihak kampus perlu melakukan monitoring akademik dengan jadwal rutin (misalnya setiap akhir semester) untuk memastikan adanya perbaikan dari mahasiswa yang berisiko dropout.

- **Pertimbangkan program remedial**  
  Jika mahasiswa gagal pada beberapa mata kuliah, program remedial dapat membantu mereka memperbaiki nilai tanpa harus menunda kelulusan terlalu lama.

- **Konseling untuk mengatasi masalah personal/finansial**  
  Banyak kasus dropout tidak hanya disebabkan faktor akademik, tetapi juga permasalahan pribadi dan finansial. Konseling psikologis dan bantuan finansial (misalnya potongan biaya atau beasiswa darurat) bisa menjadi solusi efektif.

- **Libatkan academic advisor dan orang tua**  
  Advisor (dosen wali) bersama orang tua dapat dilibatkan dalam diskusi tindak lanjut sehingga mahasiswa merasa didukung baik dari sisi akademik maupun lingkungan keluarga.

#### 2. Jika Mahasiswa Tidak Terindikasi Akan Melakukan Dropout, Maka Direkomendasikan untuk:

- **Pertahankan kualitas akademik yang baik**  
  Mahasiswa tetap perlu diarahkan agar menjaga konsistensi performa akademiknya melalui kebiasaan belajar yang teratur dan disiplin.

- **Dorong partisipasi dalam kegiatan kampus**  
  Mahasiswa dapat diperkuat motivasinya dengan dilibatkan dalam kegiatan organisasi, penelitian, maupun lomba, sehingga mereka lebih terikat secara emosional dengan kampus.

- **Berikan apresiasi dan penghargaan**  
  Pemberian penghargaan (misalnya sertifikat, beasiswa prestasi, atau publikasi pencapaian) dapat meningkatkan motivasi dan menjadi teladan bagi mahasiswa lain.

- **Kembangkan soft skills dan keterampilan tambahan**  
  Walaupun tidak berisiko dropout, mahasiswa perlu difasilitasi untuk meningkatkan keterampilan non-akademik seperti kepemimpinan, komunikasi, dan pemecahan masalah, yang akan bermanfaat di dunia kerja.

- **Siapkan jalur percepatan akademik**  
  Bagi mahasiswa berprestasi, dapat diberikan opsi percepatan kelulusan, kesempatan mengambil mata kuliah lintas jurusan, atau program magang industri untuk memperkuat kompetensi mereka.

---

