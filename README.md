# machine_learnine_capstone3

# **Business Problem Understanding**

**Background**

Seiring dengan pertumbuhan industri perhotelan yang pesat, meningkatnya kompleksitas dalam manajemen pemesanan dan transaksi menjadi tantangan yang signifikan. Salah satu aspek krusial dalam hal ini adalah penanganan yang efektif terhadap transaksi yang awalnya dicatat sebagai gagal bayar.  Transaksi yang gagal bayar tidak hanya berdampak pada pendapatan hotel, tetapi juga memberikan pengalaman yang tidak memuaskan bagi tamu yang berusaha melakukan pemesanan. Tantangan utama yang dihadapi oleh hotel adalah bagaimana mengatasi ketidakakuratan dalam sistem yang dapat menyebabkan transaksi yang seharusnya gagal bayar diinterpretasikan sebagai berhasil bayar. Hal ini dapat terjadi karena berbagai alasan, termasuk kesalahan teknis, ketidaksesuaian data, atau bahkan faktor eksternal yang tidak terduga. Dalam banyak kasus, kesalahan ini dapat menimbulkan ketidaknyamanan operasional, potensi kehilangan pendapatan, dan pada akhirnya, merugikan kepuasan pelanggan.

**Problem Statement**

Masalah yang dihadapi adalah upaya untuk mengurangi jumlah pelanggan yang pada kenyataannya membatalkan pemesanan (pembayaran), tetapi dalam prediksi dianggap berhasil melakukan pemesanan (pembayaran). Kesalahan semacam ini dapat berdampak serius pada keseimbangan keuangan dan efisiensi operasional hotel.

0: Transkasi Completed

1: Transaction Canceled

**Goals**

Meningkatkan Akurasi Prediksi
- Mengembangkan model prediktif yang lebih akurat untuk mengidentifikasi pelanggan yang benar-benar melakukan pembatalan, tetapi pada awalnya diprediksi berhasil melakukan pemesanan.
Optimalkan Alokasi Sumber Daya
- Mengurangi kesalahan prediksi, diharapkan hotel dapat mengoptimalkan alokasi sumber daya, termasuk penjadwalan staf dan manajemen inventaris kamar, sehingga mengurangi dampak operasional dari pembatalan yang tidak terduga.
Minimalkan Kerugian Finansial
- Mengurangi jumlah pelanggan yang sebenarnya membatalkan pemesanan namun diprediksi berhasil dapat membantu hotel mengurangi kerugian finansial yang disebabkan oleh pelanggan yang tercatat sudah membayar namun sebenarnya belum melakukan pembayaran.

**Analytic Aprroach**

Akan dibangun model klasifikasi untuk memprediksi probabilitas pelanggan yang berhasil menyelesaikan transaksi sebagai pembatalan transaksi.

**Metric Evaluation**

False Negative (FN): Jumlah prediksi yang salah bahwa pelanggan berhasil melakukan transaksi namun actualnya membatalkan tansaksi. FN terjadi ketika model gagal mengidentifikasi pelanggan yang sebenarnya membatalkan transaksi. Jika jumlah FN tinggi, hal ini dapat mengakibatkan beberapa konsekuensi yang tidak diinginkan, seperti:

- Kekosongan Kamar yang Tidak Terduga: Jika pelanggan yang sebenarnya membatalkan diabaikan oleh model, hotel mungkin tidak mempersiapkan kamar tambahan atau menyediakan layanan yang sesuai, menyebabkan kekosongan kamar yang tidak terduga.
- Kerugian Finansial: Hotel mungkin telah menyiapkan sumber daya dan layanan untuk pelanggan yang pada akhirnya tidak datang, menyebabkan kerugian finansial yang dapat dihindari.
- Dampak Operasional: Kegagalan dalam mengantisipasi pembatalan dapat menyebabkan ketidakefisienan dalam pengelolaan operasional, seperti penjadwalan staf dan manajemen inventaris kamar.

Recall: Fokus diberikan pada meningkatkan kemampuan model untuk mendeteksi sebanyak mungkin kasus positif yang sebenarnya (pembatalan). Tujuannya adalah untuk meminimalkan jumlah FN, sehingga model dapat lebih baik mengidentifikasi pelanggan yang benar-benar membatalkan pemesanan.



