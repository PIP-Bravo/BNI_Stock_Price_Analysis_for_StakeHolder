# 📊 Stock Price Analysis for StakeHolder : A Study Case on BNI Stock Historical Price  
*A Data-Driven Approach to Support Strategic Decisions for Investors, Risk Managers, and Traders as Stakeholders*

> # 📌 Project Overview
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


> # 🗂️ Raw Dataset Link
Dataset historis saham BNI tersedia di Kaggle melalui tautan berikut:  
🔗 [BNI Stock Historical Price - Kaggle](https://www.kaggle.com/datasets/caesarmario/bank-negara-indonesia-stock-historical-price/data)


> # 💡 Insight & Findings
Bagian ini menyajikan hasil temuan dan insight dari proses  analisis teknikal saham PT Bank Negara Indonesia (BBNI) menggunakan berbagai indikator dan metrik kinerja. Setiap sub-bagian menampilkan visualisasi yang disertai dengan insight dan findings untuk mendukung pengambilan keputusan.


## 5.1 Trend Analysis (Close + SMA20 & SMA50)
### Visualisasi  
![Trend Analysis](path/to/your/image.png)  

### Insight  
- (Tuliskan insight utama di sini, misalnya: pergerakan harga saham cenderung naik dalam jangka menengah dengan dukungan SMA 20 dan SMA 50.)  

### Findings  
- (Tuliskan temuan detail di sini, misalnya: harga berhasil menembus SMA 50 sebagai sinyal bullish jangka panjang.)  


## 5.2 Volatility & Performance Metrics  
### Visualisasi  
![Volatility & Performance](path/to/your/image.png)  

### Insight  
- (Contoh: volatilitas bulanan menunjukkan fluktuasi signifikan pada periode tertentu, mengindikasikan adanya tekanan pasar eksternal.)  

### Findings  
- (Contoh: return tahunan menunjukkan konsistensi positif meskipun terdapat periode volatilitas tinggi.)  


## 5.3 Rolling Volatility Plot  
### Visualisasi  
![Rolling Volatility](path/to/your/image.png)  

### Insight  
- (Contoh: rolling volatility memperlihatkan pola peningkatan risiko pada periode tertentu, diikuti dengan fase stabilisasi.)  

### Findings  
- (Contoh: investor perlu memperhatikan lonjakan volatilitas karena berpotensi memengaruhi keputusan entry/exit.)  


## 5.4 Monthly Returns Analysis  
### Visualisasi  
![Monthly Returns](path/to/your/image.png)  

### Insight  
- (Contoh: return bulanan menunjukkan pola musiman dengan kinerja kuat di kuartal pertama.)  

### Findings  
- (Contoh: strategi dollar-cost averaging dapat memanfaatkan fluktuasi bulanan untuk akumulasi saham.)  


## 5.5 Max/Min Month Results 
### Visualisasi  
![Max Min Month](path/to/your/image.png)  

### Insight  
- (Contoh: kinerja tahunan menunjukkan tren pertumbuhan konsisten meskipun terjadi fluktuasi pasar global.)  

### Findings  
- (Contoh: return positif berturut-turut selama beberapa tahun memperkuat daya tarik saham sebagai investasi jangka panjang.)  


## 5.6 RSI Analysis  
### Visualisasi  
![RSI Analysis](path/to/your/image.png)  

### Insight  
- (Contoh: RSI mengindikasikan kondisi overbought pada beberapa periode, diikuti koreksi harga jangka pendek.)  

### Findings  
- (Contoh: trader dapat menggunakan sinyal RSI ini untuk timing entry/exit, sementara investor jangka panjang melihatnya sebagai peluang beli ketika harga terkoreksi.)   


> # 🤖 AI Support Explanation
Analisis ini didukung dengan pemanfaatan teknologi AI, khususnya **Large Language Model (LLM)**, untuk meningkatkan efektivitas dalam interpretasi data.  

- **Classification**: AI digunakan untuk mengelompokkan periode harga saham berdasarkan volatilitas (tinggi, sedang, rendah).  
- **Summarization**: Hasil analisis grafik serta data numerik diringkas oleh LLM menjadi insight yang mudah dipahami stakeholder.  
- **Sentiment Analysis**: AI dapat dikembangkan lebih lanjut untuk menganalisis sentimen berita ekonomi terhadap pergerakan harga saham BNI.  

Dengan adanya dukungan AI, proses analisis menjadi lebih cepat, akurat, dan actionable bagi stakeholder.  

---

✨ *Kesimpulan singkat:*  
Proyek ini memberikan wawasan mendalam terkait harga saham BNI dengan pendekatan analisis berbasis data historis dan dukungan AI. Stakeholder dapat memanfaatkan insight ini untuk membuat keputusan investasi yang lebih cerdas, tepat waktu, dan relevan dengan kondisi pasar.

---
