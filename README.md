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




