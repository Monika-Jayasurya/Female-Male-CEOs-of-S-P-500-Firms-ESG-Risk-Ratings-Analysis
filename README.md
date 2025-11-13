# 👩‍💼 Female CEOs and S&P 500 Firms — ESG Risk Analysis

This project analyzes **Environmental, Social, and Governance (ESG)** risk ratings for **S&P 500 companies**, focusing on whether **female-led firms** demonstrate different ESG risk profiles compared to **male-led firms**.  
The study combines **Python-based Exploratory Data Analysis (EDA)** and **SQL analysis** to extract actionable insights about gender diversity, governance, and sustainability transparency.

---

## 📘 Project Context

Organizations globally are being assessed for their environmental, social, and governance (ESG) performance.  
This analysis investigates whether **CEO gender** influences ESG risk outcomes, governance quality, and sustainability practices.

**Objective:**  
To evaluate ESG risk differences between male- and female-led S&P 500 firms, identify transparency gaps, and uncover governance trends across leadership profiles.

---

## 🧩 Dataset Overview

**Dataset Size:** 503 company records  
**Source:** Sustainalytics ESG Ratings (S&P 500 firms)

| Column | Description |
|---------|--------------|
| `Ticker` | Stock symbol of each company |
| `ESG Score` | Composite risk score (lower = better ESG performance) |
| `Environment Score` | Measures environmental management, emissions, and resource use |
| `Social Score` | Reflects employee welfare, diversity, and community engagement |
| `Governance Score` | Assesses transparency, board oversight, and accountability |
| `CEO Full Name` | Full name of company CEO |
| `CEO Gender` | Gender of CEO (male / female / none) |
| `ESG Score Date` | Date of ESG evaluation |
| `ESG Status` | Status of ESG score availability |
| `CEO Status` | Indicates active/inactive CEO position |

---

## 🧹 Data Cleaning and Preparation (Python)

- Validated column types and standardized gender values (`male`, `female`, `None`)
- Converted `ESG Score Date` into datetime format
- Checked and handled null values using `isnull().sum()`
- Filtered incomplete ESG records for accurate analysis

---

## 📊 Python Exploratory Data Analysis (EDA)

### 👩‍⚖️ CEO Gender Distribution
- **Male CEOs:** 462 (92.03%)  
- **Female CEOs:** 40 (7.97%)  
➡️ Significant leadership gender gap in S&P 500 companies.

### ♻️ Overall ESG Risk Scores by Gender
| Metric | Female CEOs | Male CEOs |
|---------|-------------|-----------|
| Mean ESG Risk | **21.60** | 22.09 |
| Median | 19.50 | 21.74 |
| Std. Deviation | 9.15 | 8.11 |

✅ **Insight:** Female-led companies show marginally lower ESG risk and more consistent sustainability governance.

### 🌱 Environmental Risk
| Metric | Female | Male |
|---------|--------|------|
| Mean | 6.41 | 6.47 |
| Median | 2.75 | 3.83 |

➡️ Female-led firms have slightly lower environmental risk; higher variability indicates outliers.

### 🤝 Social Risk
| Metric | Female | Male |
|---------|--------|------|
| Mean | 10.64 | 9.72 |

➡️ Female-led firms show higher social engagement but also variability in stakeholder practices.

### 🏛 Governance Risk
| Metric | Female | Male |
|---------|--------|------|
| Mean | **6.10** | 6.76 |
| Median | 5.71 | 6.24 |

✅ **Insight:** Female-led firms have **lower governance risk**, implying stronger oversight and compliance.

---

## 🧠 SQL Exploratory Data Analysis

### 🔍 Average Scores by CEO Gender
| CEO Gender | Avg ESG | Avg Env | Avg Soc | Avg Gov |
|-------------|----------|----------|----------|----------|
| Female | 21.60 | 6.41 | 10.64 | 7.25 |
| Male | 22.09 | 6.47 | 9.72 | 7.50 |
| None | 34.18 | 7.18 | 18.52 | 8.47 |

✅ **Insight:** Companies with *undisclosed CEO gender* show the **highest ESG risk**, indicating transparency and reporting challenges.

### 🏆 Top Performing Female CEOs
- Female-led firms (e.g., **Gail Koziara Boudreaux**) rank among companies with the **lowest ESG risk**.
- Female CEOs demonstrate better governance and environmental consistency.

### 🚨 High-Risk Clusters
- Firms with missing gender data have the weakest ESG reporting.
- A small group of male-led firms dominate the highest-risk segment.

---

## 📈 Key Findings

1. **Female-led firms** show marginally better overall ESG performance.  
2. **Social engagement** scores higher in female-led companies.  
3. **Governance risk** is lower under female leadership — better accountability.  
4. Companies with **undisclosed CEO gender** show the **highest ESG risk** (poor transparency).  
5. Female-led companies show **more consistency** and fewer extreme outliers.  

---

## 💡 Insights & Recommendations

| Category | Recommendation |
|-----------|----------------|
| **Diversity & Inclusion** | Encourage gender diversity in executive leadership for balanced ESG outcomes. |
| **Transparency** | Enforce CEO and governance disclosure to reduce ESG data risk. |
| **Governance** | Strengthen board independence and accountability frameworks. |
| **Social Responsibility** | Expand employee welfare, diversity, and community programs to maintain social advantage. |

---

## 🧩 Tools & Technologies Used

- **Python:** Pandas, NumPy, Matplotlib, Seaborn (EDA & Visualization)  
- **SQL (SQLite):** Data querying and aggregation  
- **Jupyter Notebook:** Integrated analysis and narrative  
- **Excel:** Data cleaning, validation, and initial inspection  

---

## 📊 Visualization Snapshot

![Female CEOs ESG Analysis Dashboard](https://github.com/user-attachments/assets/your-image-id.png)

*Figure: Distribution of ESG risk scores by CEO gender (Female vs Male)*

---

## 🏁 Conclusion

Female leadership in S&P 500 firms correlates with **slightly lower ESG risks** and **higher social engagement**, reinforcing the value of diversity in executive positions.  
However, limited sample size (only ~8% female CEOs) means future research should expand longitudinally to strengthen conclusions.  

**Transparency and governance disclosure remain critical for reducing ESG-related risks across the corporate landscape.**

---

### 👩‍💼 Author
**Monika Jayasurya**  
_Data Reporting Analyst | ESG & Sustainability Enthusiast_  
📧 monikajayasurya01@gmail.com  
🌐 [LinkedIn](https://linkedin.com) | [GitHub](https://github.com)
