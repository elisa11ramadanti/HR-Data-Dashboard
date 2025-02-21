# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

HR-Data-Dashboard

Nama: Elisa Ramadanti

---

## Business Understanding

Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000. Ia memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri. Walaupun telah menjadi menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%.

Untuk mencegah hal ini semakin parah, manajer departemen HR ingin meminta bantuan Anda mengidentifikasi berbagai faktor yang mempengaruhi tingginya attrition rate tersebut. Selain itu, ia juga meminta Anda untuk membuat business dashboard untuk membantunya memonitori berbagai faktor tersebut.

### Permasalahan Bisnis

1. Tingginya Tingkat Pengunduran Diri Karyawan
    - Pengunduran Diri Karyawan di Jaya Jaya Maju melebihi 15%, menyebabkan perusahaan kehilangan lebih dari 100 karyawan setiap tahun.
    - Mengakibatkan biaya tinggi terkait rekrutmen, pelatihan ulang, dan hilangnya produktivitas yang jika tidak ditangani, dapat mengakibatkan hilangnya talenta berbakat, penurunan moral karyawan, dan reputasi perusahaan yang buruk.

2. Tantangan dalam Pengelolaan Karyawan
    - Manajer HR membutuhkan alat untuk memantau faktor-faktor yang mempengaruhi attrition.
    - Diperlukan business dashboard untuk memberikan wawasan real-time tentang tingkat attrition dan faktor-faktor penyebabnya.

---

### Cakupan Proyek

1. Data Understanding:

      Melakukan eksplorasi awal terhadap dataset karyawan untuk memahami struktur data, tipe data, distribusi nilai, dan pola-pola yang ada. Langkah ini mencakup:
    - Analisis statistik deskriptif.
    - Visualisasi data seperti distribusi usia, hubungan antara pendapatan bulanan dan usia, serta tingkat pendidikan.
    - Identifikasi missing value dan data duplikat.
2. Data Preparation :
  
    Menyiapkan dataset agar siap digunakan untuk pemodelan. Langkah ini meliputi:
    -  Penanganan missing value.
    -  Encoding data kategorikal menggunakan LabelEncoder.
    -  Feature engineering untuk membuat fitur baru seperti TotalSatisfaction, AvgYearsPerCompany, dan PromotionFrequency.
    -  Normalisasi data numerik menggunakan MinMaxScaler.

3. Identifikasi Faktor-Faktor yang Mempengaruhi Perputaran Karyawan :

    - Mengidentifikasi pola dan hubungan antara variabel-variabel seperti kepuasan kerja, jarak tempat tinggal, lamanya bekerja di perusahaan, dan faktor lainnya yang memengaruhi pengunduran diri karyawan.
4. Rekomendasi Langkah-Langkah Konkrit untuk Menurunkan Attrition 
5. Membangun Model Machine Learning untuk Memprediksi Kemungkinan Karyawan akan Keluar :
    - Mengembangkan model prediktif menggunakan SVM dan Logistic Regression untuk memprediksi kemungkinan seorang karyawan mengundurkan diri.

---


### Persiapan

1. **Sumber Data:**  [Employee Data](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee)

2. Setup environment:
    - Instal semua library yang dibutuhkan:
        ```bash
          pip install -r requirements.txt
        ```
    - Load Dataset yang digunakan:
        ```
          df = pd.read_csv("/Dataset/employee_data.csv")
        ```
    - Menjalankan Dashboard Metabase:
       ```
          docker -compose up
       ```
## Business Dashboard

Dashboard bisnis dirancang untuk memberikan wawasan visual terkait faktor-faktor yang memengaruhi pengunduran diri karyawan. Visualisasi mencakup informasi berikut:


1. Total Departemen dalam perusahaan.
2. Jumlah Total Karyawan di perusahaan.
3. Rata-rata Tingkat Pengunduran Diri (Attrition Rate) .
4. Rata-rata Jarak Tempuh dari tempat tinggal karyawan ke kantor.
5. Rata-rata Pendapatan Bulanan karyawan perusahaan.
6. Distribusi Karyawan Berdasarkan Gender .
7. Tingkat Pendidikan karyawan perusahaan.
8. Grafik Pengunduran Diri Berdasarkan Jarak.
9. Grafik Pengunduran Diri Berdasarkan Posisi Kerja

Link Dashboard: [HR Data Dashboard](http://localhost:3000/public/dashboard/d7ece5af-b653-46e4-ae6c-2b05743dbe7a)

---


## Conclusion

1. Model Machine Learning :
    - Model Logistic Regression berhasil memprediksi kemungkinan pengunduran diri karyawan dengan akurasi sebesar 88% . Model ini dapat digunakan oleh perusahaan untuk mengidentifikasi karyawan yang memiliki risiko tinggi mengundurkan diri, sehingga langkah pencegahan seperti intervensi atau penyesuaian kebijakan dapat dilakukan secara proaktif.
2. Insight dari Dashboard :

  Berdasarkan visualisasi pada dashboard bisnis, diperoleh beberapa temuan penting:
  - Perusahaan memiliki 3 departemen utama .
   - Jumlah karyawan laki-laki lebih banyak dibandingkan karyawan perempuan.
   - Beberapa posisi kerja tertentu menunjukkan tren yang lebih tinggi dalam hal pengunduran diri karyawan. Hal ini dapat menjadi indikator bahwa faktor pekerjaan atau lingkungan kerja di posisi tersebut perlu dievaluasi lebih lanjut.
  - Karyawan yang tinggal dekat dengan perusahaan (jarak 0-5 km) ternyata tidak selalu bertahan lebih lama. Faktanya, kelompok ini memiliki tingkat pengunduran diri yang cukup tinggi.

---

### Rekomendasi Action Items

1. Berikan pelatihan dan program pengembangan yang sesuai dengan kebutuhan karyawan guna meningkatkan keterlibatan, motivasi, serta keterampilan mereka dalam bekerja.
2. Meningkatkan Rasa Kebersamaan melalui Acara Sosial

---

### Login Metabase
- `Email` : elisaramadanti11@gmail.com
- `password` : Tahuwalik12_ 
