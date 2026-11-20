# House Price Prediction

Project pembelajaran mechine learning sederhana untuk memprediksi harga rumah berdasarkan features dari dataset menggunakan algoritma DecisionTreeRegressor.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)

## 📊 Dataset & Fitur

Dataset dimuat langsung dari repositori ini (`dataset/train.csv` dan `dataset/test.csv`, berbasis dataset harga rumah klasik dengan 81 kolom pada data latih).

* **Target Prediksi:** `SalePrice` (harga jual rumah)
* **Fitur yang Digunakan (`features`):**
  * `LotArea` — Luas area tanah
  * `YearBuilt` — Tahun rumah dibangun
  * `1stFlrSF` — Luas lantai 1 (kaki persegi)
  * `2ndFlrSF` — Luas lantai 2 (kaki persegi)
  * `FullBath` — Jumlah kamar mandi penuh
  * `BedroomAbvGr` — Jumlah kamar tidur di atas permukaan tanah
  * `TotRmsAbvGrd` — Total ruangan di atas permukaan tanah
 
  ## 🧠 Model & Evaluasi

1. **Pembagian Data:** Data dibagi menjadi *training set* dan *validation set* menggunakan `train_test_split` (`random_state=1`).
2. **Model:** `DecisionTreeRegressor(random_state=1)` dilatih menggunakan data latih.
3. **Metrik Evaluasi:** **Mean Absolute Error (MAE)** pada data validasi menghasilkan nilai **29,653** (rata-rata selisih absolut prediksi terhadap harga aktual).

## 🛠️ Teknologi yang Digunakan

* **Python**
* **pandas** — Manipulasi dan pembacaan data tabular (`.csv`)
* **scikit-learn** — Pemodelan `DecisionTreeRegressor`, `train_test_split`, dan metrik `mean_absolute_error`
