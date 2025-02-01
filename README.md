# Prediksi Harga Tiket Pesawat Regresi Linear, Decision Tree, Random Forest, dan Xg Boosting 

Perkembangan    di    bidang    pariwisata menjadi sebuah daya tarik bagi seorang traveller yang  ingin  berkunjung  dan  menikmati wisata  di seluruh dunia, dan dapat menjadi dampak positif di  sektor  penerbangan  dan  sektor  pariwisata. Dengan  adanya  peran  teknologi  sangat  banyak mempengaruhi segala bidang, dan salah satunya pada   penjualan   tiket   pesawat. Hal   tersebut menjadi  keuntungan bagi  penyedia  jasa  layanan perjalanan     dalam     memperjual belikan     tiket pesawat   dengan   tarif   yang   murah.   Dengan banyaknya  maskapai  yang  bersaing  satu  sama lain,  maka  maskapai  berlomba  untuk  menjadi pilihan   utama   konsumen/pasar,   namun   untuk mencapai   hal   tersebut,   belum   ada   strategi maskapai  yang  dapat  memprediksi  harga  tiket pesawat  sesuai  dengan  kebutuhan  pasar.  Untuk memenuhi kebutuhan maskapai, maka diperlukan  suatu  cara  untuk  menetapkan  harga tiket  pesawat  sesuai  kebutuhan  pasar  dengan bantuan pengaruh teknologi dan informasi. 

Penelitian tentang analisis prediksi harga pesawat didorong oleh beberapa alasan, baik dari perspektif akademis maupun praktis. Industri penerbangan sering mengalami ketidakstabilah harga tiket, banyak pihak perusahan maskapai mencari cara untuk memprediksi harga tiket dengan lebih baik dari data harga sebelumnya. Penelitian ini dapat memberikan wawasan yang berharga bagi perusahaan maskapai dalam mengambil keputusan strategi, sehingga konsumen dapat memprediksi harga tiket pesawat agar memberikan pengalaman perjalanan yang lebih baik. 


## Pengumpulan Data
Pada penelitian ini digunakan dataset Prediksi Harga Tiket Pesawat yang terdokumentasi pada platform kaggle.com detail dari dataset tersebut yaitu : 
a.	Dataset terdiri dari 300.153 records dengan 12 fitur.
b.	Dataset terdiri dari :
•	8 data kategori dengan tipe data object yaitu airline, flight, source_city, departure_time, stops, arrival_time, destination_city, class.
•	4 data numerik dengan satu type data float64 yaitu duration dan 3 tipe data int 4 yaitu unnamed, days_left, dan price.
c.	Data sekunder dikumpulkan dari situs web Easy My Trip. 
d.	Data dikumpulkan selama 50 hari, dari 11 Februari hingga 31 Maret 2022.

## Pengolahan Data dengan Metode Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) adalah tahapan dalam data science untuk memahami dan mengenal dataset. EDA membantu menemukan hubungan signifikan antara variabel dalam dataset besar. Teknik yang umum digunakan dalam EDA meliputi:
1. **Teknik Statistik Deskriptif:** Memberikan ringkasan data seperti mean, median, modus, deviasi standar, dan kuartil.
2. **Analisis Data Univariat:** Eksplorasi satu variabel menggunakan histogram, box plot, dan ringkasan statistik.
3. **Analisis Data Multivariat:** Mengeksplorasi hubungan antar variabel menggunakan matriks korelasi, analisis regresi, dan scatter plot matriks.

## Data Pre-Processing
Data preprocessing memastikan data yang akan dianalisis akurat dan konsisten. Tahapan yang dilakukan meliputi:
1. **Data Ingestion:**
   - Mengimpor data dari CSV menggunakan Pandas
   - Membaca data
   - Mencari duplikasi
   - Mendeteksi missing values
   - Mencari outliers

2. **Data Cleaning:**
   - Dropping baris dengan nilai kosong
   - Imputation untuk mengisi nilai hilang
   - Interpolasi untuk menghasilkan nilai baru dalam jangkauan data

3. **Data Formatting:** Mengubah format data agar sesuai dengan kebutuhan analisis.

## Modeling
1. **Regresi Linear:** Algoritma sederhana untuk memodelkan hubungan linier antara variabel.
2. **Decision Tree:** Pohon keputusan yang digunakan untuk klasifikasi dan regresi dengan fleksibilitas tinggi.
3. **Random Forest:** Algoritma berbasis banyak decision tree untuk meningkatkan akurasi.
4. **XGBoost:** Algoritma boosting yang menggabungkan gradient boosting untuk prediksi yang lebih cepat dan akurat.

## Evaluasi Model
Evaluasi model bertujuan untuk mengukur kinerja prediksi dengan metrik sebagai berikut:
1. **Mean Absolute Error (MAE):** Mengukur rata-rata kesalahan absolut antara nilai prediksi dan aktual.
2. **Mean Squared Error (MSE):** Mengukur rata-rata selisih kuadrat antara nilai prediksi dan aktual.
3. **R-Squared (R²):** Mengukur proporsi varians variabel terikat yang dijelaskan oleh variabel bebas.

Semakin rendah MAE dan MSE serta semakin tinggi nilai R², semakin baik kinerja model.

