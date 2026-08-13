# 🛒 Analisis Penjualan Ritel (Retail Sales Analysis)

## 📌 Gambaran Umum
Proyek ini berfokus pada pemrosesan dan analisis data transaksi ritel untuk menghasilkan wawasan bisnis yang dapat ditindaklanjuti. Berawal dari data mentah hingga menjadi laporan yang terstruktur, proyek ini mendemonstrasikan proses end-to-end dalam membersihkan data, menangani nilai anomali (*outliers*), dan menyusun agregasi metrik penjualan.

## 🎯 Tujuan Proyek
*   Membersihkan data transaksi historis dari format mentah menjadi dataset yang siap dianalisis.
*   Mengevaluasi performa penjualan berdasarkan kategori produk, demografi pelanggan (gender dan usia).
*   Mengidentifikasi tren pendapatan bulanan untuk periode 2023 hingga awal 2024.

## 📂 Struktur Data
Proyek ini menggunakan dua dokumen utama sebagai basis data dan pelaporan:

1.  **`retail_practice_workbook (1).xlsx`** 
    Berisi panduan proyek awal serta dataset mentah (`Data_Penjualan_Raw`) yang mencakup titik data seperti ID Pelanggan, Usia, Gender, Kategori Produk, Kuantitas, Harga Satuan, dan Total Belanja.
2.  **`Retail Sales Analysis.xlsx`** 
    Merupakan hasil akhir pengolahan data yang terbagi menjadi tiga *sheet* utama:
    *   **Ringkasan**: Ikhtisar eksekutif pengerjaan proyek.
    *   **Data_Bersih**: Dataset hasil *cleaning* dengan penambahan kolom kategorisasi (*Age Group*, *Month*), perhitungan statistik deskriptif (*Mean*, *STDEV*), serta deteksi status *outlier*.
    *   **Analisis_Sintesis**: Agregasi metrik untuk mengekstrak performa bisnis.

## 📊 Wawasan Utama (Key Insights)
Berdasarkan sintesis data yang dilakukan, ditemukan beberapa temuan penting:
*   **Performa Produk:** *Electronics* menjadi penyumbang pendapatan tertinggi dengan total kontribusi 34,4% ($156.905), disusul secara ketat oleh *Clothing* (34,1%) dan *Beauty* (31,4%).
*   **Demografi Pelanggan:** Pembeli perempuan (*Female*) sedikit mendominasi total pendapatan sebesar 51% dibandingkan pembeli laki-laki (*Male*) di angka 49%.
*   **Tren Waktu:** Tren pendapatan bulanan berfluktuasi cukup signifikan, dengan puncak penjualan tertinggi terjadi pada bulan Mei 2023 yang melampaui $53.000.

## 🛠️ Metodologi & Langkah-langkah
1.  **Ekstraksi Data:** Menarik data historis dari file *raw* tabular.
2.  **Transformasi Data:** Mengelompokkan pelanggan ke dalam rentang usia dan mengekstrak format waktu (Bulan-Tahun) dari kolom tanggal transaksi.
3.  **Kendali Mutu (Quality Control):** Menerapkan perhitungan statistika dasar untuk memfilter dan menandai transaksi anomali (Normal vs. Outlier).
4.  **Agregasi & Pelaporan:** Melakukan pivot data untuk menghitung total kuantitas, total pendapatan, dan persentase kontribusi dari masing-masing segmen bisnis.
