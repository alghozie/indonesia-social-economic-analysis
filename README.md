# Analisis Realisasi TKDD & Faktor-Faktor yang Mempengaruhi IPM Provinsi di Indonesia (2023)

**Kompetisi:**  
*TECHFEST 2025 — Data Analytics Competition*  
**Tim:** breztech  

---

## Deskripsi Proyek

Proyek ini bertujuan untuk **menganalisis hubungan antara realisasi Transfer ke Daerah dan Dana Desa (TKDD)** dengan **Indeks Pembangunan Manusia (IPM)** di seluruh provinsi di Indonesia tahun 2023.  
Analisis dilakukan untuk mengidentifikasi seberapa besar efektivitas realisasi anggaran publik dalam meningkatkan kualitas pembangunan manusia di berbagai daerah.

Melalui analisis dan visualisasi berbasis data, proyek ini diharapkan dapat:
-  Menggambarkan distribusi realisasi TKDD di setiap provinsi.  
-  Menemukan hubungan antara anggaran, kemiskinan, dan IPM.  
-  Memberikan rekomendasi kebijakan berbasis data untuk mendukung pemerataan pembangunan.  
-  Mendukung upaya Indonesia menuju pembangunan berkelanjutan dan merata.

---

## Teknologi & Library yang Digunakan

| Komponen | Teknologi |
|-----------|------------|
| **Bahasa Pemrograman** | Python 3 |
| **Analisis Data** | Pandas, NumPy |
| **Visualisasi Data** | Matplotlib, Seaborn |
| **Analisis Statistik** | Scikit-learn (Regresi Linear, Korelasi Pearson) |
| **Lingkungan Pengembangan** | Google Colab |
| **Sumber Data** | Dataset Lomba Data Analytics TECHFEST 2025 (BPS, DJPK, dan sumber publik) |

---

## Langkah Menjalankan Proyek

1. **Buka file notebook di Google Colab**
   - Upload file `TECHFEST.ipynb` dan `Dataset Lomba Data Analytics TECHFEST 2025.xlsx` ke Google Drive.  
   - Pastikan path dataset sudah benar di dalam notebook.

2. **Mount Google Drive**
   ```python
   from google.colab import drive
   drive.mount('/content/drive')

3. **Atur Path Dataset**
   DATA_PATH = '/content/drive/MyDrive/TECHFEST/Dataset Lomba Data Analytics TECHFEST 2025.xlsx'

4. **Jalankan seluruh sel**
   Notebook akan melakukan pembersihan data, analisis statistik, dan menghasilkan berbagai visualisasi otomatis.

| No | Visualisasi                                              | Deskripsi                                                                |
| -- | -------------------------------------------------------- | ------------------------------------------------------------------------ |
| 1  | **Distribusi Persentase Realisasi TKDD per Provinsi**    | Menunjukkan kategori `<90%`, `90–100%`, `>100%`.                         |
| 2  | **Scatter Plot: Pagu vs Realisasi TKDD**                 | Menggambarkan efektivitas penyerapan anggaran tiap provinsi.             |
| 3  | **Top 10 dan Bottom 10 Provinsi**                        | Mengidentifikasi provinsi dengan realisasi tertinggi & terendah.         |
| 4  | **Heatmap Korelasi Variabel Ekonomi & Sosial**           | Menunjukkan hubungan antara TKDD, PDRB, kemiskinan, dan IPM.             |
| 5  | **Realisasi vs Persentase Kemiskinan**                   | Menganalisis dampak penyerapan anggaran terhadap kemiskinan.             |
| 6  | **Realisasi vs IPM**                                     | Melihat seberapa kuat realisasi TKDD berpengaruh terhadap IPM.           |
| 7  | **IPM vs APBN Per Kapita (log scale)**                   | Menunjukkan titik jenuh peningkatan IPM berdasarkan anggaran.            |
| 8  | **Triple Trouble Map**                                   | Menyoroti provinsi dengan IPM rendah, kemiskinan tinggi, dan APBN besar. |

## Hasil & Insight Utama
1. Mayoritas provinsi sudah menyalurkan realisasi TKDD di atas 90%.
2. Namun, realisasi tinggi tidak selalu berarti IPM tinggi — efektivitas lebih penting daripada nominal.
3. Korelasi kuat antara pagu_tkdd dan realisasi_tkdd.
4. Korelasi negatif antara persentase kemiskinan dan IPM.
5. Korelasi positif moderat antara PDRB per kapita dan IPM.
6. Beberapa provinsi seperti Gorontalo, NTT, Papua Barat, dan Sulawesi Tengah termasuk kategori Triple Trouble (IPM rendah + kemiskinan tinggi + anggaran besar).

## Rekomendasi Kebijakan
1. Fokus pada efektivitas penyerapan anggaran, bukan sekadar jumlah dana.
2. Terapkan evaluasi berbasis kinerja pada program TKDD.
3. Replikasi strategi provinsi ber-IPM tinggi dengan realisasi efisien.
4. Berikan pendampingan teknis dan fiskal untuk daerah Triple Trouble.
5. Gunakan dashboard real-time monitoring TKDD untuk meningkatkan transparansi.
