# 📊 E-Commerce Sales Performance & Revenue Optimization Strategy

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?style=flat&logo=pandas)
![Status](https://img.shields.io/badge/Project-Portfolio%20Ready-green)

Project ini menganalisis tren transaksi bisnis e-commerce (2011) untuk mengidentifikasi pola musiman (*seasonality*) dan merumuskan rekomendasi alokasi stok serta strategi pemasaran berbasis data.

---

## 👤 About Me
* **Name:** Muhammad Fauzan Rizkiatama Syam
* **Target Role:** Data Analyst / Business Intelligence Analyst
* **Focus Skills:** End-to-End Data Analysis, Data Cleaning, Storytelling
* **Links:** [LinkedIn](https://linkedin.com) | [GitHub](https://github.com)

---

## 📌 Project Overview & Business Context
Perusahaan e-commerce retail menghadapi tantangan fluktuasi permintaan bulanan dan risiko kehabisan stok (*out-of-stock*) pada periode sibuk. Project ini dipilih karena masalah musiman (*seasonality*) merupakan salah satu tantangan paling kritis pada industri E-Commerce yang berdampak langsung pada *cashflow* dan kepuasan pelanggan.

### Objectives:
1. Memahami tren pendapatan bulanan sepanjang tahun 2011.
2. Mengidentifikasi bulan *peak season* untuk perencanaan pasokan barang.
3. Menyusun rekomendasi operasional dan strategi pemasaran berbasis data.

---

## 🛠️ Data Pipeline & Feature Engineering
* **Data Cleaning:** Dari 4,870 baris data awal, dilakukan pembersihan data transaksi yang tidak valid (`Quantity <= 0` dan `UnitPrice <= 0`) hingga menghasilkan 4,549 baris data transaksi bersih.
* **Feature Engineering:**
  * Ekstraksi komponen waktu dari `InvoiceDate`: `YearMonth`, `MonthName`, `DayName`, dan `Hour`.
  * Perhitungan total nilai transaksi: `TotalAmount = Quantity * UnitPrice`.

---

## 📈 Key Findings & Insights
* **Total Revenue 2011:** **$94,570.36** dari 4,549 transaksi bersih.
* **Fase Stabil (Q1–Q2):** Pendapatan relatif stabil di angka rata-rata **$6.5K – $7.5K** per bulan.
* **Peak Season (November):** Bulan **November 2011** mencatatkan puncak penjualan tertinggi sebesar **$17,948.84** (menyumbang **19.0%** dari total pendapatan tahunan, naik **+76.3%** dibandingkan Oktober).
* **Pola Pre-Holiday Restocking:** Kenaikan penjualan mulai terjadi secara konsisten sejak bulan Agustus ($9.9K), menandakan reseller/pembeli melakukan stok barang lebih awal sebelum periode libur akhir tahun.

> ⚠️ **Catatan Data Desember:** Data bulan Desember 2011 hanya mencakup transaksi hingga tanggal 9 Desember (data parsial), sehingga penurunan grafik di bulan Desember bukan menunjukkan penurunan penjualan riil.

---

## 💡 Business Recommendations
1. **Inventory Readiness:** Meningkatkan kapasitas stok produk *top-selling* sebesar 80–100% pada bulan September–Oktober untuk mengantisipasi *surge* di bulan November.
2. **Marketing & Campaign Timing:** Meluncurkan promo *early bird* atau *bulk order discount* pada pertengahan Agustus untuk mengunci pesanan B2B lebih awal.
3. **Customer Retention:** Memberikan insentif/poin bagi pelanggan yang bertransaksi di bulan *low-season* (Januari–April) agar *engagement* tetap terjaga sepanjang tahun.

---

## 📂 Repository Structure
```text
├── ecommerce.csv                   # Raw Dataset
├── Fauzan_on_Assignment_D20_.ipynb # Jupyter Notebook (Python Analysis Code)
├── portofolio_2.pdf                 # Executive Slide Presentation
└── README.md                        # Documentation File
