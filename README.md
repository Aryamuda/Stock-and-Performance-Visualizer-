# Stock Performance Visualizer & Comparator

## Deskripsi Singkat

Proyek ini bertujuan untuk mengambil data historis beberapa saham (khususnya 5 saham utama AS beserta S&P 500 ETF - SPY), memvisualisasikan harga dan indikator teknikalnya, serta membandingkan kinerja harga saham tersebut dalam periode waktu tertentu. Visualisasi utama berfokus pada perbandingan persentase perubahan harga untuk melihat bagaimana masing-masing saham berkinerja relatif terhadap satu sama lain dan terhadap pasar (SPY).

## Fitur Utama

* **Pengambilan Data Saham:** Mengambil data historis harga saham (OHLCV - Open, High, Low, Close, Volume), dividen, dan informasi lainnya menggunakan `yfinance`.
* **Perhitungan Indikator Teknikal:** Menghitung berbagai indikator teknikal seperti Simple Moving Average (SMA), Exponential Moving Average (EMA), Relative Strength Index (RSI), dan Volume Weighted Average Price (VWAP) menggunakan library `ta`.
* **Visualisasi Data Individu:** Membuat grafik candlestick interaktif untuk masing-masing saham, lengkap dengan volume dan indikator teknikal yang dipilih. Menggunakan `Plotly` untuk visualisasi yang interaktif dan menarik.
* **Perbandingan Kinerja:** Membuat grafik garis yang membandingkan persentase perubahan harga dari beberapa saham dan SPY selama periode waktu yang ditentukan (misalnya, 5 tahun terakhir) untuk analisis kinerja relatif.
* **Interaktivitas:** Grafik yang dihasilkan memungkinkan zoom, pan, dan menampilkan detail saat kursor diarahkan (hover).

## Teknologi & Alat yang Digunakan

* **Python:** Bahasa pemrograman utama.
* **Jupyter Notebook/Google Colab:** Lingkungan pengembangan interaktif.
* **`yfinance`:** Untuk mengambil data pasar historis dari Yahoo Finance.
* **`pandas`:** Untuk manipulasi dan analisis data.
* **`ta`:** Library untuk analisis teknikal, digunakan untuk menghitung indikator.
* **`plotly`:** Untuk membuat visualisasi data yang interaktif dan dinamis.
* **`matplotlib`:** (Mungkin digunakan secara implisit oleh `mplfinance` atau untuk kustomisasi legenda jika `mplfinance` digunakan pada tahap awal).

## Pengaturan & Instalasi (Setup & Installation)

1.  **Clone Repositori (jika sudah diunggah ke GitHub):**
    ```bash
    git clone [https://github.com/Aryamuda/Stock-and-Performance-Visualizer-.git)
    cd Stock-and-Performance-Visualizer-
    ```

2.  **Buat dan Aktifkan Virtual Environment (Direkomendasikan):**
    ```bash
    python -m venv venv
    # Windows
    venv\Scripts\activate
    # macOS/Linux
    source venv/bin/activate
    ```

3.  **Instal Dependensi:**
    ```bash
    pip install yfinance pandas ta plotly matplotlib # Tambahkan library lain jika ada
    ```
    *(Catatan: `matplotlib` mungkin sudah terinstal sebagai dependensi `plotly` atau `mplfinance` jika Anda menggunakannya.)*

## Cara Penggunaan

1.  Buka file Jupyter Notebook utama (misalnya, `5_Stock_And_Comparison_Performance_With_ETF_SNP500_.ipynb`) di Jupyter Notebook, JupyterLab, atau Google Colab.
2.  Pastikan Anda memiliki koneksi internet untuk mengambil data saham.
3.  Jalankan sel-sel notebook secara berurutan
4.  Grafik interaktif akan ditampilkan sebagai output dari sel-sel yang relevan.

## Contoh Visualisasi

**Contoh Grafik Candlestick dengan Indikator:**
(AAPL.png)

**Contoh Grafik Perbandingan Kinerja:**
(./Performance%20Comparison.png)

## Rencana Pengembangan (To-Do / Future Enhancements)

* [ ] Menambahkan lebih banyak pilihan indikator teknikal.
* [ ] Memungkinkan pengguna untuk memasukkan daftar ticker saham secara dinamis.
* [ ] Membuat antarmuka pengguna (GUI) sederhana menggunakan Streamlit atau Dash.
* [ ] Menyimpan konfigurasi dan hasil analisis.
* [ ] Menambahkan analisis statistik lebih lanjut.

## Kontribusi

Kontribusi, isu, dan permintaan fitur sangat diharapkan! Silakan buka *issue* baru untuk mendiskusikan perubahan yang ingin Anda buat atau *pull request* jika Anda sudah memiliki perbaikan.
