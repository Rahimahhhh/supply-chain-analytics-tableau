# Supply Chain Analytics Dashboard

## Tentang Proyek

Dataset yang saya gunakan berisi catatan transaksi dari beberapa pemasok, mencakup data produk, rute pengiriman, biaya logistik, dan informasi pelanggan. Dari data mentah ini, saya mencoba menjawab satu pertanyaan utama: **di mana sebetulnya pendapatan dan efisiensi operasional bisa dioptimalkan?**

Proses dimulai dari data cleaning di Excel menghapus duplikasi, menstandardisasi nama kategori produk yang tidak konsisten, dan memvalidasi kolom biaya yang nilainya ada di luar rentang wajar. Setelah data siap, analisis dan visualisasi dilakukan di Tableau Public.

## Temuan Utama

**Sisi komersial:**
- Tiga pemasok teratas menyumbang lebih dari 60% total pendapatan, tapi lead time mereka lebih panjang dibanding pemasok menengah. Ini membuka pertanyaan soal trade-off antara volume dan keandalan pasokan.
- Segmen pelanggan tertentu menunjukkan frekuensi pembelian tinggi tapi nilai transaksi rendah, pola yang berbeda dari segmen dengan nilai tinggi tapi jarang memesan. Keduanya butuh pendekatan komersial yang berbeda.

**Sisi operasional:**
- Biaya pengiriman bervariasi signifikan antar rute, tapi tidak selalu berkorelasi dengan jarak. Beberapa rute pendek justru lebih mahal karena pilihan moda transportasi yang kurang efisien.
- Satu carrier menunjukkan konsistensi waktu pengiriman yang lebih baik dari yang lain dengan selisih biaya yang tidak terlalu besar.

## Dashboard

### Executive Overview
Ringkasan KPI pendapatan, pemasok teratas, dan segmentasi pelanggan untuk kebutuhan pelaporan ke manajemen.

![Executive Overview](images/executive_dashboard.png)

**[Buka di Tableau Public](https://public.tableau.com/shared/P4X326HKZ?:display_count=n&:origin=viz_share_link)**

### Logistics & Operations
Analisis biaya per rute, perbandingan carrier, dan efisiensi moda transportasi untuk kebutuhan tim operasional.

![Logistics & Operations](images/logistics_dashboard.png)

**[Buka di Tableau Public](https://public.tableau.com/views/LogisticsOperationsDashboard_17827015433220/LogisticsOperations?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**

## Alur Kerja

```
Raw Data (CSV)
    ↓
Data Cleaning & Validasi — Microsoft Excel
(hapus duplikat, standardisasi kategori, validasi outlier biaya)
    ↓
Visualisasi & Analisis — Tableau Public
(2 dashboard: eksekutif + operasional)
    ↓
Insight & Rekomendasi
```

## Tools

| Tahap | Tools |
|---|---|
| Data Cleaning | Microsoft Excel |
| Visualisasi | Tableau Public |

## Struktur Repositori

```
Supply-Chain-Analytics/
├── dashboard/
│   ├── Logistics & Operations Dashboard.twbx
│   └── Supply Chain Executive Dashboard.twbx
├── dataset/
│   └── supply_chain_data.csv
├── images/
│   ├── executive_dashboard.png
│   └── logistics_dashboard.png
└── README.md
```
