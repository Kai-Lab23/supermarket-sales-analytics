# Sales Analysis Project

## Overview

Project ini menganalisis data penjualan supermarket untuk memahami pola penjualan, perilaku pelanggan, distribusi profit, dan peluang perbaikan bisnis.

Analisis dilakukan menggunakan pendekatan Exploratory Data Analysis (EDA) dengan Python, Pandas, Matplotlib, dan Seaborn.

## Business Objective

Tujuan dari project ini adalah untuk memahami performa sales dan profit berdasarkan kategori produk, kota, hari, dan jam agar dapat mendukung pengambilan keputusan bisnis berbasis data.

## Dataset

Dataset yang digunakan berisi 1.000 data transaksi supermarket.

Beberapa kolom utama dalam dataset:

- Invoice ID
- Branch
- City
- Customer type
- Gender
- Product line
- Unit price
- Quantity
- Tax 5%
- Sales
- Date
- Time
- Payment
- cogs
- gross margin percentage
- gross income
- Rating

## Tools yang Digunakan

- Python
- Pandas
- Matplotlib
- Seaborn
- Google Colab

## Struktur Project

```text
sales-analysis-colab/
├── data/
│   ├── raw/
│   │   └── supermarket-sales/
│   └── processed/
│       └── clean_data.csv
│
├── outputs/
│   ├── figures/
│   │   ├── Sales_by_category.png
│   │   ├── Profit_by_category.png
│   │   ├── Daily_sales_pattern.png
│   │   ├── Hourly_sales_pattern.png
│   │   ├── Profit_by_city.png
│   │   └── Correlation_analysis.png
│   │
│   └── summary/
│       └── business_summary.csv
│
├── notebooks/
│   └── sales_analysis.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Alur Analisis

1. Data Understanding
   - Mengecek ukuran dataset, nama kolom, tipe data, missing values, duplicate values, dan statistik deskriptif.

2. Data Cleaning
   - Mengubah kolom Date dan Time ke format datetime.
   - Mengubah beberapa kolom menjadi tipe data category.
   - Menstandarkan nilai pada kolom kategorikal.
   - Membuat kolom tambahan berbasis waktu seperti year, month, month_name, day, day_name, dan hour.
   - Menyimpan data bersih ke file `clean_data.csv`.

3. Exploratory Data Analysis
   - Analisis total sales dan profit
   - Sales berdasarkan kategori produk
   - Profit berdasarkan kategori produk
   - Pola penjualan harian
   - Pola penjualan per jam
   - Profit berdasarkan kota
   - Analisis korelasi

4. Business Interpretation
   - Key Insights
   - Business Recommendations
   - Conclusion

## Data Limitation

Dataset hanya mencakup transaksi pada periode Januari hingga Maret 2019. Oleh karena itu, analisis tren jangka panjang belum dapat dilakukan. Analisis difokuskan pada pola perilaku penjualan dalam jangka pendek dan pola transaksi berdasarkan kategori, kota, hari, serta jam.

## Key Insights

1. Penjualan dan profit terutama dipengaruhi oleh Quantity dan Unit Price, sementara margin cenderung konstan di seluruh kategori.
2. Distribusi penjualan dan profit antar kategori serta kota relatif merata, menunjukkan bahwa bisnis tidak bergantung pada satu segmen atau wilayah tertentu.
3. Pola penjualan harian cenderung stabil tanpa perbedaan signifikan antar hari.
4. Analisis per jam menunjukkan adanya peningkatan aktivitas pada jam istirahat siang dan malam.
5. Analisis korelasi menunjukkan bahwa Sales dipengaruhi oleh Quantity dan Unit Price, sementara variabel turunan seperti cogs, gross income, dan Tax 5% memiliki korelasi sempurna karena hubungan matematis.

## Business Recommendations

1. Prioritaskan strategi penjualan pada faktor yang paling mendorong Sales, yaitu Quantity dan Unit Price.
2. Optimalkan kesiapan operasional pada jam puncak, terutama saat istirahat siang dan malam.
3. Evaluasi jam dengan performa lebih rendah untuk mencari peluang peningkatan penjualan secara terbatas.
4. Pertahankan distribusi penjualan yang sudah merata antar kategori dan kota agar bisnis tetap stabil.
5. Interpretasikan hasil korelasi secara hati-hati, terutama pada variabel yang saling terhubung secara matematis.

## Conclusion

Secara keseluruhan, bisnis menunjukkan performa penjualan dan profit yang relatif stabil di berbagai kategori, kota, dan hari. Faktor utama yang mendorong penjualan adalah Quantity dan Unit Price, sementara pola per jam menunjukkan adanya aktivitas yang lebih tinggi pada jam istirahat siang dan malam.

Temuan ini menunjukkan bahwa peluang optimasi lebih banyak berada pada strategi volume penjualan dan pengelolaan operasional pada jam-jam tertentu.

## Author

Khairu Ikramendra
