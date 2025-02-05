# 📌 Valorant Gameplay Analysis & Model Comparison

## 📝 Project Overview
This project analyzes Valorant gameplay data and evaluates different machine learning models to predict player performance. The goal is to understand key factors that influence match outcomes.

## 🎮 Dataset
- **Source:** Valorant match statistics
- **Columns:**
  - `Player ID`, `Agent`, `KDA`, `Win/Loss`, `Map`, `Rank`, `Headshot %`, `Damage per Round`
  - `Rounds Won`, `Rounds Lost`, `Economy`, `Spike Plants`, `Spike Defuses`

## ⚙️ Methodology
1. **Data Preprocessing**
   - Handling missing values
   - Label encoding the output
   - Encoding categorical data (e.g., Agents, Maps)

2. **Exploratory Data Analysis (EDA)**
   - Distribution of player statistics
   - Impact of different agents on performance
   - Correlation between rank and gameplay metrics

3. **Model Implementation**
   - XGBoost Classifer for o/p prediction
   - RandomForestClassifier for o/p prediction

4. **Model Evaluation**
   - Accuracy and precision metrics
   - Confusion Matrix visualization
   - Feature Importance analysis

## 🛠️ Installation & Usage
```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Clone the repository
git clone <repo_url>
cd <repo_folder>

# Open Jupyter Notebook
jupyter notebook valorant-analysis-models-comparison.ipynb
```
## Conclusion:
- This analysis provides insights into factors affecting Valorant gameplay performance.
- It helps in selecting the best predictive model for ranking and match outcomes.
