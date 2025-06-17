
```markdown
# 🛒 E-Commerce User Behavior Analytics & Prediction

This end-to-end project simulates, analyzes, and models user behavior in an e-commerce environment using synthetic data. It uncovers actionable insights, predicts purchase decisions with high accuracy, and demonstrates real-time stream processing capabilities.

---

## 📌 Project Description

The goal is to understand what drives user purchases in an online shopping platform by analyzing session data. We use exploratory data analysis, machine learning (Random Forest), and real-time stream simulation (Kafka) to:

- Identify trends in product views, cart additions, and purchases
- Segment customers based on behavior patterns
- Predict purchase likelihood with over **99.98% accuracy**
- Demonstrate real-time scoring using synthetic stream data

---

## 📂 Project Structure

```

ecommerce/
│
├── data\_generator.py          # Script to generate synthetic session data
├── preprocessing.py           # Data cleaning and feature engineering
├── model\_train.py             # Model training (Random Forest)
├── kafka\_simulator.py         # Real-time Kafka-like stream simulation
├── visuals.ipynb              # EDA, visualizations, and dashboards
│
├── ecommerce\_cleaned.csv      # Cleaned dataset
├── stream\_output.csv          # Simulated streaming results
├── ecommerce.ipynb            # Main analysis notebook
├── ecommerce\_report.docx      # Final project report
└── README.md                  # Project overview

````

---

## 📊 Key Visualizations

- Bar Plot: Product Views & Cart Additions by Category  
- Stacked Bar Plot: Cart Abandonment by Category  
- Box Plot: Session Duration vs Purchase  
- Heatmap: Feature Correlation  
- PCA Cluster Plot: Customer Segmentation  
- Interactive Plot: Pages Visited vs Session Duration  

---

## 🧠 Machine Learning Model

- **Model:** Random Forest Classifier  
- **Target:** `purchase_made`  
- **Train/Test Split:** 75% / 25%  
- **Accuracy:** 99.98%  
- **Precision / Recall / F1-Score:** 100%  
- **Top 5 Features:**  
  1. Products Viewed  
  2. Products Added to Cart  
  3. Time Spent Per Page  
  4. Pages Visited  
  5. Session Duration  

---

## 👥 Customer Segmentation (K-Means)

- **Clusters Identified:**  
  1. Browsers (high views, no cart)  
  2. Cart Abandoners (cart added, no purchase)  
  3. One-Click Buyers (short sessions, quick purchases)  
  4. Explorers (long sessions, high engagement)

---

## ⏱ Real-Time Simulation

- **Script:** `kafka_simulator.py`  
- **Frequency:** Generates new session events every 2 seconds  
- **Logic:** Simulates producer-consumer behavior and scoring  

---

## ✅ Business Recommendations

1. Retarget cart abandoners with discounts or reminders  
2. Personalize homepage using session history  
3. Improve checkout UX for Electronics & Fashion  
4. Use real-time scoring for high-intent users  
5. Target clusters with specific marketing campaigns  

---

## ⚙️ Getting Started

1. Clone this repo  
   ```bash
   git clone https://github.com/yourusername/ecommerce-analytics.git
   cd ecommerce-analytics
````

2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

3. Generate synthetic data

   ```bash
   python data_generator.py --rows 50000
   ```

4. Run preprocessing and modeling

   ```bash
   python preprocessing.py
   python model_train.py
   ```

5. Simulate real-time stream

   ```bash
   python kafka_simulator.py
   ```

---

## 📑 License

This project is open-source and free to use under the MIT License.

---

## 🙌 Acknowledgements

Thanks to open-source libraries including:

* Pandas, NumPy, Scikit-learn, Seaborn, Plotly, Kafka (Simulated)

---

## 🚀 Author

**Edward Acquah**
Final Year Computer Engineering Student – University of Ghana

