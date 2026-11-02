#  HCMC Apartment Rental Price Analysis

##  Giới thiệu

**Đề tài:** Phân tích các yếu tố ảnh hưởng đến giá cho thuê và xây dựng mô hình dự đoán giá thuê căn hộ chung cư tại TP. Hồ Chí Minh.

**Môn học:** DS111 – Phân tích dữ liệu  
**Nguồn dữ liệu dự kiến:** [Batdongsan.com.vn](https://batdongsan.com.vn/)  
**Ngôn ngữ:** Python

## Mục tiêu

- Thu thập và tiền xử lý dữ liệu căn hộ cho thuê.
- Phân tích khám phá dữ liệu (EDA).
- Phân tích tương quan và kiểm định thống kê.
- Lựa chọn các đặc trưng ảnh hưởng đến giá thuê.
- Xây dựng và đánh giá mô hình dự đoán giá thuê.
- Trực quan hóa kết quả bằng Dashboard.

## Dataset

Bộ dữ liệu dự kiến gồm **15 thuộc tính**:

`listing_id`, `created_date`, `rental_price`, `district`, `ward`, `project_name`, `area_sqm`, `num_bedrooms`, `num_bathrooms`, `floor_level`, `balcony_direction`, `furniture_status`, `legal_status`, `has_air_conditioner`, `price_per_sqm`.

- **Target:** `rental_price` (triệu VNĐ/tháng).
- **Features:** Các thuộc tính căn hộ được lựa chọn sau tiền xử lý.
- **Lưu ý:** `price_per_sqm = rental_price / area_sqm` chỉ dùng cho phân tích, không dùng làm đầu vào dự đoán `rental_price` để tránh Data Leakage.

## 📁 Cấu trúc thư mục

```text
ds111/
├── dashboard/                 # Dashboard Power BI
├── data/
│   ├── raw/                   # Dữ liệu thô
│   └── processed/             # Dữ liệu đã xử lý
├── notebook/
│   ├── 01_data_collection.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_statistical_analysis.ipynb
│   ├── 05_feature_selection.ipynb
│   ├── 06_modeling.ipynb
│   └── 07_model_evaluation.ipynb
├── reports/                   # Báo cáo và biểu đồ
├── src/                       # Mã nguồn Python
└── README.md
```

## Quy trình thực hiện

1. **Data Collection:** Thu thập dữ liệu từ nguồn được phép.
2. **Data Cleaning:** Xử lý dữ liệu thiếu, trùng lặp và ngoại lệ.
3. **EDA:** Phân tích và trực quan hóa dữ liệu.
4. **Statistical Analysis:** Pearson, Spearman, ANOVA.
5. **Feature Selection:** Mutual Information, Random Forest Importance.
6. **Modeling:** Linear Regression, Random Forest, XGBoost.
7. **Model Evaluation:** Đánh giá bằng MAE, RMSE, R².

## 🛠️ Công nghệ

- **Python:** Pandas, NumPy, Matplotlib, Seaborn, SciPy.
- **Machine Learning:** Scikit-learn, XGBoost.
- **Data Collection:** Requests, BeautifulSoup (khi được phép).
- **Visualization:** Power BI.
- **Development:** Jupyter Notebook, Git, GitHub.

## Chuẩn đầu ra DS111

| Chuẩn | Nội dung |
|---|---|
| G1 | Lựa chọn nguồn và quy trình phân tích dữ liệu |
| G2 | Áp dụng thư viện xây dựng mô hình |
| G3.1 | Đánh giá mô hình phân tích dữ liệu |
| G3.2 | Đánh giá và phản biện kết quả |
| G4 | Thiết kế quy trình phân tích dữ liệu |

##  Kết quả dự kiến

- Dataset đã làm sạch.
- Báo cáo EDA và phân tích thống kê.
- Các mô hình dự đoán giá thuê.
- Bảng so sánh hiệu suất mô hình.
- Dashboard trực quan hóa kết quả.

---

**DS111 – Data Analysis Project**