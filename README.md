# UMKM Inventory Analytics Dashboard

Dashboard analisis inventori UMKM menggunakan **Microsoft Power BI** untuk memantau stok barang, menganalisis transaksi masuk dan keluar, serta mengidentifikasi produk dengan stok rendah.

## 1. Project Overview

Proyek ini dibuat untuk mengolah data inventori menjadi informasi yang lebih mudah dipahami melalui visualisasi dashboard.

Data yang digunakan merupakan dataset simulasi selama tiga bulan, mulai dari 1 Maret sampai 30 Mei 2026. Dataset disusun berdasarkan struktur database dari sistem inventori berbasis web yang sebelumnya dikembangkan menggunakan Laravel sebagai bagian dari proyek tugas akhir.

Dengan Power BI, data tersebut diolah menjadi beberapa visualisasi agar kondisi persediaan dan aktivitas transaksi dapat dipantau dengan lebih mudah.

### Project Objectives

- Menampilkan informasi jumlah produk dan total stok.
- Memantau transaksi barang masuk dan keluar.
- Mengetahui produk yang memiliki stok rendah.
- Mengidentifikasi produk dengan jumlah barang keluar tertinggi.
- Melihat aktivitas transaksi berdasarkan tanggal dan supplier.

## 2. Business Problem

Dalam pengelolaan inventori, pencatatan barang saja belum cukup untuk memberikan gambaran mengenai kondisi persediaan. Data yang terkumpul perlu diolah agar dapat membantu proses pemantauan dan pengambilan keputusan.

Beberapa hal yang menjadi fokus dalam proyek ini:

1. **Pemantauan stok barang:** Mengetahui produk yang memiliki stok rendah agar dapat segera diperiksa dan ditindaklanjuti.
2. **Aktivitas transaksi:** Memahami jumlah dan kuantitas barang yang masuk maupun keluar selama periode tertentu.
3. **Produk dengan aktivitas tinggi:** Mengetahui produk yang paling banyak keluar sebagai bahan pertimbangan dalam pengelolaan stok.
4. **Informasi inventori:** Menggabungkan informasi produk, kategori, supplier, dan transaksi ke dalam satu dashboard agar lebih mudah dianalisis.

Melalui dashboard ini, informasi inventori disajikan dalam bentuk KPI, grafik, tabel, dan filter interaktif.

## 3. Dataset Overview

Dataset yang digunakan merupakan data simulasi dengan periode pengamatan selama tiga bulan.

| Informasi | Jumlah |
|---|---:|
| Periode data | 1 Maret – 30 Mei 2026 |
| Jumlah produk | 50 produk |
| Total stok | 40.409 unit |
| Transaksi masuk | 198 transaksi |
| Transaksi keluar | 2.422 transaksi |
| Total barang masuk | 56.407 unit |
| Total barang keluar | 20.885 unit |

> **Catatan:** Seluruh data merupakan data simulasi untuk kebutuhan pengembangan proyek dan portofolio, bukan data operasional UMKM sebenarnya.

## 4. Dashboard Preview

Dashboard terdiri dari tiga halaman utama:

### 4.1 Overview

Menampilkan ringkasan kondisi inventori melalui KPI, grafik tren transaksi, produk dengan barang keluar tertinggi, serta informasi kategori dan supplier.

![Overview Dashboard](Preview/01-Overview.png)

### 4.2 Inventory Detail

Menampilkan informasi stok setiap produk, kategori, supplier, dan status persediaan. Halaman ini juga membantu melihat produk dengan stok terendah.

![Inventory Detail Dashboard](Preview/02-Inventory-Detail.png)

### 4.3 Transaction Analysis

Menampilkan aktivitas transaksi barang masuk dan keluar, perbandingan kuantitas barang, tren transaksi berdasarkan tanggal, serta riwayat transaksi.

![Transaction Analysis Dashboard](Preview/03-Transaction-Analysis.png)

## 5. Key Insights

Berdasarkan hasil pengolahan dan visualisasi data, terdapat beberapa informasi yang dapat diperoleh:

1. **Kondisi stok:** Dari 50 produk, terdapat 2 produk dengan status stok rendah dan 48 produk dengan status stok aman. Penentuan status menggunakan batas minimum 20 unit.
2. **Barang masuk:** Selama periode pengamatan, tercatat sebanyak 56.407 unit barang masuk.
3. **Barang keluar:** Total barang yang keluar selama periode pengamatan mencapai 20.885 unit.
4. **Jumlah transaksi:** Terdapat 198 transaksi masuk dan 2.422 transaksi keluar.
5. **Produk dengan barang keluar tertinggi:** Beberapa produk seperti Indomie Goreng, Le Minerale, dan Mie Sedaap Ayam Bawang termasuk produk dengan kuantitas barang keluar tertinggi pada visualisasi.
6. **Tren transaksi:** Aktivitas barang masuk dan keluar mengalami perubahan sepanjang periode pengamatan dan dapat dipantau melalui grafik tren.

## 6. Recommendations

Dari hasil analisis tersebut, beberapa tindakan yang dapat dipertimbangkan adalah:

1. **Memeriksa stok rendah:** Produk dengan stok 20 unit atau kurang perlu diperhatikan dan dievaluasi untuk menentukan kebutuhan pengadaan ulang.
2. **Memantau produk dengan barang keluar tinggi:** Produk yang memiliki jumlah barang keluar tinggi perlu mendapatkan perhatian lebih dalam perencanaan persediaan.
3. **Mengevaluasi transaksi secara berkala:** Data barang masuk dan keluar dapat digunakan untuk melihat perubahan aktivitas persediaan dari waktu ke waktu.
4. **Memperhatikan supplier:** Informasi supplier dapat dimanfaatkan sebagai bahan evaluasi dalam proses pengadaan barang.
5. **Memperbarui data inventori:** Pembaruan data secara rutin diperlukan agar informasi yang ditampilkan tetap sesuai dengan kondisi persediaan terbaru.

## 7. Tools & Technologies

| Tools | Penggunaan |
|---|---|
| Microsoft Power BI | Membuat dashboard dan visualisasi data |
| Power Query | Mengolah dan menggabungkan data |
| DAX | Membuat measure dan perhitungan analisis |
| Laravel | Sistem inventori berbasis web sebagai dasar struktur dataset |
| CSV / Database | Sumber data untuk analisis |

## 8. Project Limitations

- Data yang digunakan merupakan data simulasi dengan periode tiga bulan.
- Hasil analisis hanya menggambarkan kondisi berdasarkan dataset yang tersedia.
- Batas stok rendah sebesar 20 unit ditentukan sebagai aturan untuk kebutuhan analisis.
- Dashboard berfokus pada analisis deskriptif dan pemantauan inventori, bukan prediksi stok secara langsung.

---

**Project Type:** Data Analytics Portfolio Project

**Focus:** Inventory Analysis, Transaction Analysis, Data Visualization

**Tools:** Power BI, Power Query, DAX, Laravel
