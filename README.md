Analisis Penjualan Video Game Global
Selamat datang di repositori analisis penjualan video game global! Proyek ini menggali dataset populer yang berisi informasi penjualan lebih dari 16.000 video game dari tahun 1980 hingga 2020. Tujuan utama analisis ini adalah untuk mengungkap tren dan wawasan menarik dari industri video game selama empat dekade.

📊 Dataset
Dataset yang digunakan dalam analisis ini adalah "Video Game Sales" yang bersumber dari Kaggle. Dataset ini mencakup informasi krusial tentang setiap game, termasuk:

Platform: Konsol atau platform tempat game dirilis (misalnya, PS4, PC, Wii).

Tahun Rilis: Tahun saat game pertama kali diluncurkan.

Genre: Jenis atau kategori game (misalnya, Action, Sports, RPG).

Publisher: Perusahaan yang menerbitkan game.

Penjualan Regional: Data penjualan dalam jutaan unit untuk Amerika Utara (NA), Eropa (EU), Jepang (JP), dan wilayah lainnya (Other).

Penjualan Global: Total penjualan di seluruh dunia.

⚙️ Proses Analisis
Analisis ini dilakukan dalam beberapa tahap utama untuk memastikan hasil yang akurat dan mendalam.

Pembersihan Data (Data Cleaning):

Mengidentifikasi dan menghapus baris data dengan nilai yang hilang pada kolom Year dan Publisher untuk menjaga integritas dataset.

Memperbaiki tipe data pada kolom Year dari float (desimal) menjadi integer (bilangan bulat).

Rekayasa Fitur (Feature Engineering):

Membuat kolom baru Platform_Family untuk mengelompokkan platform individual (misalnya, 'PS2', 'PS3', 'PS4') ke dalam keluarga konsol yang lebih besar (misalnya, 'PlayStation'). Ini menyederhanakan analisis tren antar-merek.

Analisis Data Eksploratif (Exploratory Data Analysis - EDA):

Melakukan analisis untuk menjawab pertanyaan-pertanyaan kunci bisnis dan industri.

Menggunakan visualisasi data seperti grafik batang, diagram garis, dan heatmap untuk menyajikan temuan secara efektif.

💡 Temuan Utama (Key Insights)
Beberapa wawasan paling menarik yang ditemukan dari analisis ini adalah:

Dominasi Genre Aksi: Genre Action merupakan genre yang paling banyak dirilis dan juga menghasilkan total penjualan global tertinggi.

Puncak Industri Game: Puncak perilisan dan penjualan game terjadi pada periode 2008-2011, terutama didorong oleh kesuksesan platform Nintendo Wii dan DS.

Raja Penjualan: Wii Sports menjadi game terlaris sepanjang masa, sebagian besar karena dibundel dengan konsol Nintendo Wii.

Perbedaan Pasar Regional: Terdapat perbedaan selera pasar yang signifikan antara Barat dan Timur. Genre Action dan Shooter sangat dominan di Amerika Utara, sementara genre Role-Playing (RPG) memiliki pangsa pasar yang jauh lebih kuat di Jepang.

Publisher Raksasa: Nintendo tidak hanya menjadi publisher dengan total penjualan tertinggi tetapi juga secara konsisten merilis banyak judul paling sukses dalam sejarah.

🛠️ Teknologi yang Digunakan
Python: Bahasa pemrograman utama yang digunakan untuk analisis.

Pandas: Untuk manipulasi dan pembersihan data.

Matplotlib & Seaborn: Untuk pembuatan visualisasi data.

Jupyter Notebook: Lingkungan kerja interaktif untuk menjalankan analisis.

🚀 Cara Menjalankan Proyek
Untuk menjalankan analisis ini di mesin lokal Anda, ikuti langkah-langkah berikut:

Clone repositori ini:

Bash

git clone [URL-repositori-Anda]
Pindah ke direktori proyek:

Bash

cd [nama-folder-proyek]
Instal dependensi yang dibutuhkan:

Bash

pip install pandas matplotlib seaborn jupyterlab
Jalankan Jupyter Notebook:

Bash

jupyter lab
Buka file .ipynb untuk melihat dan menjalankan kode analisis secara langsung.







rayhankwar...bal_kaggle
GitHub

Buatkan Deskripsi hasil analisis dari ipynb saya jelaskan detail sehingga user membaca mudah mengerti



Show thinking
Tentu, berdasarkan analisis dari file Jupyter Notebook Anda, berikut adalah deskripsi detail dan mudah dimengerti yang bisa langsung Anda gunakan untuk file README di GitHub Anda. Deskripsi ini menjelaskan setiap langkah analisis dan temuan utamanya.

