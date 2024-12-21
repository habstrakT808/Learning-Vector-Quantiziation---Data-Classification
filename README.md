# Learning Vector Quantization (LVQ)

## Deskripsi
Proyek ini mengimplementasikan berbagai variasi algoritma Learning Vector Quantization (LVQ) untuk klasifikasi data:

1. **LVQ (Learning Vector Quantization)**: Algoritma dasar untuk memetakan data ke centroid.
2. **LVQ2**: Perluasan LVQ dengan pembaruan dua centroid terdekat berdasarkan rasio jarak.
3. **LVQ2.1**: Peningkatan LVQ2 dengan pengaruh parameter epsilon untuk pembaruan yang lebih adaptif.

Proyek ini menggunakan dataset buatan untuk eksperimen klasifikasi, dan mencakup visualisasi hasil model untuk mempermudah analisis performa.

## Implementasi
File kode Python mencakup fungsi-fungsi berikut:

### 1. Training Model
- `lvq_fit(train, target, lrate, b, max_epoch)`
- `lvq2_fit(train, target, lrate, b, max_epoch, epsilon)`
- `lvq21_fit(train, target, lrate, b, max_epoch, epsilon)`

### 2. Testing Model
- `lvq_predict(X, model)`
- `calc_accuracy(a, b)`

### 3. Visualisasi
Menggunakan matplotlib untuk memvisualisasikan:
- Data pelatihan
- Centroid (prototipe model)
- Hasil prediksi data pengujian

## Parameter Model
- **Learning rate**: 0.5
- **Penurunan learning rate**: 0.8
- **Epoch maksimum**: 100
- **Epsilon**: 0.3

## Langkah Eksperimen
1. **Data Preparation**: Dataset dibuat menggunakan `make_classification` dari scikit-learn dengan 4 kelas.
2. **Training**: Masing-masing algoritma dilatih menggunakan data pelatihan.
3. **Testing**: Model diuji pada data pengujian.
4. **Visualisasi**: Hasil model divisualisasikan untuk analisis.

## Hasil dan Analisis
| Algoritma | Akurasi |
|-----------|---------|
| LVQ       | 80%     |
| LVQ2      | 65%     |
| LVQ2.1    | 85%     |

### Analisis:
- **LVQ**: Memberikan hasil yang cukup baik namun kurang fleksibel untuk data kompleks.
- **LVQ2**: Menunjukkan akurasi lebih rendah karena sensitivitas terhadap parameter epsilon.
- **LVQ2.1**: Memberikan hasil terbaik dengan akurasi 85% berkat mekanisme pembaruan yang lebih adaptif.

## Dependensi
- Python 3.x
- Numpy
- Pandas
- Matplotlib
- Scikit-learn

## Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone https://github.com/habstrakT808/Learning-Vector-Quantiziation---Data-Classification.git
   ```
2. Install dependensi:
   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```
3. Jalankan script:
   ```bash
   python lvq.py
   ```

## Kontak
Untuk pertanyaan atau masukan, silakan hubungi:
- **Email**: [hafiyan@example.com](mailto:hafiyan@example.com)
- **GitHub**: [github.com/hafiyan](https://github.com/habstrakT808)
