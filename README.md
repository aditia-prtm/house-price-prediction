# Prediksi Harga Rumah

Project machine learning sederhana untuk memprediksi harga rumah menggunakan **Linear Regression**, berdasarkan fitur-fitur seperti luas bangunan, jumlah kamar tidur, jarak ke pusat kota, dan usia bangunan.

## Deskripsi

Project ini membangun model regresi linear untuk memprediksi harga rumah dari 4 fitur utama:

- **Luas bangunan** (m²)
- **Jumlah kamar tidur**
- **Jarak ke pusat kota** (km)
- **Usia bangunan** (tahun)

Dataset yang digunakan merupakan data simulasi sebanyak 500 sampel rumah yang dibuat secara sintetis dengan pola harga yang realistis (dipengaruhi luas, jumlah kamar, jarak kota, usia bangunan, dan noise acak).

## Library yang Digunakan

- `pandas` — manipulasi dan analisis data
- `numpy` — komputasi numerik
- `matplotlib` & `seaborn` — visualisasi data
- `scikit-learn` — pemodelan machine learning (Linear Regression, train-test split, standardisasi, evaluasi metrik)

## Instalasi

Pastikan Python 3 sudah terinstal, lalu install dependensi berikut:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## Cara Menjalankan

1. Clone atau unduh repository ini.
2. Jalankan Jupyter Notebook:
   ```bash
   jupyter notebook main.ipynb
   ```
3. Jalankan seluruh sel (cell) secara berurutan dari atas ke bawah (`Run All`).

## Alur Project

| Tahap | Deskripsi |
|-------|-----------|
| 1. Import Library | Mengimpor seluruh library yang dibutuhkan |
| 2. Generate Dataset | Membuat dataset simulasi 500 rumah |
| 3. Eksplorasi Data (EDA) | Statistik deskriptif, cek missing value, visualisasi distribusi & korelasi |
| 4. Preprocessing Data | Split data (80% training / 20% testing) & standardisasi fitur |
| 5. Training Model | Melatih model Linear Regression |
| 6. Evaluasi Model | Menghitung MAE, RMSE, dan R² serta visualisasi aktual vs prediksi |
| 7. Prediksi Harga Rumah Baru | Menguji model pada data rumah baru |
| 8. Kesimpulan | Ringkasan hasil dan insight dari model |

## Hasil Model

| Metrik | Nilai |
|--------|-------|
| Model | Linear Regression |
| Jumlah Data | 500 sampel |
| Training / Testing | 80% / 20% |
| R² Score | ~0.95+ |

**Insight dari model:**
- Luas bangunan adalah faktor terbesar penentu harga rumah.
- Setiap kamar tidur tambahan meningkatkan harga secara signifikan.
- Semakin jauh dari pusat kota, harga rumah cenderung semakin turun.
- Usia bangunan berpengaruh negatif terhadap harga rumah.

## Struktur Project

```
.
├── main.ipynb      # Notebook utama berisi seluruh proses analisis dan pemodelan
└── README.md        # Dokumentasi project
```

## Catatan

Dataset pada project ini bersifat **simulasi/sintetis** (dibuat dengan `numpy.random`) dan digunakan untuk keperluan pembelajaran konsep regresi linear, bukan data harga rumah nyata.