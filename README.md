Proyek ini merupakan analisis data untuk mengidentifikasi faktor-faktor yang memengaruhi pembatalan pemesanan hotel. Masalah pembatalan reservasi menjadi perhatian serius dalam industri perhotelan karena dapat berdampak langsung pada pendapatan dan efisiensi operasional hotel. Oleh karena itu, melalui pendekatan data science, proyek ini bertujuan membantu pihak manajemen hotel memahami pola pembatalan dan membuat keputusan yang lebih tepat. Dataset yang digunakan berasal dari situs [Kaggle](https://www.kaggle.com/), berisi 119.390 data reservasi hotel dengan berbagai informasi, seperti jenis hotel, status pembatalan (`is_canceled`), waktu tunggu sebelum check-in (`lead_time`), tipe pelanggan (`market_segment`), status pengunjung ulang (`is_repeated_guest`), status deposit, perubahan pemesanan (`booking_changes`), tarif harian (`adr`), dan banyak fitur lainnya.

Tujuan utama dari proyek ini adalah:
* Mengetahui pola dan variabel yang paling berpengaruh terhadap pembatalan.
* Membangun model prediksi untuk mengklasifikasikan apakah reservasi akan dibatalkan atau tidak.
* Memberikan insight yang dapat digunakan untuk mendukung kebijakan promosi, sistem refund, dan strategi pemasaran.

Langkah-langkah yang dilakukan:
1. Exploratory Data Analysis (EDA)
   Menganalisis distribusi dan korelasi data, serta menemukan pola penting seperti pengaruh `lead_time`, `previous_cancellations`, dan `deposit_type`.
2. Data Preprocessing
   Melakukan encoding data kategorikal menggunakan Label Encoder, menghapus/memperbaiki nilai kosong dan outlier, serta menormalkan data numerik menggunakan MinMax Scaler. Data yang tidak seimbang juga diseimbangkan agar model tidak bias terhadap mayoritas kelas.
3. Modeling
   Membangun dan mengevaluasi model klasifikasi menggunakan beberapa algoritma, dan memilih model terbaik berdasarkan akurasi dan stabilitasnya terhadap data.

Insight yang ditemukan:
* Semakin lama waktu tunggu sebelum check-in (`lead_time`), semakin tinggi kemungkinan pembatalan.
* Pelanggan yang pernah membatalkan sebelumnya lebih cenderung membatalkan lagi.
* Pelanggan berulang (`repeated_guest`) cenderung lebih setia dan jarang membatalkan.
* Tidak adanya deposit menunjukkan risiko pembatalan lebih tinggi.
* Tarif tinggi (`adr`) juga berkaitan dengan tingkat pembatalan yang lebih besar.

Teknologi yang digunakan:

* Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
* Jupyter Notebook
* Label Encoding dan MinMax Scaler
* Algoritma klasifikasi (seperti Decision Tree, Random Forest, dsb.)

Anggota Kelompok:

* M Agil Mubarok (2012210012)
* Afica Marsha Nurcahaya (2012310002)
* Ferindriakarina Lintang Helsadamara (2012310007)
* Eis Aghisni (2012310701)

Proyek ini dikembangkan untuk keperluan pembelajaran dalam bidang data science dan dapat menjadi dasar atau referensi untuk pengembangan lebih lanjut, khususnya dalam industri perhotelan.
