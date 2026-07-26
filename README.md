# Banking Performance Dashboard

## 📌 Project Type
Personal Project

## 📊 Overview
Project ini merupakan dashboard interaktif berbasis Microsoft Power BI yang dikembangkan untuk menganalisis performa operasional perbankan menggunakan dataset transaksi internal yang mensimulasikan aktivitas nasabah pada berbagai produk dan layanan keuangan.

Fokus utama dari project ini adalah mengolah data transaksi menjadi informasi yang terstruktur, konsisten, dan mudah dianalisis untuk mendukung monitoring operasional serta pengambilan keputusan strategis. Proses yang dilakukan mencakup data modeling, pembuatan calculated columns dan measures menggunakan DAX, serta visualisasi data untuk mengevaluasi aktivitas transaksi, segmentasi pelanggan, performa cabang, dan pendapatan berbasis biaya (fee-based revenue).

## 🎯 Objectives

- Menyajikan ringkasan performa transaksi melalui KPI utama, meliputi Total Transaction Value, Total Transactions, Active Customers, Average Transaction Amount, dan Total Fee Revenue.
- Memantau perkembangan nilai transaksi dan jumlah pelanggan aktif secara periodik untuk mengidentifikasi tren aktivitas perbankan.
- Mengevaluasi distribusi transaksi berdasarkan Product Category, Transaction Channel, dan Customer Segment.
- Menganalisis profil pelanggan berdasarkan Monthly Income, Credit Score, serta Customer Segment.
- Membandingkan performa cabang berdasarkan nilai transaksi, jumlah transaksi, pelanggan aktif, dan credit score.
- Mengidentifikasi pola perilaku transaksi pada setiap Credit Score Segment.
- Mengevaluasi sumber utama fee-based revenue berdasarkan Product Category, Customer Segment, Credit Score Segment, Transaction Type, dan Channel.
- Mengidentifikasi produk dan segmen pelanggan yang memberikan kontribusi terbesar terhadap pendapatan berbasis biaya.

## ⚙️ Data Processing

- Data cleaning untuk memastikan konsistensi dan kualitas data.
- Data transformation untuk menyesuaikan struktur data agar siap dianalisis.
- Data modeling menggunakan star schema untuk mendukung analisis multidimensi.
- Pembuatan calculated columns dan measures menggunakan DAX untuk menghasilkan KPI dan business metrics.
- Pembuatan forecasting sederhana menggunakan Power Query (R Script) untuk memproyeksikan tren transaksi dan pelanggan.
- Perancangan dashboard interaktif menggunakan slicer, navigasi halaman, drill-down, decomposition tree, dan visual analytics.

## 🧠 Business Logic

- Total Transaction Value dihitung berdasarkan total Amount dari seluruh transaksi.
- Total Transactions dihitung berdasarkan jumlah Transaction ID.
- Active Customers dihitung berdasarkan jumlah Customer ID unik.
- Average Transaction Amount dihitung menggunakan rata-rata Amount pada seluruh transaksi.
- Total Fee Revenue dihitung sebagai penjumlahan Credit Card Fees, Insurance Fees, dan Late Payment Amount.
- Average Fee per Transaction dihitung menggunakan Total Fee Revenue dibagi Total Transactions.
- Customer Segment digunakan untuk mengelompokkan pelanggan berdasarkan tingkat pendapatan.
- Credit Score Segment dibentuk menggunakan grouping Customer Score menjadi enam kategori risiko, yaitu Distressed, High Risk, Moderate Risk, Standard, Preferred, dan Prime.
- Forecast transaksi dan pelanggan dibuat menggunakan Recursive Moving Average sebagai pendekatan sederhana untuk memproyeksikan tren beberapa bulan berikutnya.
- Branch Performance dievaluasi menggunakan kombinasi Total Transaction Value, Total Transactions, Active Customers, Average Transaction Amount, dan Average Credit Score.
- Fee Revenue Breakdown dianalisis menggunakan Decomposition Tree untuk mengidentifikasi jalur kontribusi fee-based revenue berdasarkan Product Category, Customer Segment, Credit Score Segment, Transaction Type, dan Channel.

## 🛠️ Tools & Skills

- Microsoft Power BI
- Power Query
- R Script
- Data modeling
- Star schema
- DAX (Data Analysis Expressions)
- Calculated columns & measures
- Forecasting
- Business intelligence
- Banking analytics
- Data visualization & dashboard design
- Business analysis

## 📊 Preview & Insights

### Executive Overview

Dashboard untuk memantau aktivitas transaksi, performa produk, distribusi channel, serta perkembangan nilai transaksi secara menyeluruh.

<img width="4100" height="2350" alt="banking-transactions-analytics-1" src="https://github.com/user-attachments/assets/fa6fbd9b-38cc-4885-aeef-1fef85116468" />

