# Analisis Harga Pangan Pokok Indonesia (2022–2026)

Proyek ini menganalisis data harga 10 komoditas bahan pangan pokok di seluruh 34 provinsi Indonesia dari Januari 2022 hingga Februari 2026. Data bersumber dari sistem pemantauan harga pangan Bank Indonesia (PIHPS) yang tersedia di [bi.go.id/hargapangan](https://www.bi.go.id/hargapangan).

## Komoditas yang Dianalisis

| No | Komoditas       |
|----|-----------------|
| 1  | Bawang Merah    |
| 2  | Bawang Putih    |
| 3  | Beras           |
| 4  | Cabai Merah     |
| 5  | Cabai Rawit     |
| 6  | Daging Ayam     |
| 7  | Daging Sapi     |
| 8  | Gula Pasir      |
| 9  | Minyak Goreng   |
| 10 | Telur Ayam      |

## Struktur Notebook

1. **Import & Load Data** — Memuat 10 file CSV dan menggabungkannya menjadi satu dataframe terpadu
2. **Data Understanding** — Eksplorasi awal: dimensi, tipe data, statistik deskriptif
3. **Data Preprocessing** — Parsing tanggal, deteksi missing values, dan penanganan outlier dengan metode IQR
4. **EDA: Tren Harga Nasional** — Rata-rata harga nasional per komoditas dari waktu ke waktu
5. **EDA: Perubahan Harga Tahunan (YoY)** — Persentase perubahan harga per tahun
6. **EDA: Perbandingan Harga Antar Provinsi** — Heatmap harga per provinsi dan ranking provinsi termahal/termurah
7. **EDA: Volatilitas & Korelasi** — Koefisien variasi dan matriks korelasi antar komoditas
8. **Modeling: Linear Regression** — Prediksi tren harga 30 hari ke depan menggunakan ordinary least squares
9. **Kesimpulan & Insight** — Ringkasan temuan utama dari analisis

## Cara Penggunaan

### 1. Clone repositori

```bash
git clone https://github.com/username/nama-repo.git
cd nama-repo
```

### 2. Install dependensi

```bash
pip install -r requirements.txt
```

### 3. Jalankan notebook

```bash
jupyter notebook analisis_harga_pangan.ipynb
```

atau buka langsung di Google Colab.

## Dependensi

- Python 3.10+
- pandas 2.2.2
- numpy 1.26.4
- matplotlib 3.8.4
- seaborn 0.13.2

## Sumber Data

Data harga pangan bersumber dari **Pusat Informasi Harga Pangan Strategis (PIHPS)** Bank Indonesia, [https://www.bi.go.id/hargapangan](https://www.bi.go.id/hargapangan).
