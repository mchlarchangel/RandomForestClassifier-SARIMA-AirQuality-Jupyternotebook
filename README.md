# **Data Logging ESP32 Forecasting and Classification**
## **Deskripsi Proyek**
Proyek ini bertujuan untuk memproses data yang dikumpulkan oleh ESP32 dan melakukan klasifikasi kualitas udara serta forecasting untuk beberapa fitur lingkungan seperti Humidity, Temperature, CO2, CO, dan PM2.5 Density. Data ini diolah untuk menghasilkan prediksi kualitas udara pada waktu pagi, siang, sore, dan malam, serta menghitung beberapa metrik evaluasi model.

## **Dataset**
Dataset yang digunakan berisi fitur-fitur berikut:
+ Date and Time
+ Humidity
+ Temperature
+ CO2
+ CO
+ PM2.5 Density

## **Klasifikasi menggunakan Random Forest**
+ Menghitung AQI (Air Quality Index) berdasarkan konsentrasi PM2.5, CO, dan CO2 menggunakan breakpoints sesuai standarts AQI.
+ Mengkategorikan kualitas udara ke dalam tiga kategori: Baik, Sedang, Buruk.
+ Memisahkan data menjadi training dan test set.
+ Mengevaluasi akurasi model menggunakan confusion matrix, classification report, dan cross-validation.

## **Forecasting Menggunakan SARIMA**
+ Mengelompokkan data berdasarkan tanggal dan waktu (pagi, siang, sore, malam).
+ Menggunakan model SARIMA untuk melakukan forecasting 4 langkah ke depan (1 hari kedepan) untuk setiap fitur.

## **Kesimpulan**
Proyek ini berhasil memproses dan menganalisis data lingkungan dari ESP32 untuk tujuan klasifikasi dan forecasting. Model yang digunakan memberikan hasil yang memuaskan dalam memprediksi kualitas udara dan nilai fitur lingkungan di masa depan.