### Insights

- Selama tahun **2024**, bank memproses **total transaction value** sebesar sekitar **€35,81 juta** yang berasal dari **7 ribu transaksi** dengan **5 ribu pelanggan aktif**. Nilai rata-rata setiap transaksi mencapai sekitar **€5,06 ribu**, sedangkan **fee-based revenue** yang dihasilkan mencapai sekitar **€222,80 ribu**, menunjukkan bahwa sebagian besar aktivitas bank berasal dari pemrosesan transaksi, sementara pendapatan diperoleh melalui biaya layanan yang dikenakan pada transaksi tertentu.
- Perkembangan **total transaction value** menunjukkan fluktuasi sepanjang tahun dengan penurunan pada **Februari** dan **Juni**, sebelum meningkat kembali dan mencapai nilai tertinggi pada **Desember**. Pola tersebut mengindikasikan peningkatan aktivitas transaksi menjelang akhir tahun.
- Distribusi transaksi berdasarkan **Channel** relatif merata. **Mobile Banking** menjadi channel yang paling banyak digunakan dengan kontribusi sekitar **26,91%**, diikuti **Branch Banking (24,76%)**, **ATM (24,37%)**, dan **Online Banking (23,96%)**. Kondisi ini menunjukkan bahwa pelanggan telah memanfaatkan berbagai kanal layanan secara seimbang.
- Berdasarkan **Product Category**, **Mortgage** menghasilkan **total transaction value** terbesar, diikuti oleh **Loan** dan **Credit Card**, sedangkan **Savings Account** memberikan kontribusi nilai transaksi terendah. Temuan ini menunjukkan bahwa produk pembiayaan masih mendominasi aktivitas finansial pelanggan.
- Analisis berdasarkan **Customer Segment** menunjukkan bahwa **Middle Income Segment** menghasilkan **total transaction value** terbesar dibandingkan segmen lainnya. Hampir seluruh kategori produk juga mencatat performa terbaik pada segmen ini, sehingga kelompok pelanggan tersebut menjadi kontributor utama aktivitas transaksi selama periode pengamatan.

---

### Customer Insight

Dashboard untuk mengevaluasi karakteristik pelanggan, perilaku transaksi, serta performa cabang berdasarkan berbagai metrik utama.
<img width="4100" height="2350" alt="banking-transactions-analytics-2" src="https://github.com/user-attachments/assets/85ba4e65-ea4f-4dda-8411-96304e1056b6" />

### Insights

- Selama tahun **2024**, terdapat sekitar **5 ribu pelanggan aktif** dengan **rata-rata pendapatan bulanan €5,49 ribu** dan **rata-rata credit score 576**, yang menunjukkan bahwa mayoritas pelanggan berada pada kategori risiko menengah.
- Jumlah pelanggan aktif mengalami fluktuasi sepanjang tahun dengan penurunan pada **Februari**, kemudian meningkat hingga mencapai puncaknya pada **Juli**, sebelum kembali stabil dan meningkat pada **Desember**. Pola ini menunjukkan adanya perubahan aktivitas pelanggan sepanjang periode observasi.
- Analisis **Transaction Behavior by Credit Score Segment** menunjukkan bahwa kelompok **Distressed**, **High Risk**, **Moderate Risk**, **Standard**, dan **Preferred** memiliki volume transaksi yang relatif serupa dengan komposisi jenis transaksi yang konsisten. Sebaliknya, kelompok **Prime** mencatat volume transaksi yang lebih rendah dibandingkan segmen lainnya, mengindikasikan bahwa pelanggan dengan credit score tertinggi tidak selalu menjadi kelompok yang paling aktif dalam bertransaksi.
- Ringkasan profil pelanggan memperlihatkan bahwa kelompok **Preferred** memiliki jumlah pelanggan aktif terbesar, sedangkan kelompok **Prime** memiliki jumlah pelanggan paling sedikit namun mencatat **rata-rata credit score tertinggi**. Di sisi lain, rata-rata **monthly income** dan **transaction value** antar segmen tidak menunjukkan perbedaan yang terlalu besar, sehingga aktivitas transaksi tidak hanya dipengaruhi oleh tingkat credit score.
- Analisis performa cabang menunjukkan bahwa **Zaragoza** mencatat **total transaction value** terbesar dengan lebih dari **€4,8 juta**, diikuti oleh **Murcia** dan **Malaga**. Perbedaan performa antar cabang lebih dipengaruhi oleh jumlah transaksi dan pelanggan aktif dibandingkan rata-rata nilai transaksi maupun credit score pelanggan.

---

### Revenue Analytics

