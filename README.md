# Analisis Regresi Kinerja Siswa (Student Performance Regression)

Proyek ini berisi implementasi dan analisis pemodelan regresi menggunakan Python untuk memprediksi nilai akhir siswa berdasarkan beberapa fitur akademik.

## 📋 Fitur Dataset (`DM_Week6_Student_Regression.csv`)
Dataset terdiri dari 179 baris dan 6 kolom tanpa nilai kosong[cite: 4]:
1. **`jam_belajar`**: Jumlah jam belajar siswa[cite: 4].
2. **`kehadiran`**: Persentase kehadiran siswa di kelas[cite: 4].
3. **`nilai_tugas`**: Rata-rata nilai tugas siswa[cite: 4].
4. **`nilai_kuis`**: Rata-rata nilai kuis siswa[cite: 4].
5. **`aktivitas_forum`**: Tingkat keaktifan siswa dalam forum diskusi[cite: 4].
6. **`nilai_akhir`** *(Target)*: Nilai akhir yang diperoleh siswa[cite: 4].

---

## 🛠️ Pustaka yang Digunakan
* **Pandas & NumPy**: Untuk pemuatan dan manipulasi data[cite: 4].
* **Matplotlib**: Untuk visualisasi data[cite: 4].
* **Scikit-Learn (`sklearn`)**: Untuk pemodelan machine learning, evaluasi metrik, dan *preprocessing*[cite: 4]:
  * `train_test_split` (Pembagian data latih dan data uji)[cite: 4]
  * `LinearRegression` & `KNeighborsRegressor` (Algoritma regresi)[cite: 4]
  * `StandardScaler` & `make_pipeline` (Standardisasi dan *pipeline* data)[cite: 4]
  * `mean_absolute_error`, `mean_squared_error`, `r2_score` (Metrik evaluasi)[cite: 4]

---

## ⚙️ Alur Kerja (Workflow)
1. **Pemuatan & Pemeriksaan Data**: Memuat dataset dari file CSV, memeriksa ukuran dataset, serta memastikan tidak ada nilai kosong (*missing values*)[cite: 4].
2. **Pembagian Data (*Splitting*)**: Memisahkan fitur dan variabel target (`nilai_akhir`), lalu membagi data menjadi data latih (80%) dan data uji (20%)[cite: 4].
3. **Regresi Linear Sederhana**: Membangun model regresi linear menggunakan satu fitur utama, yaitu tingkat kehadiran (`kehadiran`), untuk mendapatkan parameter intersep ($\beta_0$) dan slope ($\beta_1$)[cite: 4].

---

## 🚀 Cara Menjalankan
Pastikan pustaka yang dibutuhkan telah terpasang, lalu jalankan sel-sel kode di dalam Jupyter Notebook atau lingkungan Python Anda secara berurutan.
