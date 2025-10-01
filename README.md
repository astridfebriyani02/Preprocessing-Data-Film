# Preprocessing-Data-Film

## Deskripsi Proyek
Repositori ini menyediakan kumpulan skrip Python yang digunakan untuk membersihkan sekaligus menyiapkan (preprocessing) dataset film. Tahap preprocessing menjadi pondasi penting dalam proses data science karena menentukan mutu data yang nantinya dipakai dalam analisis maupun pemodelan. Data yang rapi dan konsisten akan mengurangi risiko kesalahan interpretasi.
## Konteks
Analisis data di industri perfilman sangat membantu dalam menilai faktor-faktor yang memengaruhi kesuksesan sebuah film. Beberapa ukuran utama yang sering dipakai adalah judul film, pendapatan kotor (gross), anggaran produksi (budget), genre, dan rating penonton, dll. Pada praktiknya, dataset mentah jarang sekali langsung siap pakai. Informasi di dalamnya kerap tidak lengkap, tidak konsisten, atau mengandung error. Tanpa proses perapihan, analisis dan pemodelan yang dibangun dari data tersebut akan menghasilkan keluaran yang menyesatkan.
## Problem Statement (Permasalahan)
Dataset film mentah biasanya menghadapi sejumlah kendala, di antaranya:
- Adanya missing values pada informasi penting seperti pendapatan dan budget.
- Nilai yang tidak konsisten atau kesalahan penulisan
- Adanya nilai yang tidak standar
Maka dari itu, kendala ini perlu ditangani sebelum data dimanfaatkan lebih jauh.
## Tujuan
Proyek ini berfokus pada pembersihan dataset agar data yang semula mentah berubah menjadi lebih terstruktur dan dapat dipakai dengan aman. Langkah-langkah utamanya mencakup:
- Memeriksa dan menyusun kembali format data agar seragam.
- Membersihkan data dengan cara mengisi atau menghapus data yang hilang dan tidak logis.
- Menghasilkan file movie_dataset_cleaned.csv yang siap untuk analisis, visualisasi, maupun machine learning.
## Dataset
Data awal (movie_sample_dataset.csv) berisi informasi seputar film, mencakup: nama sutradara, durasi, anggaran, pendapatan kotor, tahun rilis, skor IMDb, negara, format (berwarna/hitam putih), genre, bahasa, pemeran, jumlah like di Facebook, serta judul film.
## Proses Preprocessing
Skrip Preprocessing_Data.ipynb menjalankan beberapa tahap preprocessing data, diantaranya:
1. Pembersihan data, diantaranya
   - Penananganan (menghapus) nilai yang hilang, seperti pada kolom gross dan budget.
   - Penananganan nilai yang tidak konsisten atau kesalahan penulisan, seperti perbedaan penulisan antara "color" dan "Color".
   - Mengubah atau menghapus nilai yang tidak standar, seperti nilai negatif atau N/A.
2. Transformasi Data
   - Memisahkan kolom yang awalnya tergabung menjadi beberapa kolom terpisah seperti pada kolom genre.
   - Menormalisasi teks, seperti mengubah teks menjadi huruf kecil.
## Hasil
Output preprocessing berupa file movie_dataset_cleaned.csv yang lebih konsisten, valid, dan siap digunakan. Seluruh variabel telah melalui validasi sehingga masalah umum seperti missing values atau kesalahan input dapat diminimalisir.
## Rekomendasi Lanjutan
Dengan dataset bersih ini, beberapa analisis yang dapat dilakukan antara lain:
- Statistik deskriptif untuk menguji korelasi antar variabel (misalnya anggaran, durasi, pendapatan).
- Visualisasi tren berdasarkan tahun, sutradara, atau genre.
- Pemodelan prediktif menggunakan machine learning untuk memperkirakan pendapatan atau rating penonton.
