# International-Education-Costs-Data-Analysis
The following repository deals with the notebook of  International-Education-Costs and built a predictive system.
# 🌎 International Education Cost Analysis

![Dashboard Preview](screenshots/dashboard.png)

## 📌 Project Overview
Analysis of global higher education costs using the **International_Education_costs** dataset to help students:
- Compare tuition + living expenses across 50+ countries
- Identify most affordable study destinations
- Budget for hidden costs (visas, insurance, textbooks)

## 🚀 How to Use
git clone https://github.com/yourusername/education-cost-analysis.git

## 📂 Dataset
**File**: `International_Education_costs.csv`  
**Size**: 15,000+ records  
**Key Columns**:
| Column | Description | Example |
|--------|-------------|---------|
| `country` | Study destination | Germany |
| `university` | Institution name | TU Munich |
| `degree_level` | Bachelor/Master/PhD | Master |
| `tuition_usd` | Annual fees | 12500 |
| `living_cost_index` | Cost of living score | 72.5 |
| `visa_fee` | Student visa cost | 110 |

## 📂 Repository Structure

.
├── data/
│   ├── International_Education_costs.csv
│   └── cleaned_data.csv
├── analysis.ipynb
├── README.md
└── screenshots/

[View Sample Data](data/sample.csv)

## 🔍 Key Insights
1. **Cost Comparison**:
   - Germany offers free tuition but high living costs (€12k/year)
   - US MBA programs cost 3x more than European equivalents

2. **Affordability Score**:
   ```python
   df['affordability'] = df['university_rank'] / df['total_cost']
