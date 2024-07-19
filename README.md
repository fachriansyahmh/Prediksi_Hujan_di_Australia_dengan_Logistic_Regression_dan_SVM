# Prediksi Hujan di Australia dengan Logistic Regression dan SVM

buka link berikut untuk detail projectnya : <a href="https://github.com/fachriansyahmh/Prediksi_Harga_Uber_dan_Lyft_di_Boston_Menggunakan_Linear_Regression/blob/main/PYTN_KampusMerdeka_FP1_Fachriansyah-Muhammad-Haikal.ipynb" target="_blank">Project</a>


## Latar Belakang

Hujan merupakan faktor penting dalam kehidupan sehari-hari. Di Australia, prediksi hujan memiliki nilai signifikan karena negara ini sering mengalami cuaca tidak menentu dan rentan terhadap kekeringan serta bencana alam terkait pola hujan yang tidak teratur.

**Logistic Regression** adalah metode statistik yang digunakan untuk memodelkan hubungan antara variabel dependen biner (hujan atau tidak hujan) dengan satu atau lebih variabel independen (misalnya suhu, kelembaban, tekanan udara, dsb.). Model ini dapat membantu mengidentifikasi pola dan korelasi antara variabel cuaca dan kemungkinan terjadinya hujan di Australia.

**Support Vector Machine (SVM)** adalah algoritma pembelajaran mesin yang digunakan untuk membangun model prediktif dengan melakukan klasifikasi data. SVM mencari batas pemisah antara dua kelas data (hujan atau tidak hujan) yang memaksimalkan jarak antara batas pemisah dan contoh data terdekat dari masing-masing kelas. Algoritma ini dapat digunakan untuk memprediksi apakah suatu wilayah di Australia akan mengalami hujan berdasarkan data cuaca historis dan fitur-fitur relevan.

Dengan memanfaatkan data cuaca historis yang ada, kedua model ini dapat dilatih untuk memahami pola dan hubungan antara variabel cuaca dan kemungkinan hujan di masa depan, sehingga membantu masyarakat di Australia membuat keputusan yang lebih terinformasi.

## Dataset

Dataset yang digunakan dalam proyek ini adalah **Rain in Australia**, yang berisi data cuaca harian selama 10 tahun di Australia. Dataset ini memiliki 145,460 entri dengan 23 atribut. Namun, hanya 22 atribut yang digunakan dalam proyek ini:

- `Location`: Nama kota di Australia
- `MinTemp`: Temperatur terendah hari itu (°C)
- `MaxTemp`: Temperatur tertinggi hari itu (°C)
- `Rainfall`: Jumlah curah hujan hari itu (mm)
- `Evaporation`: Jumlah evaporasi (mm) selama 24 jam sebelum jam 9 pagi
- `Sunshine`: Jumlah jam cerah dengan cahaya matahari
- `WindGustDir`: Arah kecepatan angin tertinggi selama 24 jam sebelum jam 12 malam
- `WindGustSpeed`: Kecepatan angin tertinggi (km/jam) selama 24 jam sebelum jam 12 malam
- `WindDir9am`: Arah angin jam 9 pagi
- `WindDir3pm`: Arah angin jam 3 sore
- `WindSpeed9am`: Kecepatan angin jam 9 pagi (km/jam)
- `WindSpeed3pm`: Kecepatan angin jam 3 sore (km/jam)
- `Humidity9am`: Humiditas jam 9 pagi (%)
- `Humidity3pm`: Humiditas jam 3 sore (%)
- `Pressure9am`: Tekanan udara jam 9 pagi (hPa)
- `Pressure3pm`: Tekanan udara jam 3 sore (hPa)
- `Cloud9am`: Persentase langit yang tertutup awan jam 9 pagi (oktas)
- `Cloud3pm`: Persentase langit yang tertutup awan jam 3 sore
- `Temp9am`: Temperatur jam 9 pagi (°C)
- `Temp3pm`: Temperatur jam 3 sore (°C)
- `RainToday`: Apakah hari ini hujan (1: ya, 0: tidak)
- `RainTomorrow`: Variabel yang diprediksi (1: ya, 0: tidak)

## Objektif

1. Menemukan faktor-faktor yang mempengaruhi terjadinya hujan di Australia.
2. Membandingkan akurasi prediksi hujan di Australia dengan menggunakan model Logistic Regression dan Support Vector Machine.
3. Memberikan wawasan yang bermanfaat bagi masyarakat di Australia.

## Pengambilan Kesimpulan

### 1. Faktor-Faktor

Faktor-faktor yang mempengaruhi hujan esok hari di Australia adalah:

- `Location`
- `MinTemp`
- `MaxTemp`
- `Rainfall`
- `Evaporation`
- `Sunshine`
- `WindGustDir`
- `WindGustSpeed`
- `WindDir9am`
- `WindDir3pm`
- `WindSpeed9am`
- `WindSpeed3pm`
- `Humidity9am`
- `Humidity3pm`
- `Pressure9am`
- `Pressure3pm`
- `Cloud9am`
- `Cloud3pm`
- `Temp9am`
- `Temp3pm`
- `RainToday`

### 2. Akurasi

- Akurasi model Logistic Regression: 75.64%
- Akurasi model Support Vector Machine: 76.61%

Model Support Vector Machine menunjukkan akurasi prediksi yang lebih tinggi dibandingkan Logistic Regression pada dataset ini.

### 3. Wawasan

- Semakin rendah temperatur, kemungkinan besar besok akan hujan.
- Semakin tinggi kelembapan, kemungkinan besar besok akan hujan.
- Semakin rendah tekanan udara, kemungkinan besar besok akan hujan.
- Semakin tinggi kecepatan angin, kemungkinan besar besok akan hujan.
