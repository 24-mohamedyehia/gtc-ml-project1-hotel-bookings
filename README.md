# 🏨 Hotel Bookings Analysis & Prediction  

## 📌 Project Overview  
This project analyzes hotel booking data and prepares it for machine learning.  
The goal is to clean, explore, and preprocess the dataset so that we can build models to predict booking behaviors (e.g., cancellations).  

---

## 📂 Steps in the Project  

### **1. Data Preparation**  
- Loaded the dataset `hotel_bookings.csv`.  
- Dropped irrelevant columns (e.g., `company`, `agent`).  
- Checked for duplicates and missing values.  
- Handled missing data (imputation or dropping).  

---

### **2. Exploratory Data Analysis (EDA)**  
- Explored basic statistics and distributions.  
- Created visualizations for:  
  - Booking trends across years/months.  
  - Average stay duration.  
  - Cancellations vs. confirmed bookings.  

---

### **3. Feature Engineering & Preprocessing**  
- Created new features:  
  - `total_guests = adults + children + babies`  
  - `total_nights = stays_in_weekend_nights + stays_in_week_nights`  
  - `is_family` → Yes/No if children or babies included.  
- Encoded categorical variables:  
  - One-Hot Encoding for low-cardinality features (`meal`, `market_segment`).  
  - Frequency Encoding / Grouping for high-cardinality features (`country`).  
- Removed data leakage: Dropped `reservation_status` & `reservation_status_date`.  
- Final split into training and testing sets (`test_size=0.2`, `random_state=42`).  

---

## ⚙️ Technologies Used  
- **Python** 🐍  
- **Pandas** & **NumPy** → Data manipulation  
- **Matplotlib** & **Seaborn** → Data visualization  
- **Scikit-learn** → Preprocessing & splitting data  

