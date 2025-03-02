# 📊 Analisis Sentimen Ulasan Produk

## 📝 Deskripsi Proyek
Proyek ini bertujuan untuk melakukan **analisis sentimen** pada ulasan produk menggunakan dua model berbeda: **VADER** dan **RoBERTa**. Dengan membandingkan hasil dari kedua model ini, kita dapat menentukan mana yang lebih akurat dalam mengklasifikasikan sentimen dari teks ulasan pelanggan.

## 📂 Dataset
Dataset yang digunakan berasal dari **Amazon Fine Food Reviews**, yang berisi lebih dari **500.000 ulasan** pelanggan terhadap berbagai produk makanan di Amazon. Dataset ini mencakup beberapa kolom utama:

| Kolom | Deskripsi |
|--------|------------|
| `Id` | ID unik untuk setiap ulasan |
| `ProductId` | ID produk yang diulas |
| `UserId` | ID pengguna yang memberikan ulasan |
| `ProfileName` | Nama profil pengguna |
| `HelpfulnessNumerator` | Jumlah suara "membantu" untuk ulasan |
| `HelpfulnessDenominator` | Total suara untuk ulasan |
| `Score` | Skor (1-5) yang diberikan oleh pengguna |
| `Time` | Waktu ulasan diberikan dalam format timestamp UNIX |
| `Summary` | Ringkasan singkat dari ulasan |
| `Text` | Isi lengkap dari ulasan |

## 🛠️ Metode Analisis
Analisis sentimen dilakukan menggunakan dua pendekatan utama:
1. **VADER (Valence Aware Dictionary and sEntiment Reasoner)**
   - Cocok untuk teks pendek dan berbasis kamus.
   - Menghasilkan skor **negatif (`vader_neg`), netral (`vader_neu`), positif (`vader_pos`), dan compound (`vader_compound`)**.
2. **RoBERTa (Robustly optimized BERT approach)**
   - Model deep learning berbasis transformer.
   - Menghasilkan skor **negatif (`roberta_neg`), netral (`roberta_neu`), dan positif (`roberta_pos`)**.


## 🔍 Kesimpulan
- **VADER** lebih baik dalam menangkap sentimen eksplisit dengan kata-kata sederhana.
- **RoBERTa** lebih baik dalam menangkap konteks yang lebih kompleks dan nuansa dalam teks panjang.
