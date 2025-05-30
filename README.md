# 📊 TikTok Usage Behavior Analysis using Machine Learning

This project explores how personal TikTok sharing behavior evolves over time, using real data collected from TikTok's activity archive. The motivation lies in examining whether social media engagement declines naturally, particularly during exam periods or due to personal disengagement from algorithm-driven content.

---

## 🎯 Motivation

Over time, I noticed that people around me — including myself — began to consume increasingly similar content, visit the same places, and follow the same trends on social media. This raised questions about how my own habits were changing and whether I was subconsciously stepping back from platforms like TikTok.

This project aims to answer that question using data science tools.

---

## 🧾 Dataset

- Personal TikTok data collected via TikTok's [Download Your Data](https://www.tiktok.com/legal/report/data-access/en) feature.
- The dataset includes **monthly counts of shared video links** between 2022 and 2024.
- Additional contextual features were manually added (e.g., final exam months, summer).

---

## ⚙️ Methodology

- **Exploratory Analysis**: Line chart showing month-to-month changes in link sharing.
- **Feature Engineering**:
  - `Previous Month Link Count`
  - `Is_Summer` (June–August)
  - `Is_Final` (June 2024)
- **Modeling**:
  - Trained a **Random Forest Classifier** to predict whether monthly usage increased or decreased
  - Compared with logistic regression, Random Forest performed significantly better

---

## 📈 Results

- **Line Chart**: Clear downward trend with seasonal spikes (e.g. January, June).
- **Random Forest Performance**:
  - Successfully predicted both increases and decreases
  - Highlighted `Previous Month Link Count` as the most important predictor
- **Confusion Matrix & Metrics** included in the notebook

---

## 🔍 Interpretation

The analysis reveals that social media behavior — particularly content sharing — is influenced by both **personal cycles** and **contextual signals** like exams or holidays. The most predictive feature was recent behavior, confirming that short-term digital habits strongly affect future engagement.

---

## 📁 Files Included

- `TikTok_ML_Project_Professional_Final.ipynb`: Full code and analysis
- `results/line_chart.png`: Time-based usage visualization
- `results/feature_importance.png`: Model interpretation
- `data/tiktok_data_cleaned.csv`: Cleaned and anonymized dataset (optional)

---

## 🧠 Conclusion

This project combines personal reflection and technical analysis to model behavioral change on social media. Using simple yet effective machine learning models, we can quantify how and when our engagement shifts — revealing insights that go beyond what the algorithm shows us.

---

## 👤 Author

Arda Dinç – DSA210 (2024–2025 Spring)  
Sabancı University
