# Analisis Penjualan & Kinerja Perusahaan (Company Sales & Performance Analytics)

Repositori portofolio data analyst ini berisi proyek end-to-end analisis penjualan perusahaan, mulai dari pembersihan data mentah (*data cleaning*), pengelolaan basis data, hingga visualisasi data interaktif menggunakan Python dan SQLite.

---

## 📁 Struktur Direktori & File
- **`raw_sales_data_messy.csv`**: Dataset penjualan mentah sebelum dibersihkan (mengandung nilai kosong, inkonsistensi format, dll).
- **`cleaned_sales_data.csv`**: Dataset hasil pembersihan (*data cleaning*) yang siap digunakan untuk analisis lanjutan.
- **`data__cleaning.ipynb`**: Notebook Jupyter yang mendokumentasikan proses *data wrangling* dan pembersihan data.
- **`visualization.ipynb`**: Notebook Jupyter untuk eksplorasi dan visualisasi data penjualan.
- **`company_sales.db`**: Basis data SQLite yang menyimpan tabel bersih (`sales_performance`).
- **`company_sales.sqbpro`**: File proyek SQLite Studio untuk manajemen basis data.

---

## 📊 Ringkasan & Temuan Utama (Key Findings)

Berdasarkan analisis terhadap **515 transaksi** penjualan dalam basis data perusahaan:

1. **Total Pendapatan (*Total Transaction Value*)**:
   - Total keseluruhan nilai transaksi: **~Rp 1.45 Miliar**
   - Rata-rata nilai per transaksi bervariasi tergantung kategori produk dan diskon.

2. **Kategori Produk Unggulan**:
   - **Elektronik**: Merupakan kontributor pendapatan terbesar (mendominasi pasar dengan nilai ~Rp 944 Juta).
   - Kategori lainnya meliputi **Olahraga** (~Rp 162 Juta), **Rumah Tangga** (~Rp 150 Juta), serta kategori Pakanan, Kesehatan, Pakaian, dan Kecantikan.

3. **Distribusi Penjualan Berdasarkan Kota**:
   - Penjualan tersebar di berbagai kota besar seperti **Yogyakarta** (~Rp 221 Juta), **Bali** (~Rp 206 Juta), **Makassar**, **Bandung**, dan **Jakarta**.

---

## 🛠️ Teknologi & Tools yang Digunakan
- **Python**: Pemrosesan dan manipulasi data (`pandas`, `numpy`)
- **Visualisasi**: `matplotlib`, `seaborn`
- **Database**: SQLite (`company_sales.db`, SQLite Studio `company_sales.sqbpro`)
- **Environment**: Jupyter Notebook

---

## 🚀 Cara Menjalankan Proyek
1. Pastikan pustaka Python terinstal (`pandas`, `matplotlib`, `seaborn`).
2. Jalankan Jupyter Notebook untuk melihat proses pembersihan dan visualisasi:
   ```bash
   jupyter notebook "data__cleaning.ipynb"
   jupyter notebook "visualization.ipynb"
   ```
3. Akses basis data menggunakan SQLite atau SQLite Studio dengan membuka file `company_sales.db`.