Dashboard untuk mengevaluasi pendapatan berbasis biaya (fee-based revenue) berdasarkan produk, pelanggan, jenis transaksi, dan channel.
<img width="4100" height="2350" alt="banking-transactions-analytics-3" src="https://github.com/user-attachments/assets/a9648953-96c4-4cf9-befd-ba5af0cb80dd" />

### Insights

- Selama tahun **2024**, bank menghasilkan **fee-based revenue** sebesar sekitar **€222,80 ribu**. Pendapatan tersebut didominasi oleh **Late Payment Amount (€120 ribu)**, diikuti **Insurance Fees (€70 ribu)** dan **Credit Card Fees (€40 ribu)**. Rata-rata pendapatan biaya yang diperoleh bank mencapai sekitar **€31,46** untuk setiap transaksi.
- Analisis **Fee Revenue Breakdown** menunjukkan bahwa produk **Loan** menjadi kontributor terbesar terhadap **fee-based revenue**. Pada jalur analisis yang dipilih, kontribusi terbesar berasal dari **High Income Segment**, kemudian mengerucut pada pelanggan dengan **Prime Credit Score**, di mana **Loan Payment** menjadi jenis transaksi utama yang menghasilkan fee. Pada tahap akhir, **Branch Banking** menjadi channel dengan kontribusi fee tertinggi dibandingkan ATM, Mobile, maupun Online Banking untuk kombinasi pelanggan tersebut.
- Berdasarkan **Product Category**, **Loan** menghasilkan **fee-based revenue** terbesar dengan selisih yang cukup signifikan dibandingkan kategori produk lainnya. **Credit Card** menempati posisi kedua, sedangkan **Mortgage** dan **Savings Account** memberikan kontribusi fee yang relatif lebih rendah.
- Distribusi **fee-based revenue** berdasarkan **Customer Segment** menunjukkan bahwa **Middle Income Segment** memberikan kontribusi terbesar terhadap total pendapatan berbasis biaya, diikuti oleh **High Income Segment** dan **Low Income Segment**. Temuan ini menunjukkan bahwa peluang pendapatan bank tidak hanya berasal dari nasabah berpendapatan tinggi, tetapi juga didukung oleh tingginya aktivitas transaksi pada segmen menengah.
- Secara keseluruhan, **Loan** menjadi kontributor utama **fee-based revenue**, terutama melalui transaksi **Loan Payment**. Temuan ini dapat menjadi dasar dalam mengevaluasi strategi produk, mengoptimalkan sumber pendapatan berbasis biaya, serta mengidentifikasi segmen pelanggan yang memberikan kontribusi terbesar terhadap pendapatan non-bunga bank.

## 💡 Business Recommendations

Berdasarkan hasil analisis dashboard, beberapa rekomendasi bisnis yang dapat dipertimbangkan antara lain:

- **Optimalkan produk pembiayaan sebagai penggerak bisnis utama.** Produk **Loan** dan **Mortgage** menghasilkan nilai transaksi tertinggi, sementara **Loan** juga menjadi kontributor terbesar terhadap **fee-based revenue**. Bank dapat memperkuat strategi cross-selling dan upselling pada produk pembiayaan untuk meningkatkan aktivitas transaksi sekaligus pendapatan berbasis biaya.

- **Terapkan strategi pemasaran yang lebih tersegmentasi.** **Middle Income Segment** memberikan kontribusi terbesar terhadap nilai transaksi dan fee-based revenue, sedangkan pelanggan dengan **Prime Credit Score** menunjukkan kontribusi fee yang tinggi pada jalur analisis Loan. Pendekatan pemasaran yang disesuaikan dengan karakteristik masing-masing segmen dapat meningkatkan efektivitas penawaran produk.

- **Percepat transformasi layanan digital tanpa mengabaikan layanan cabang.** Meskipun **Mobile Banking** menjadi channel yang paling banyak digunakan, kontribusi transaksi masih relatif seimbang dengan Branch, ATM, dan Online Banking. Kondisi ini menunjukkan pentingnya menjaga pengalaman pelanggan secara konsisten di seluruh channel (omnichannel banking).

- **Lakukan monitoring kapasitas operasional secara berkala.** Tren menunjukkan peningkatan aktivitas transaksi dan jumlah pelanggan pada periode akhir tahun. Informasi ini dapat dimanfaatkan untuk merencanakan kebutuhan sumber daya, kapasitas sistem, maupun pelayanan cabang agar mampu mengakomodasi peningkatan volume transaksi.

- **Diversifikasi sumber fee-based revenue.** Pendapatan berbasis biaya saat ini masih didominasi oleh **Late Payment Amount**. Bank dapat mengurangi ketergantungan terhadap pendapatan yang bersifat penalti dengan meningkatkan kontribusi dari layanan bernilai tambah, seperti produk kartu kredit, asuransi, maupun layanan digital yang memberikan fee secara berkelanjutan.
