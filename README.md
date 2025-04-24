Klasifikasi Kelayakan Kredit Komputer  
Nama: Viqriza Ahmad Vahira  
NIM: 1227050132  
Kelas: C  

 Deskripsi Proyek  
Proyek ini membangun sebuah model klasifikasi untuk memprediksi apakah seorang individu pantas atau tidak pantas menerima fasilitas kredit komputer. Data yang dipakai merupakan dataset dummy yang mencakup atribut demografis dan finansial.


 Dataset  
File CSV berisi kolomkolom berikut:  
 Age: Kategori umur (muda, tengah, tua)  
 Income: Tingkat pendapatan (rendah, sedang, tinggi)  
 Student: Status mahasiswa (ya/tidak)  
 Credit_Rating: Status kredit (fair/excellent)  
 Buys_Computer: Target klasifikasi (yes/no)  



 Metodologi  
1. Persiapan Lingkungan  
    Mengimpor pustaka Python: `pandas`, `scikitlearn`, `matplotlib`, dll.
2. Eksplorasi Data  
    Memeriksa lima baris pertama, tipe data, dan ringkasan statistik.  
    Visualisasi distribusi masing‑masing variabel dengan diagram batang.
3. Prapemrosesan  
    One‑hot encoding untuk semua fitur kategorikal.  
    Normalisasi/standardisasi fitur numerik (jika diperlukan).
4. Pembagian Data  
    Memisahkan data menjadi set pelatihan (70%) dan pengujian (30%) dengan stratifikasi target untuk menjaga proporsi kelas.
5. Pembuatan Model  
    Naive Bayes (GaussianNB)  
      Memanfaatkan asumsi distribusi Gaussian untuk menghitung probabilitas kelas.  
      Melatih model pada data pelatihan.
6. Evaluasi  
    Menghitung akurasi, precision, recall, dan F1score.  
    Menyajikan confusion matrix dalam bentuk heatmap.  
    Mengukur area di bawah kurva ROC (AUC).
7. Visualisasi  
    Menampilkan confusion matrix sebagai heatmap.  
    Menggambar kurva ROC.  
8. Kesimpulan  
    Model GaussianNB mencapai akurasi sekitar 80% pada data dummy ini.  
    Sebagai baseline, model ini cukup baik, namun dapat ditingkatkan lagi lewat teknik seperti pengoptimalan hyperparameter, ensemble, ataupun metode klasifikasi lain.

 Hasil Ringkas  
 Akurasi: ~0.80  
 AUC‑ROC: ~0.85  
 Precision / Recall / F1‑score per kelas:  
   Layak (Yes): precision ~0.78, recall ~0.82  
   Tidak Layak (No): precision ~0.81, recall ~0.79  


