#Project ini digunakan sebagai penyelesaian project akhir statistika kelas C kelompok 6
# Laporan Analisis Statistika  
## Uji Normalitas dan One Sample t-Test Data Nilai Matematika Siswa Group C pada Dataset Student Study Performance

## Deskripsi Proyek
Proyek ini merupakan analisis statistika inferensial menggunakan metode **One Sample t-Test** untuk menguji apakah rata-rata nilai matematika siswa dari **Group C** pada dataset *Student Study Performance* berbeda secara signifikan terhadap nilai hipotesis tertentu.

Sebelum dilakukan pengujian hipotesis, data terlebih dahulu dianalisis menggunakan:
- Statistik deskriptif
- Visualisasi data (Histogram dan QQ Plot)
- Uji normalitas Kolmogorov-Smirnov

Analisis dilakukan menggunakan bahasa pemrograman **Python** pada platform **Google Colab**.

---

## Dataset
Dataset yang digunakan:
- **Student Study Performance Dataset**

Fokus penelitian:
- Kolom: `math_score`
- Kelompok: `group C`
- Jumlah populasi Group C: 319 data
- Jumlah sampel penelitian: 100 data (random sampling)

---

## Metode Analisis

### 1. Statistik Deskriptif
Meliputi:
- Mean
- Median
- Standar deviasi
- Variansi
- Nilai minimum
- Nilai maksimum
- Quartile
- IQR
- Skewness
- Kurtosis

### 2. Visualisasi Data
- Histogram
- QQ Plot

### 3. Uji Normalitas
Menggunakan:
- Kolmogorov-Smirnov Test

### 4. Uji Hipotesis
Menggunakan:
- One Sample t-Test
- Two-tailed hypothesis
- Taraf signifikansi α = 0.05

---

## Hipotesis Penelitian

### Hipotesis Nol (H0)
μ = 65.5

### Hipotesis Alternatif (H1)
μ ≠ 65.5

---

## Hasil Analisis

### Statistik Deskriptif
| Statistik | Nilai |
|---|---|
| Jumlah Data | 100 |
| Mean | 64.66 |
| Median | 66.50 |
| Standar Deviasi | 16.0480 |
| Minimum | 0 |
| Maksimum | 98 |

---

### Uji Normalitas Kolmogorov-Smirnov
| Keterangan | Nilai |
|---|---|
| D hitung | 0.0991 |
| D tabel | 0.1360 |
| p-value | 0.2624 |

Kesimpulan:
- Data berdistribusi normal

---

### One Sample t-Test
| Keterangan | Nilai |
|---|---|
| t hitung | -0.5234 |
| t tabel | 1.9842 |
| p-value | 0.6018 |

Kesimpulan:
- H0 diterima
- Tidak terdapat perbedaan signifikan antara rata-rata nilai matematika siswa Group C dengan nilai hipotesis 65.5

---

## Library Python yang Digunakan

```python
pandas
numpy
matplotlib
seaborn
scipy
statsmodels
