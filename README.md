##  Data Analysis Report: User Funnel & Demographic Insights

---

## 1. Data Overview

The dataset contains user interaction and loan processing data, including demographic, geographic, and funnel-related features.

* Original dataset size: ~1,000,000 rows
* Cleaned dataset (with valid age): ~180,000 rows
* Key features analyzed:

  * User funnel stages (`state_id`)
  * Conversion indicators (`loan_no`, `kyc_successful`)
  * Demographics (`age`, `gender`)
  * Geography (`state`, `city`)

---

## 2. Data Cleaning & Preprocessing

* Removed irrelevant and highly sparse columns (e.g., company details, coordinates)
* Converted `dob` to age and filtered unrealistic values (18–60)
* Handled missing values appropriately:

  * Gender → filled as “Unknown” (in full dataset)
  * Age → derived only for valid DOB records
* Maintained two datasets:

  * **Full dataset** → for funnel & conversion analysis
  * **Filtered dataset** → for age-based analysis

---

## 3. Demographic Insights

### Age Distribution

* Majority users fall in the **24–35 age range**
* Peak around late 20s
* Very low participation from users above 50

👉 Indicates platform primarily attracts **young professionals**

---

### Age Group Distribution

* **26–35 → largest segment**
* 18–25 and 36–50 → moderate presence
* 50+ → minimal

---

### Gender Distribution

* Large portion of missing gender data in original dataset
* Filtered dataset shows male dominance, but may be biased

---

## 4. Funnel Analysis

* Majority of users remain in early stages (e.g., `route_user`)
* Very few users progress to later stages such as KYC and loan approval

👉 Indicates a **significant drop-off at the initial stages**

---

## 5. Conversion Analysis

### Overall Conversion Rate

* Full dataset: **~0.07% (very low)**
* Filtered dataset: **~1.46%**

👉 Users with more complete data are more likely to convert

---

## 6. Geographic Insights

### Top User States

* Maharashtra (highest)
* Karnataka
* Uttar Pradesh
* West Bengal

👉 Strong presence in urban and Tier-2 regions

---

### State-wise Conversion

* High conversion:

  * Tamil Nadu
  * Jharkhand
  * Kerala
* Lower conversion despite high traffic:

  * Maharashtra
  * Karnataka

👉 High traffic ≠ high conversion

---

## 7. Age-wise Conversion

| Age Group | Conversion Rate     |
| --------- | ------------------- |
| 18–25     | 0.85%               |
| 26–35     | 1.55%               |
| 36–50     | **1.89% (highest)** |
| 50–60     | 1.86%               |
| 60–70     | ~0%                 |

### Key Insight:

* Younger users → more engagement
* Older users → higher conversion

---

## 8. Key Insights Summary

* Majority users are **young (26–35)** but **mid-age users (36–50)** convert more
* Conversion rate is **extremely low overall**, indicating funnel inefficiency
* Users with more complete data show higher conversion
* Significant variation in conversion across states
* High traffic regions do not necessarily yield high conversion

---

## 9. Recommendations

### 🔹 Improve Funnel Efficiency

* Simplify onboarding process
* Reduce number of steps
* Add progress indicators

---

### 🔹 Increase Trust & Transparency

* Highlight security and compliance
* Provide clear information on data usage

---

### 🔹 Target High-Converting Segments

* Focus on users aged **36–60**
* Offer personalized loan options

---

### 🔹 Optimize High-Traffic Regions

* Improve UX in states like Maharashtra and Karnataka
* Identify drop-off points region-wise

---

### 🔹 Retarget Drop-off Users

* Use SMS/WhatsApp reminders
* Encourage completion with incentives

---

### 🔹 Encourage Data Completion

* Prompt users to fill missing details early
* Offer benefits for completing profiles

---

## 10. Conclusion

The analysis reveals that while the platform successfully attracts a large number of users, it struggles with conversion due to significant drop-offs in the funnel.

By improving onboarding experience, targeting high-converting segments, and optimizing regional strategies, the platform can significantly enhance its conversion performance and overall efficiency.

---
-Noureen AC
