# 📊 Stock Price Analysis for StakeHolder : A Study Case on BNI Stock Historical Price  
*A Data-Driven Approach to Support Strategic Decisions for Investors, Risk Managers, and Traders as Stakeholders*

> # 📌 **Project Overview**
## 🔎 Tujuan Proyek :

Proyek ini bertujuan menganalisis pergerakan harga saham PT Bank Negara Indonesia (Persero) Tbk (BBNI) untuk menggali pola, tren, dan dinamika pasar yang dapat dijadikan dasar dalam pengambilan keputusan strategis. Analisis dilakukan dengan pendekatan kuantitatif berbasis data historis, meliputi indikator teknikal seperti Simple Moving Average (SMA) 20 & 50 hari, volatilitas harga, return bulanan dan tahunan, serta Relative Strength Index (RSI).

Selain itu, proyek ini juga menggabungkan hasil analisis tersebut dengan model bahasa ibm-granite/granite-3.3-8b-instruct guna menyusun rangkuman temuan utama dan menghasilkan insight yang lebih sistematis. Integrasi ini tidak hanya memberikan gambaran teknikal semata, tetapi juga membantu dalam membangun rekomendasi yang lebih aplikatif bagi para investor, manajer risiko, maupun trader.

Dengan pendekatan tersebut, proyek ini bertujuan untuk menghadirkan analisis yang tidak hanya informatif, tetapi juga relevan secara praktis. Sehingga nantinya dapat mendukung pengambilan keputusan yang lebih cermat dalam menghadapi dinamika pasar saham BBNI.


## 📚 Latar Belakang : 

Pasar modal Indonesia dalam beberapa tahun terakhir menunjukkan perkembangan yang cukup signifikan, dengan meningkatnya likuiditas serta partisipasi investor. Di antara berbagai sektor, perbankan menempati posisi penting karena kontribusinya yang besar terhadap stabilitas sistem keuangan dan perekonomian nasional. Saham perbankan juga menjadi salah satu instrumen yang paling aktif diperdagangkan di Bursa Efek Indonesia (BEI), sehingga analisis terhadap pergerakan harga saham di sektor ini memiliki nilai strategis bagi investor dan pembuat kebijakan (Sulistiawan, Rudiawarni, & Feliana, 2020).

Dalam praktik investasi, analisis teknikal sering digunakan untuk memahami perilaku pasar dan memprediksi arah pergerakan harga. Indikator seperti Moving Average (MA), Relative Strength Index (RSI), dan MACD terbukti membantu investor dalam mengidentifikasi sinyal beli maupun jual yang relevan di pasar saham Indonesia (Fahrullah, Idris, & Anwar, 2025). Walaupun demikian, sebagian besar penelitian masih berfokus pada validitas indikator tersebut dalam menghasilkan sinyal, tanpa menekankan bagaimana hasil analisis dapat diintegrasikan ke dalam strategi pengambilan keputusan yang komprehensif bagi berbagai pemangku kepentingan.

Oleh karena itu, proyek ini hadir untuk menjembatani kesenjangan tersebut dengan menggabungkan analisis teknikal kuantitatif dan pemodelan AI menggunakan ibm-granite/granite-3.3-8b-instruct. Melalui pendekatan ini, hasil analisis tidak hanya memberikan gambaran deskriptif mengenai tren harga saham, tetapi juga menghasilkan insight preskriptif yang dapat disesuaikan dengan kebutuhan investor individu, manajer portofolio, maupun trader aktif. Dengan demikian, proyek ini diharapkan mampu memberikan kontribusi nyata dalam meningkatkan kualitas pengambilan keputusan di pasar modal Indonesia. 

### Sumber : 
- Fahrullah, M. R., Idris, A. A., & Anwar, A. (2025). Efektivitas analisis teknikal Moving Average Convergence Divergence (MACD) dan Relative Strength Index (RSI) dalam menentukan sinyal jual dan beli saham IDX30. Trending: Jurnal Manajemen dan Ekonomi, 3(2), 23–49. https://doi.org/10.30640/trending.v3i2.3905

- Sulistiawan, D., Rudiawarni, F. A., & Feliana, Y. K. (2020). Examining trading strategies using trend following indicators for Indonesian stock market. International Journal of Trade and Global Markets, 13(1), 52–60. https://doi.org/10.1504/IJTGM.2020.104921


## ❗ Identifikasi Permasalahan : 
Meskipun data pasar dan indikator teknikal tersedia dengan sangat melimpah, para pemangku kepentingan seperti investor, manajer risiko, maupun trader masih menghadapi sejumlah tantangan, antara lain:

