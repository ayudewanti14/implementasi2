# implementasi2
Implementasi HPC: Simulasi Evakuasi
Deskripsi
Notebook ini merupakan implementasi sederhana yang terinspirasi dari materi presentasi “Bridging Global Infrastructure to Address Local Challenges in High Performance Computing (HPC)” oleh Dr. Warawan dari Thammasat University.

Materi presentasi membahas bagaimana High Performance Computing (HPC) dapat dimanfaatkan untuk membantu menyelesaikan berbagai tantangan lokal, seperti prediksi banjir, pemetaan pertanian, penelitian penyakit, prakiraan cuaca dan PM2.5, pemodelan energi, simulasi evakuasi, serta penentuan rute kendaraan listrik.

Notebook ini mengambil contoh simulasi evakuasi untuk memperlihatkan konsep simulasi komputasi dan perbandingan eksekusi serial dengan eksekusi paralel.
Catatan: Notebook ini adalah contoh pembelajaran dengan peta dan data sintetis. Ini bukan sistem evakuasi nyata, bukan model yang tervalidasi untuk pengambilan keputusan darurat, dan bukan kode asli dari penelitian atau presentasi tersebut.

Tujuan
- Memahami contoh penerapan komputasi untuk masalah lokal.
- Membuat simulasi sederhana pergerakan menuju zona aman.
- Membandingkan hasil dan waktu eksekusi beberapa skenario.
- Mengenal konsep eksekusi serial dan paralel menggunakan Python.
Isi Notebook
Notebook Implementasi_HPC_Simulasi_Evakuasi.ipynb mencakup:
1. Penjelasan masalah dan asumsi simulasi.
2. Pembuatan peta grid sintetis yang berisi jalur, penghalang, titik awal, dan zona aman.
3. Simulasi pergerakan menuju zona aman.
4. Pengujian beberapa skenario dengan posisi awal yang berbeda.
5. Perbandingan eksekusi serial dan paralel menggunakan ProcessPoolExecutor.
6. Visualisasi hasil simulasi, tingkat keberhasilan, waktu eksekusi, dan perbandingan performa.
Teknologi yang Digunakan
- Python 3
- NumPy untuk pengolahan data numerik.
- Matplotlib untuk visualisasi peta dan hasil.
- concurrent.futures / ProcessPoolExecutor untuk contoh pemrosesan paralel.
- Google Colab sebagai lingkungan eksekusi yang direkomendasikan.
Cara Menjalankan di Google Colab
1. Unduh file Implementasi_HPC_Simulasi_Evakuasi.ipynb.
2. Buka Google Colab.
3. Pilih File → Upload notebook.
4. Unggah file notebook yang sudah diunduh.
5. Jalankan sel secara berurutan menggunakan tombol Run atau menu Runtime → Run all.
6. Amati peta simulasi, hasil setiap skenario, grafik tingkat keberhasilan, serta perbandingan waktu eksekusi serial dan paralel.
Jika proses paralel tidak berjalan pada lingkungan tertentu, ikuti pesan yang ditampilkan notebook dan gunakan hasil atau jalur cadangan yang disediakan di dalam kode.
Cara Kerja Singkat
1. Notebook membentuk lingkungan berbasis grid dengan beberapa penghalang dan satu zona aman.
2. Sejumlah agen simulasi ditempatkan pada posisi awal.
3. Agen bergerak berdasarkan aturan sederhana untuk mendekati zona aman.
4. Simulasi diulang pada beberapa skenario.
5. Waktu komputasi serial dan paralel diukur untuk memperkenalkan perbandingan performa.
Hasil simulasi bergantung pada parameter dan data sintetis yang digunakan. Perbandingan waktu juga dapat dipengaruhi oleh jumlah skenario, overhead proses paralel, serta keterbatasan sumber daya lingkungan Colab.
Batasan
- Peta, posisi, dan kondisi simulasi dibuat secara sintetis, bukan berasal dari data lapangan.
- Aturan gerak agen disederhanakan dan tidak mewakili perilaku manusia secara lengkap.
- Hasil tidak dapat digunakan sebagai panduan evakuasi nyata.
- Eksekusi paralel tidak selalu lebih cepat daripada serial, terutama untuk pekerjaan kecil karena adanya overhead.
- Notebook ini mendemonstrasikan konsep dasar, bukan implementasi penuh infrastruktur HPC seperti klaster komputasi.
Pengembangan Selanjutnya
Implementasi dapat dikembangkan dengan:
- Menggunakan peta wilayah dan jalur evakuasi berdasarkan data nyata yang telah diverifikasi.
- Menambahkan kepadatan penduduk, kapasitas jalur, dan kondisi jalan.
- Membandingkan beberapa algoritma pencarian rute.
- Menguji jumlah skenario yang lebih besar untuk melihat dampak paralelisasi.
- Menambahkan validasi dan evaluasi dengan data lapangan sebelum digunakan untuk tujuan praktis.
Referensi Materi
- Presentasi: “Bridging Global Infrastructure to Address Local Challenges in High Performance Computing (HPC)”, oleh Dr. Warawan, Thammasat University.
- Implementasi ini dibuat sebagai contoh pembelajaran berdasarkan tema yang dibahas dalam materi tersebut.
Lisensi dan Penggunaan
Notebook ini ditujukan untuk pembelajaran dan eksperimen akademik. Jika digunakan atau dikembangkan kembali, sertakan keterangan sumber inspirasi dan jelaskan bahwa simulasi menggunakan data sintetis.