Analisis Penjualan Video Game Global
Ini adalah proyek analisis data untuk menggali wawasan dari dataset Penjualan Video Game yang populer dari Kaggle. Tujuan dari analisis ini adalah untuk memahami tren industri video game selama beberapa dekade, mengidentifikasi genre dan platform paling sukses, serta melihat perbedaan selera pasar di berbagai wilayah.

📊 Dataset
Dataset yang digunakan berisi informasi lebih dari 16.000 video game, mencakup data-data penting seperti:

Nama Game, Platform, Tahun Rilis, Genre, dan Publisher.

Data Penjualan (dalam jutaan unit) untuk wilayah Amerika Utara (NA), Eropa (EU), Jepang (JP), wilayah lainnya, dan total penjualan global.

⚙️ Proses Analisis Data
Analisis ini dilakukan melalui beberapa tahapan sistematis untuk memastikan data akurat dan wawasan yang dihasilkan relevan.

1. Pembersihan Data (Data Cleaning)
Langkah pertama adalah memastikan kualitas data. Berdasarkan pemeriksaan awal (df.info()), ditemukan ada beberapa data yang kosong pada kolom Year dan Publisher. Baris-baris data yang tidak lengkap ini kemudian dihapus untuk menjaga keakuratan analisis. Setelah pembersihan, dataset menjadi lebih solid dengan 16.291 entri data yang siap untuk dianalisis lebih lanjut. Pemeriksaan duplikasi juga menunjukkan bahwa tidak ada data yang ganda di dalam dataset.

2. Analisis Eksplorasi Data (EDA)
Setelah data bersih, dilakukan eksplorasi untuk menemukan pola dan tren menarik melalui beberapa analisis berikut:

Distribusi Game Berdasarkan Genre
Temuan: Genre Action adalah yang paling banyak diproduksi, diikuti oleh Sports dan Misc (Miscellaneous). Ini menunjukkan bahwa pasar dibanjiri oleh game-game aksi.

Visualisasi: Grafik batang (Bar Chart) digunakan untuk menunjukkan perbandingan jumlah game dari setiap genre secara visual.

Distribusi Penjualan Global
Temuan: Mayoritas besar game memiliki penjualan global di bawah 5 juta unit. Namun, ada beberapa game yang menjadi outlier (pencilan) dengan penjualan sangat tinggi, yang menandakan adanya judul-judul blockbuster yang mendominasi pasar.

Visualisasi: Histogram dan Box Plot digunakan untuk melihat sebaran data penjualan ini.

Rata-Rata Penjualan per Genre
Temuan: Meskipun genre Action paling banyak jumlahnya, genre Platform memiliki rata-rata penjualan global tertinggi, diikuti oleh Shooter. Ini menandakan bahwa meskipun lebih sedikit diproduksi, game platform cenderung lebih sukses secara komersial per judulnya.

Visualisasi: Grafik batang digunakan untuk membandingkan rata-rata penjualan masing-masing genre.

Game Terlaris Sepanjang Masa
Temuan: Wii Sports menempati posisi puncak sebagai game dengan penjualan global tertinggi sepanjang masa, dengan angka penjualan yang jauh melampaui game lainnya di daftar 10 besar. Kesuksesan besar ini salah satunya disebabkan karena game ini dibundel dengan konsol Nintendo Wii.

Visualisasi: Grafik batang horizontal digunakan untuk menampilkan peringkat 10 game teratas.

Tren Penjualan Global dari Tahun ke Tahun
Temuan: Industri video game mengalami puncak penjualan pada periode 2008-2009. Setelah itu, terlihat adanya tren penurunan penjualan secara keseluruhan. Puncak ini bertepatan dengan era keemasan konsol seperti Nintendo Wii dan DS.

Visualisasi: Grafik garis (Line Plot) digunakan untuk menggambarkan tren total penjualan game setiap tahunnya.

Analisis Pasar Regional: Amerika Utara vs. Jepang
Temuan: Terdapat perbedaan selera pasar yang sangat jelas antara Amerika Utara dan Jepang.

Di Amerika Utara, genre Action dan Shooter sangat mendominasi pasar.

Sementara itu, di Jepang, genre Role-Playing (RPG) adalah yang paling populer, menunjukkan preferensi pasar yang sangat berbeda.

Visualisasi: Dua grafik batang yang disajikan berdampingan secara efektif menunjukkan kontras preferensi genre di kedua wilayah ini.

💡 Kesimpulan
Dari analisis ini, dapat disimpulkan bahwa meskipun genre Aksi menjadi yang paling umum, genre Platform justru lebih menguntungkan secara rata-rata. Puncak industri terjadi pada akhir tahun 2000-an, dan ada perbedaan signifikan dalam preferensi game antar wilayah, di mana pasar Jepang memiliki karakteristik unik yang didominasi oleh RPG.