1. **Menerjemahkan indikator finansial** yang kompleks menjadi strategi yang jelas dan dapat ditindaklanjuti.
2. **Mengidentifikasi tren saham jangka menengah hingga panjang** yang sesuai dengan profil risiko dan horizon pengambilan keputusan masing-masing.
3. **Mengintegrasikan analisis multi-dimensi** (seperti volatilitas, moving average, tingkat pengembalian, serta indikator momentum) ke dalam suatu rekomendasi yang menyeluruh.
4. **Menjembatani kesenjangan antara sinyal teknikal dan kebutuhan pemangku kepentingan**, di mana bahasa teknis sering kali tidak langsung dapat diterjemahkan menjadi bahasa pengambilan keputusan.

Proyek ini bertujuan untuk menjawab tantangan tersebut dengan tidak hanya melakukan analisis kinerja saham, tetapi juga mengubah hasil temuan menjadi wawasan dan rekomendasi yang terstruktur sesuai dengan kebutuhan setiap kelompok pemangku kepentingan.   


## 🛠 Metodologi & Pendekatan :  
Metodologi dalam proyek ini mengintegrasikan analisis kuantitatif dengan sumarisasi berbasis AI, yang disusun dalam langkah-langkah berikut:  

1. **Pengumpulan & Pra-pemrosesan Data**  
   - Mengambil data historis harga saham BBNI dan menyiapkannya dalam format terstruktur untuk analisis.  

2. **Eksplorasi Data & Visualisasi (EDA) & Visualisasi**  
   - Membuat visualisasi pergerakan harga saham.  
   - Menganalisis indikator teknikal utama, termasuk:  
     - Tren harga penutupan dengan **SMA 20** dan **SMA 50**.  
     - **Analisis volatilitas** untuk mengukur risiko pasar.  
     - **Return bulanan dan tahunan** untuk mengevaluasi konsistensi kinerja.  
     - **RSI (Relative Strength Index)** untuk mengidentifikasi momentum serta kondisi overbought/oversold.  

3. **Pembuatan Insight & Findings**  
   - Menuliskan insight dan temuan berdasarkan hasil visualisasi.  
   - Menyimpan semua insight dan temuan tersebut ke dalam sebuah dataframe untuk diproses lebih lanjut.  

4. **Sumarisasi dengan IBM Granite**  
   - Menggunakan model `ibm-granite/granite-3.3-8b-instruct` untuk melakukan sumarisasi terhadap insight dan temuan yang sebelumnya telah disimpan dalam dataframe.  
   - Menghasilkan sumarisasi terstruktur yang disesuaikan untuk aktor investor, risk manager, dan trader.  

5. **Pembuatan Rekomendasi**  
   - Berdasarkan hasil sumarisasi, dibuat rekomendasi yang lebih kontekstual dan spesifik untuk tiap kelompok pemangku kepentingan.


