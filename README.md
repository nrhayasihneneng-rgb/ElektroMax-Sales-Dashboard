# ElektroMax-Sales-Dashboard
Dashboard Power BI interaktif untuk menganalisis kinerja penjualan, produk, toko, dan segmen pelanggan ritel elektronik.
# Dashboard Kinerja Penjualan ElektroMax

Dashboard Power BI interaktif yang menganalisis kinerja penjualan **ElektroMax**, jaringan ritel elektronik konsumen: omzet, laba kotor, produk, toko, dan segmen pelanggan.

> Proyek latihan · Alat: Power BI, Power Query, DAX

![Overview](<img width="668" height="376" alt="Screenshot 2026-10-31 230902" src="https://github.com/user-attachments/assets/6117a7cc-2b43-4fe7-a802-d2b7295654a5" />
)

## Latar Belakang

Proyek latihan ini menganalisis kinerja penjualan jaringan ritel elektronik konsumen. Analisis berfokus pada omzet, laba kotor, produk, toko, dan segmen pelanggan untuk mengidentifikasi pola serta menghasilkan insight berbasis data bagi perencanaan penjualan dan pengambilan keputusan.

## Tujuan

- Menganalisis omzet, laba kotor, dan transaksi berdasarkan toko, wilayah, subkategori produk, dan periode waktu.
- Membandingkan kinerja dengan tahun sebelumnya (YoY).
- Memahami segmen pelanggan, kelompok umur, jenis kelamin, dan metode pembayaran.
- Memberikan insight dan rekomendasi yang dapat ditindaklanjuti untuk mendukung perencanaan penjualan.

## Model Data

Star schema dengan satu tabel fakta dan enam tabel dimensi:

| Tabel | Jenis |
|---|---|
| `FACT_PENJUALAN` | Fakta (transaksi penjualan) |
| `DIM_PELANGGAN` | Dimensi (pelanggan) |
| `DIM_PRODUK` | Dimensi (produk) |
| `DIM_PROMOSI` | Dimensi (promosi) |
| `DIM_TOKO` | Dimensi (toko) |
| `DIM_WAKTU` | Dimensi (waktu) |
| `DIM_KARYAWAN` | Dimensi (karyawan) |
| `_MEASURE` | Tabel penyimpan measure DAX |

## Measure DAX Utama

Total Omzet, Gross Profit, GPM % (margin laba kotor), Growth YoY Omzet, Omzet LY (omzet tahun lalu), Avg Ticket Size, Jumlah Transaksi, Jumlah Pelanggan, Avg Frekuensi, % Transaksi Promo, % Retur.

## Halaman Dashboard

| Halaman | Isi | Filter |
|---|---|---|
| **Overview** | Kartu KPI, tren omzet vs tahun lalu, omzet per subkategori, tabel toko | Wilayah, Tahun |
| **Produk & Toko** | Omzet per toko dan region, tren dan margin subkategori, detail produk | Subkategori, Region, Tahun |
| **Pelanggan** | Omzet per segmen, kelompok umur, jenis kelamin, metode bayar, dan promosi | Kota, Segmen, Tahun |

![Produk & Toko](<img width="669" height="373" alt="Screenshot 2026-10-31 230942" src="https://github.com/user-attachments/assets/013d19f6-70e6-4355-9d29-27ff92ce1869" />
)
![Pelanggan](<img width="668" height="376" alt="Screenshot 2026-10-31 231018" src="https://github.com/user-attachments/assets/013fe9fa-577c-4c2e-8f30-82364ea6ba02" />
)

## Key Insight (2025, semua wilayah)

- Total omzet mencapai **Rp95,43 miliar** dari **18.827 transaksi**, sekitar **Rp5,07 juta** per transaksi, dengan margin laba kotor sekitar **31%**.
- **Televisi dan AC** adalah dua subkategori produk terbesar, disusul Kulkas dan Mesin Cuci. Subkategori kecil (Microwave, Water Heater, Vacuum Cleaner, Small Appliance) berkontribusi jauh lebih sedikit.
- Omzet **merata antar toko**: toko yang terlihat berada di kisaran Rp9,13–10,13 miliar.
- Omzet harian **naik di November–Desember 2025**, dengan lonjakan tajam di akhir November. Pola akhir tahun serupa muncul pada tahun sebelumnya.
- Segmen **Regular** menyumbang **51,4%** omzet dan 51,4% transaksi.
- Nilai per transaksi **hampir sama di semua segmen** (sekitar Rp4,99–5,18 juta).
- Pelanggan usia **25–45 tahun menghasilkan 65,9%** omzet, sedangkan usia di bawah 25 hanya **8,6%**.
- Omzet perempuan (52,3%) dan laki-laki (47,5%) hampir seimbang.

## Rekomendasi

- Siapkan stok dan promo untuk November–Desember, saat permintaan memuncak.
- Prioritaskan ketersediaan Televisi dan AC sebagai kontributor omzet terbesar.
- Evaluasi subkategori kecil dengan data margin: pertahankan, bundling dengan produk besar, atau kurangi.
- Fokuskan promosi ke usia 25–45 dan pertahankan pelanggan Regular lewat program pelanggan setia.
- Jalankan kampanye uji coba untuk usia di bawah 25, lalu pantau perubahan porsi omzetnya.
- Pantau toko secara rutin: karena omzet antar toko berdekatan, penurunan mudah terlihat.

## Penulis

**Neneng Nurhayasih** · Lulusan Matematika · Analitik data

[LinkedIn](https://www.linkedin.com/in/neneng-nurhayasih)
