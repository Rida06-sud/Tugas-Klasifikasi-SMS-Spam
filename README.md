# Tugas-Klasifikasi-SMS-Spam

# Later belakang dan Permasalahan
Studi Kasus : filter SMS Spam

SMS spam adalah pesan teks yang tidak diminta, biasanya berisi iklan , penipunan berhadiah, tautan berbahya (phishing) atau ajakan menghubungi nomer berbayar. di indonesia bentuk umumnya adaah SMS "Selamat Anda menang undian" atau pinjaman online ilegal.

Permasalahan yang dihadapi:

jumlah pesan sangat besar shingga tidak mungkin disaring secara manual

aturan sederhana misalnya blokir kata "gratis" mudah dikelabuhi dan sering salah blokir pesan yng sah

dua jenis kesalahan punya dampak berbeda spam lolos menunggu dan berisko penipuan sedangkan pesan yang sah malah diblokir sehingga pengguna kehilangan pesan penting seperi kode OTP

# Metode Klasifikasi yang Digunakan
Teks tidak bisa langsung diproses model, sehingga diubah menjadi angka dengan TF-IDF (Term Frequency - Inverse Document Frequency), yaitu pembobotan yang memberi nilai tinggi pada kata yang sering muncul di sebuah pesan tetapi jarang di pesan lain.

# Dataset
SMS Spam Collection (Almeida, Hidalgo & Yamakami, 2011), tersedia di UCI Machine Learning Repository dan Kaggle.

Kolom v1: label (ham atau spam).

Kolom v2: isi pesan SMS (bahasa Inggris).

Tiga kolom Unnamed hanya berisi sisa data kosong dan akan dibuang.

# REFERENSI

Almeida, T. & Gómez Hidalgo, J. (2011). SMS Spam Collection [Dataset]. UCI Machine Learning Repository. https://archive.ics.uci.edu/dataset/228/sms+spam+collection KDnuggets (2011). New dataset released: SMS Spam Collection v.1. https://www.kdnuggets.com/2011/06/sms-spam-collection-data.html

Manning, C. D., Raghavan, P., & Schütze, H. (2008). Introduction to Information Retrieval. Cambridge University Press. https://nlp.stanford.edu/IR-book/html/htmledition/naive-bayes-text-classification-1.html

Cortes, C., & Vapnik, V. (1995). Support-vector networks. Machine Learning, 20(3), 273-297.

Fan, R.-E., et al. (2008). LIBLINEAR: A library for large linear classification. Journal of Machine Learning Research, 9, 1871-1874.

Spärck Jones, K. (1972). A statistical interpretation of term specificity and its application in retrieval. Journal of Documentation, 28(1), 11-21.
