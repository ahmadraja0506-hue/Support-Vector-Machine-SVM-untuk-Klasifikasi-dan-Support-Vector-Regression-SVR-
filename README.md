# Support-Vector-Machine-SVM-untuk-Klasifikasi-dan-Support-Vector-Regression-SVR
# Deskripsi Proyek  

Repository ini berisi implementasi algoritma Machine Learning menggunakan metode Support Vector Machine (SVM) dan Support Vector Regression (SVR) dengan bahasa pemrograman Python dan library Scikit-learn. 
Proyek ini bertujuan untuk memahami penerapan Support Vector Machine dalam dua jenis permasalahan Machine Learning, yaitu klasifikasi dan regresi. Kedua algoritma diterapkan menggunakan dataset yang berbeda sesuai dengan tujuan analisis masing-masing.

# 1. Support Vector Machine (SVM)
## Deskripsi

Support Vector Machine (SVM) merupakan algoritma Supervised Learning yang digunakan untuk melakukan klasifikasi dengan mencari hyperplane terbaik yang dapat memisahkan data ke dalam beberapa kelas.
Pada proyek ini, SVM digunakan untuk melakukan klasifikasi penyakit diabetes berdasarkan sejumlah atribut kesehatan yang terdapat pada dataset diabetes.csv.

## Dataset

Dataset yang digunakan memiliki 768 data dengan 9 kolom, yang terdiri dari 8 atribut dan 1 kolom target.
Beberapa atribut yang digunakan:

Pregnancies
Glucose
BloodPressure
SkinThickness
Insulin
BMI
DiabetesPedigreeFunction
Age
Kolom Outcome digunakan sebagai label klasifikasi

## Tahapan Proses

1. Import Dataset: Membaca dataset menggunakan Pandas dan mengubahnya menjadi DataFrame.
2. Eksplorasi Data: Menggunakan head() dan info() untuk melihat struktur serta informasi dataset.
3. Pemisahan Atribut dan Label: Memisahkan delapan atribut sebagai variabel X dan kolom Outcome sebagai variabel y.
4. Standardisasi Data: Menggunakan StandardScaler untuk menyamakan skala nilai setiap atribut.
5. Pembagian Dataset: Menggunakan train_test_split dengan 33% data testing dan 67% data training.
6. Pembuatan Model: Menggunakan SVC dari Scikit-learn untuk membangun model klasifikasi.
7. Pelatihan Model: Melatih model menggunakan data training dengan fungsi fit().
8. Evaluasi Model: Menggunakan fungsi score() untuk mengetahui akurasi model terhadap data testing.

## Hasil

Berdasarkan hasil pengujian, model SVM memperoleh akurasi sebesar 75,59% pada data testing.

# Support Vector Regression (SVR) 
## Deskripsi 

Support Vector Regression (SVR) merupakan pengembangan dari Support Vector Machine yang digunakan untuk menyelesaikan permasalahan regresi atau memprediksi nilai numerik.
Pada proyek ini, SVR digunakan untuk memprediksi gaji berdasarkan jumlah tahun pengalaman kerja menggunakan dataset Salary_Data.csv.

## Dataset

Dataset yang digunakan adalah Salary_Data.csv dengan jumlah 30 data dan terdiri dari dua atribut:
1. YearsExperience: Jumlah tahun pengalaman kerja.
2. Salary: Nilai gaji yang menjadi target prediksi.

## Tahapan Proses

1. Import Dataset: Membaca dataset menggunakan Pandas.

2. Eksplorasi Data: Menggunakan fungsi info() untuk mengetahui struktur dan tipe data.

3. Pemisahan Atribut dan Target: Memisahkan YearsExperience sebagai variabel X dan Salary sebagai variabel y.

4. Transformasi Data: Menggunakan NumPy untuk mengubah bentuk data X menjadi array dua dimensi.

5. Pembuatan Model: Menggunakan SVR dari Scikit-learn dengan konfigurasi parameter:

C = 1000
Gamma = 0.05
Kernel = RBF

6. Pelatihan Model: Melatih model menggunakan seluruh data yang tersedia dengan fungsi fit().

7. Visualisasi: Menggunakan Matplotlib untuk menampilkan persebaran data aktual melalui Scatter Plot serta garis prediksi model SVR.

## Hasil

Model SVR menghasilkan visualisasi hubungan antara pengalaman kerja dan gaji. Scatter Plot menunjukkan data aktual, sedangkan garis prediksi menggambarkan hasil estimasi model berdasarkan kernel RBF.
Notebook ini belum melakukan evaluasi menggunakan metrik seperti MAE, MSE, RMSE, atau R².

