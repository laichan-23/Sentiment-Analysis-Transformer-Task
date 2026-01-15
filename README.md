# Proyek Analisis Sentimen - Model Transformer (BERT)

Tugas ini merupakan implementasi pelabelan sentimen otomatis menggunakan arsitektur Deep Learning **Transformer**. Proyek ini mencakup proses pengambilan data, pembersihan teks (preprocessing), pelatihan model (fine-tuning), hingga pengujian pada data tanpa label.

## 👥 Anggota Kelompok
**Kelas: TI-KIP-P3**
1. **Laelatul Badriyah** - NIM: 41236732
2. **Putri Pirna** - NIM: 41236773

---

## 🚀 Alur Kerja Teknis (Workflow)

Proyek ini mengikuti tahapan standar pemrosesan bahasa alami (NLP):

1. **Data Collection**: 
   - Mengumpulkan dataset sentimen.
   - **Data Pelatihan**: 300 kalimat (100 Positif, 100 Negatif, 100 Netral).
   - **Data Pengujian**: 400 kalimat tanpa label.
2. **Preprocessing**: 
   - Membersihkan teks dari simbol/tanda baca.
   - Mengubah teks menjadi huruf kecil (case folding).
3. **Tokenization**: 
   - Mengonversi teks menjadi token/angka agar dapat dipahami oleh arsitektur Transformer.
4. **Fine-Tuning**: 
   - Melatih model Pre-trained **BERT (bert-base-uncased)** menggunakan 300 data pelatihan untuk mengenali pola sentimen.
5. **Inference (Labeling)**: 
   - Menjalankan model yang telah dilatih untuk memberikan label otomatis (Positif/Negatif/Netral) pada 400 data pengujian.
6. **Output**: 
   - Menyimpan hasil prediksi ke dalam file CSV baru yang siap digunakan.

---

## 📊 Hasil Visualisasi

(<img width="699" height="552" alt="image" src="https://github.com/user-attachments/assets/8e6fd671-2f72-42d5-b339-cbbd62b834e7" />)


*Grafik di atas menunjukkan distribusi hasil pelabelan otomatis model terhadap 400 data pengujian.*

---

## 📁 Struktur File
- `Analisis_Sentimen_Transformer.ipynb`: Notebook berisi seluruh kode eksperimen.
- `train_final.csv`: Dataset pelatihan (300 data berlabel).
- `test_labeled_result.csv`: Dataset hasil pengujian (400 data hasil prediksi model).
- `README.md`: Dokumentasi proyek.

---

## 🛠️ Teknologi yang Digunakan
- Python
- Google Colab (GPU T4)
- Hugging Face Transformers Library
- PyTorch
- Pandas & Matplotlib
