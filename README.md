
# DS111 – Phân tích Dữ liệu (Data Analytics)

Dự án học tập môn **DS111 – Phân tích Dữ liệu**

## 1. Giới thiệu dự án

**Đề tài:** Phân tích và dự đoán biến động giá cà phê tại Việt Nam dựa trên dữ liệu giá nông sản, thời tiết, tỷ giá USD/VND, nhiên liệu và hàng hóa thế giới.

**Mục tiêu:**
- Thu thập và lựa chọn nguồn dữ liệu.
- Làm sạch, chuẩn hóa và tích hợp dữ liệu.
- Khám phá các mối liên hệ giữa các biến.
- Trực quan hóa dữ liệu bằng Dashboard.
- Xây dựng và đánh giá các mô hình dự đoán.

Quy trình phân tích dựa trên **CRISP-DM** gồm 6 giai đoạn: Business Understanding, Data Understanding, Data Preparation, Modeling, Evaluation và Deployment.

## 2. Nội dung chương trình

| Chương | Nội dung |
|---|---|
| 1 | Giới thiệu và thu thập dữ liệu |
| 2 | Xử lý dữ liệu (Data Preprocessing) |
| 3 | Phân tích và xây dựng Dashboard |
| 4 | Phân tích thăm dò dữ liệu (EDA) |
| 5 | Phân tích dự đoán (Predictive Analytics) |
| 6 | Phân tích chẩn đoán |
| 7 | Xây dựng quy trình phân tích dữ liệu |

## 3. Công nghệ sử dụng

- **Ngôn ngữ:** Python 3.x
- **Xử lý dữ liệu:** Pandas, NumPy
- **Thống kê:** SciPy, Statsmodels
- **Học máy:** Scikit-learn
- **Trực quan hóa:** Matplotlib, Seaborn
- **Dashboard:** Power BI
- **Môi trường:** Jupyter Notebook, VS Code

## 4. Bộ dữ liệu

Dự án sử dụng 6 file CSV thuộc các nhóm:

| Nhóm dữ liệu | Mục đích |
|---|---|
| Nông sản | Phân tích giá cà phê nội địa |
| Thời tiết | Nhiệt độ, độ ẩm và điều kiện thời tiết |
| Tỷ giá | Tỷ giá USD/VND |
| Nhiên liệu | Giá dầu diesel |
| Hàng hóa thế giới | Giá cà phê Robusta và dầu Brent |

### Dataset sau tiền xử lý

**File:** `data/processed/coffee_analytics_clean.csv`

- **Số bản ghi:** 616
- **Số cột:** 15
- **Thời gian:** 28/05/2026 – 06/11/2026
- **Địa phương:** Gia Lai, Lâm Đồng, Đắk Lắk, Đắk Nông
- **Biến mục tiêu:** `coffee_price_vnd_kg`
- **Giá trị khuyết sau xử lý:** 0

### Danh sách 15 cột

| Cột | Ý nghĩa |
|---|---|
| date | Ngày quan sát |
| region | Địa phương |
| coffee_price_vnd_kg | Giá cà phê nội địa (VND/kg) |
| temperature_c | Nhiệt độ |
| humidity_pct | Độ ẩm |
| weather_conditions | Điều kiện thời tiết |
| usd_transfer_vnd | Tỷ giá chuyển khoản USD/VND |
| usd_spread_vnd | Chênh lệch tỷ giá mua và bán |
| diesel_price | Giá dầu diesel |
| robusta_price_usd_tonne | Giá cà phê Robusta thế giới |
| brent_price_usd_barrel | Giá dầu Brent |
| month | Tháng |
| day_of_week | Thứ trong tuần |
| coffee_price_ma7_prev | Trung bình 7 quan sát giá trước đó |
| market_missing | Cờ báo thiếu dữ liệu thị trường trước khi điền khuyết |

---

**Môn học:** DS111 – Phân tích Dữ liệu  
**Mục đích:** Học tập và thực hành phân tích dữ liệu bằng Python.