> # 🗂️ **Raw Dataset Link**
Dataset historis saham BNI tersedia di Kaggle melalui tautan berikut:  
🔗 [BNI Stock Historical Price - Kaggle](https://www.kaggle.com/datasets/caesarmario/bank-negara-indonesia-stock-historical-price/data)


> # 💡 **Insight & Findings**
Bagian ini menyajikan hasil insight yang didasari oleh temuan dari proses  analisis teknikal saham PT Bank Negara Indonesia (BBNI) menggunakan berbagai indikator dan metrik kinerja. Setiap sub-bagian menampilkan visualisasi yang disertai dengan insight dan findings untuk mendukung pengambilan keputusan.


## Trend Analysis (Close + SMA20 & SMA50)
### Visualisasi  
![Trend Analysis](https://raw.githubusercontent.com/PIP-Bravo/BNI_Stock_Price_Analysis_for_StakeHolder/refs/heads/main/visualization_image/trend_analysis.png)  

### Insight  
Terlihat adanya fluktuasi signifikan pada harga saham BNI dari 2019 hingga awal 2025, dengan tiga periode besar tren naik yang signifikan: awal 2021–pertengahan 2023, pertengahan 2023–awal 2024, dan kenaikan tajam di awal 2024 sebelum terjadi penurunan. Periode Maret–April 2020 menunjukkan penurunan tajam, kemungkinan terkait dampak awal pandemi COVID-19. Pola SMA20 dan SMA50 memperlihatkan beberapa kali terjadinya golden cross dan death cross yang menandakan potensi pergantian tren jangka menengah. 

### Findings  
- Penurunan tajam Maret 2020: dari kisaran ±4.000 IDR menjadi ±1.800 IDR.
- Golden cross terjadi di awal 2021 ketika SMA20 memotong SMA50 dari bawah, diikuti tren kenaikan hingga ±5.000 IDR pada pertengahan 2023.
- Death cross terlihat di pertengahan 2024 ketika SMA20 memotong SMA50 dari atas, diikuti penurunan dari ±6.000 IDR menjadi ±4.200 IDR pada awal 2025.
- SMA20 dan SMA50 cenderung rapat pada periode sideways (2022–2023 awal), mengindikasikan stabilitas harga relatif.


## Volatility & Performance Metrics  
### Visualisasi  
![Volatility & Performance](https://raw.githubusercontent.com/PIP-Bravo/BNI_Stock_Price_Analysis_for_StakeHolder/refs/heads/main/visualization_image/volatility_performance_metrics.png)  

### Insight  
Meskipun total return selama periode analisis positif sebesar 3,86%, return tahunan hanya 0,62%, yang menunjukkan pertumbuhan harga yang relatif stagnan dalam jangka panjang. Volatilitas tahunan cukup tinggi, mencapai 33,55%, yang berarti harga saham BNI mengalami fluktuasi besar dari tahun ke tahun. Risiko signifikan terlihat dari max drawdown sebesar -69,71%, serta periode pemulihan terpanjang (longest drawdown) mencapai 786 hari, yang setara dengan lebih dari 2 tahun.  

### Findings  
- Daily volatility: 2,11% → menunjukkan harga harian bisa berfluktuasi ±2% secara rata-rata.
- Annualized volatility: 33,55% → tingkat volatilitas tahunan yang tinggi.
- Total return: 3,86% → profit kumulatif relatif kecil dibandingkan risiko yang diambil.
- Annualized return: 0,62% → rata-rata pertumbuhan tahunan sangat rendah.
- Max drawdown: -69,71% → penurunan harga terbesar hampir 70% dari puncaknya.
- Longest drawdown: 786 hari → butuh waktu sangat lama untuk kembali ke puncak sebelumnya.


## Rolling Volatility Plot  
### Visualisasi  
![Rolling Volatility](https://raw.githubusercontent.com/PIP-Bravo/BNI_Stock_Price_Analysis_for_StakeHolder/refs/heads/main/visualization_image/rolling_volatility.png)  

### Insight  
Terlihat lonjakan volatilitas yang sangat tajam pada Maret–April 2020, mencapai hampir 100% (annualized), yang bertepatan dengan awal pandemi COVID-19 dan gejolak pasar global. Setelahnya, volatilitas cenderung menurun namun tetap berada pada level moderat (20–40%) sepanjang 2021–2023. Menjelang akhir 2024 hingga awal 2025, tren volatilitas kembali meningkat, menandakan potensi ketidakpastian pasar yang lebih besar. 

### Findings  
- Puncak tertinggi volatilitas rolling 30-hari annualized mendekati 1.0 (100%) pada awal 2020.
- Periode stabilitas relatif terlihat pada 2021–2023 dengan kisaran 0.2–0.4 (20–40%).
- Kenaikan bertahap menuju 0.4+ (40%+) terjadi sejak pertengahan 2024 hingga awal 2025.  


## Monthly Returns Analysis  
### Visualisasi  
![Monthly Returns](https://raw.githubusercontent.com/PIP-Bravo/BNI_Stock_Price_Analysis_for_StakeHolder/refs/heads/main/visualization_image/monthly_yearly_returns_heatmap.png)  

### Insight  
Heatmap menunjukkan pola fluktuasi bulanan yang cukup bervariasi dari tahun ke tahun, dengan beberapa bulan menampilkan pergerakan harga ekstrem. Contoh signifikan adalah Maret 2020 yang mencatat penurunan tajam hingga -45,62%, bertepatan dengan awal pandemi COVID-19. Sebaliknya, Oktober 2021 menunjukkan lonjakan harga sebesar +30,23%. Secara musiman, bulan Januari dan Februari cenderung lebih sering mencatatkan kinerja positif, sedangkan Mei dan Desember memiliki kecenderungan negatif di beberapa tahun.

### Findings  
- Maret 2020: -45,62% → penurunan terbesar pada dataset.
- Oktober 2021: +30,23% → kenaikan bulanan terbesar.
- Januari sering positif: 8,52% (2022), 6,98% (2024), 9,66% (2025).
- Desember negatif di 2022 (-6,82%) dan 2024 (-12,65%).
- Mei negatif di 2019 (-12,50%), 2021 (-5,26%), dan 2024 (-16,19%).


## Max/Min Month Results 
### Visualisasi  
![Max Min Month](https://raw.githubusercontent.com/PIP-Bravo/BNI_Stock_Price_Analysis_for_StakeHolder/refs/heads/main/visualization_image/max_min_month_year.png)  

### Insight  
Data menunjukkan tiga bulan terbaik dan terburuk dalam hal return bulanan. Oktober 2021 mencatat kinerja tertinggi sebesar +30,23%, diikuti November 2020 (+26,58%) dan Juni 2020 (+19,58%). Sebaliknya, Maret 2020 mencatat penurunan bulanan terbesar sebesar -45,62%, diikuti Mei 2024 (-16,19%) dan Juni 2022 (-14,44%). Hasil ini menunjukkan bahwa periode awal pandemi COVID-19 menampilkan pergerakan ekstrem, baik penurunan maupun lonjakan harga. 

### Findings  
- Top months-> Oktober 2021: +30,23%; November 2020: +26,58%; Juni 2020: +19,58%. 
- Bottom months-> Maret 2020: -45,62%; Mei 2024: -16,19%; Juni 2022: -14,44%. 


## RSI Analysis  
### Visualisasi  
![RSI Analysis](https://raw.githubusercontent.com/PIP-Bravo/BNI_Stock_Price_Analysis_for_StakeHolder/refs/heads/main/visualization_image/rsi.png)  

### Insight  
Grafik RSI(14) menunjukkan fluktuasi kekuatan relatif harga sepanjang periode 2019–2025, dengan beberapa kali mencapai area overbought di atas 70 dan oversold di bawah 30. Periode overbought terlihat cukup sering pada 2020–2022, yang menunjukkan adanya tekanan beli berlebihan pada fase-fase tertentu. Sebaliknya, area oversold juga muncul secara berkala, menandakan potensi pembalikan harga akibat tekanan jual yang tinggi. 

### Findings  
- Batas overbought: di atas 70 (garis merah putus-putus) sering tercapai pada 2020–2022.
- Batas oversold: di bawah 30 (garis hijau putus-putus) terjadi di beberapa titik, termasuk pada awal 2019 dan periode 2023–2024.


> # ✅ **Recommendations**
Berdasarkan hasil temuan dan insight yang kemudian disumarisasi, berikut adalah rekomendasi yang dibuat untuk masing-masing stakeholder yang teridentifikasi, terkait dengan apa yang harus mereka lakukan dengan saham BNI.

## 👤 Bagi Investor  
- **Menyesuaikan Bobot Portofolio**

  Kurangi proporsi BNI dalam portofolio jika saat ini terlalu besar, mengingat imbal hasil tahunan yang hanya 0,62% dan drawdown yang signifikan. Targetkan maksimal 5–8% dari total portofolio untuk mengurangi dampak risiko saham tunggal.

- **Strategi Masuk/Keluar Berdasarkan Musim**

  Gunakan periode yang secara historis positif (Januari, November) untuk mengakumulasi posisi, dan pertimbangkan untuk mengurangi eksposur sebelum bulan-bulan dengan kinerja yang secara historis negatif (Maret, Mei).

- **Strategi Penangkapan Dividen (Dividend Capture)**

  Jika BNI memiliki jadwal dividen yang stabil, gunakan strategi dividend capture menjelang tanggal ex-date, tetapi batasi periode kepemilikan untuk menghindari volatilitas jangka panjang.

- **Peningkatan Bertahap (Gradual Scaling)**

  Lakukan pembelian secara bertahap (dollar-cost averaging) ketika harga berada di area undervalued berdasarkan rasio P/E dan P/B historis, dikombinasikan dengan sinyal golden cross dari SMA (Simple Moving Average).


## 👤 Bagi Risk Manager  
- **Menerapkan Tingkat Stop-Loss yang Dinamis**

  Terapkan stop-loss adaptif yang disesuaikan dengan volatilitas saat ini. Misalnya, jika ATR (Average True Range) tinggi, gunakan jarak stop-loss yang lebih lebar (2–3x ATR) untuk menghindari terkena market noise.

- **Lindung Nilai dengan Kontrak Berjangka atau Opsi Indeks**

  Gunakan kontrak berjangka IHSG (Indonesian Composite Index) atau opsi saham sektor keuangan untuk melindung nilai (hedging) portofolio selama periode volatilitas tinggi, terutama jika volatilitas rolling > 40%..

- **Sistem Pemantauan Drawdown**

  Siapkan sistem peringatan jika drawdown melebihi 20% dari puncak harga terakhir. Hal ini akan memicu evaluasi ulang posisi dan potensi untuk penyesuaian risiko yang cepat.

- **Formula Ukuran Posisi**

  Terapkan ukuran posisi berbasis risiko yang tetap (misalnya, risiko maksimal 1–2% dari modal per posisi) untuk meminimalkan kerugian kumulatif dari volatilitas ekstrem.  


## 👤 Bagi Trader 
- **Konfirmasi Crossover**

  Gabungkan golden/death cross SMA20-SMA50 dengan indikator volume dan RSI untuk mengonfirmasi sinyal masuk/keluar. Jangan masuk posisi hanya berdasarkan satu crossover saja.

- **Pemanfaatan Volatilitas**

  Ketika volatilitas di atas 50%, gunakan strategi opsi seperti straddle/strangle untuk memanfaatkan pergerakan harga yang besar tanpa arah yang pasti.


- **Swing Trade Berdasarkan Musim**

  Masuk posisi sebelum bulan Januari dan November, dengan target keluar di pertengahan bulan, berdasarkan pola historis yang positif. Hindari membuka posisi besar sebelum Maret atau Mei.

- **Scalping Volatilitas Intraday**

  Gunakan Bollinger Bands dan indikator volatilitas intraday untuk mencari peluang scalping sebesar 0,5–1,5% ketika harga menyentuh batas atas atau bawah, terutama pada hari-hari dengan rilis berita atau laporan keuangan penting.


> # 🤖 **AI Support Explanation**
## Model yang Digunakan
- **ibm-granite/granite-3.3-8b-instruct**

## Penjelasan Singkat Model
Model ini merupakan Large Language Model (LLM) berbasis instruksi (instruction-tuned) yang dikembangkan oleh IBM. Model ini cocok untuk analisis teks, summarization, dan knowledge extraction dalam domain yang membutuhkan bahasa profesional seperti analisis finansial.  

## Pemanfaatan
- Dalam proyek ini, model dimanfaatkan khusus untuk **melakukan summarization dari insight dan findings** yang dihasilkan melalui analisis data pasar.  
- Summarization difokuskan pada **penyusunan narasi terstruktur** berdasarkan perspektif aktor yang berbeda, seperti **Investor, Risk Manager, dan Trader**.  
- Hasil summarization membantu menyederhanakan data teknis yang kompleks menjadi dasar pembuatan rekomendasi yang **mudah dipahami dan relevan bagi stakeholder**.  

## Tahapan Penggunaan
![Tahapan Penggunaan Model IBM]()
1. **Pengumpulan Insight & Findings**  
   - Insight dan temuan hasil analisis data disimpan dalam sebuah DataFrame (`insight_findings_df`), yang mencakup kolom seperti:  
     - *Insight & Findings*  
     - *Evidence*  
     - *Relevance*  

2. **Penyusunan Prompt**  
   - Seluruh teks dari DataFrame digabung menjadi satu string (`full_text`).  
   - Dibuat prompt terstruktur yang memuat instruksi jelas, termasuk:  
     - Kategorisasi insight berdasarkan stakeholder (Investor, Risk Manager, Trader).  
     - Penjelasan detail beserta implikasi strategis.  
     - Kesimpulan komprehensif yang menyatukan semua perspektif.  

3. **Eksekusi Model**  
   - Prompt diberikan ke model `ibm-granite/granite-3.3-8b-instruct` melalui fungsi `output.invoke()`.  
   - Parameter seperti `max_tokens` dan `temperature` diatur untuk mengoptimalkan panjang dan kedalaman jawaban.  

4. **Hasil Summarization**  
   - Model menghasilkan teks naratif terstruktur.  
   - Output kemudian disimpan dalam variabel (`summary_text`) dan ditampilkan dengan format profesional.   


✨ *Kesimpulan singkat:*  
Proyek ini memberikan wawasan mendalam terkait harga saham BNI dengan pendekatan analisis berbasis data historis dan dukungan AI. Stakeholder dapat memanfaatkan insight ini untuk membuat keputusan investasi yang lebih cerdas, tepat waktu, dan relevan dengan kondisi pasar.

---
