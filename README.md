# Klasifikasi Sentimen Ulasan Restoran pada Google Maps Menggunakan Algoritma Naive Bayes

Tugas Besar Kecerdasan Buatan — Telkom University, Tahun Akademik 2026/2027

## Anggota Kelompok
| Nama | NIM | Kontribusi |
|---|---|---|
| Qadlizaky Ermansyah | 101032400152 | Data dan pembersihan teks |
| Bagus Suryansyah Dharmawinata | 101032400046 | Implementasi Naive Bayes dari nol |
| Muhammad Rahmad Dany | 101032400053 | Evaluasi dan verifikasi dengan scikit-learn |
| Agung Prayasa NR | 101032400182 | Perbaikan model (cross-validation dan prior seimbang) |

## Deskripsi
Program ini mengklasifikasikan ulasan restoran di Google Maps menjadi **positif** atau **negatif** menggunakan algoritma **Naive Bayes** yang diimplementasikan dari nol (dengan Laplace smoothing dan logaritma), lalu diverifikasi dengan `MultinomialNB` dari scikit-learn.

## Dataset
[Google Maps Restaurant Reviews (Kaggle)](https://www.kaggle.com/datasets/denizbilginn/google-maps-restaurant-reviews), berisi 1100 ulasan. Ulasan bintang 4–5 dilabeli positif, bintang 1–2 negatif, dan bintang 3 dibuang, sehingga tersisa 928 ulasan.

## Hasil
| Model | Akurasi | Recall negatif | F1 macro |
|---|---|---|---|
| Naive Bayes (prior sesuai data) | 87,10% | 0,20 | 0,63 |
| **Naive Bayes (prior seimbang)** | **88,17%** | **0,47** | **0,75** |

## Cara Menjalankan
1. Download dataset dari link Kaggle di atas, lalu ambil file `reviews.csv`.
2. Buka `NaiveBayes_Restoran.ipynb` di Google Colab (bisa lewat tombol **Open in Colab** di notebook).
3. Upload `reviews.csv` lewat ikon folder di sidebar kiri.
4. Klik **Runtime → Jalankan semua**.
