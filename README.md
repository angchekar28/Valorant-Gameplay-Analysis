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
   - Implemented for loops to streamline the plotting of Countplots, Histplots, and Barplots across multiple features instead of using separate blocks  

3. **Model Implementation**  
   - Compared XGBoost, Random Forest, and CatBoost using a for loop for efficiency  
   - Performed hyperparameter tuning and k-fold cross-validation for better model performance  

4. **Model Evaluation**  
   - Accuracy and precision metrics  
   - Classification Study 
   - Feature Importance analysis (Not Updated in Code. Basic Fearure Engineering Was Done)
   - Previously, Random Forest had the best accuracy at 78 percent, but after optimization, CatBoost achieved 85 percent accuracy.  

5. **Dimensionality Reduction**  
   - Attempted dimensionality reduction using LDA, but it did not provide significant improvements. Hence, it was not included in the final project scope.

## 🏆 Conclusion
- CatBoost demonstrated the highest accuracy and is the most suitable model for this dataset  
- Hyperparameter tuning played a crucial role in enhancing performance, highlighting the importance of fine-tuning machine learning models  
- Dimensionality reduction methods like LDA may not always be beneficial, and their effectiveness depends on the dataset and feature distribution (Removed from code)  
- Using for loops for visualization and model comparisons increased efficiency and improved code readability  
- Future improvements could include testing additional models, feature engineering, and exploring alternative dimensionality reduction techniques  

## 🚀 Feature Scaling & Deep Learning Experiment
I have performed feature scaling and deep learning separately in a Google Colab notebook. However, the results did not show a significant improvement nor outperformed CatBoost's accuracy of 85 percent.  
I would love to hear your suggestions on improving the model performance.  

## 🛠️ Installation & Usage
```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Clone the repository
git clone <repo_url>
cd <repo_folder>

# Open Jupyter Notebook
jupyter notebook valorant-analysis-models-comparison.ipynb
