# 🎯 GenAI Hackathon – Google Play Store Data Analysis

### *Official Submission for Innomatics Research Labs – GenAI Internship Test (15 Nov 2025)*

This project presents a complete end-to-end analysis of Google Play Store applications, integrating multi-source datasets (Excel, JSON, SQLite), performing deep cleaning, exploratory data analysis, statistical tests, NLP, and basic machine learning modeling.

All findings in this README are **directly based on the outputs obtained from the notebook** — no assumptions, no fabricated numbers.

---

## 🛠️ Technologies & Methods Used

### **🔧 Data Cleaning & Processing**
- **Multi-source Data Integration**: Excel, JSON, SQLite database
- **Data Type Conversion**: String to numeric, datetime parsing
- **Missing Value Handling**: Group-based imputation, median filling
- **Outlier Detection**: IQR method for review outliers
- **Text Standardization**: Uppercase conversion, whitespace stripping

### **📊 Statistical Analysis**
- **Descriptive Statistics**: Mean, median, standard deviation
- **Confidence Intervals**: 95% CI using t-distribution
- **Hypothesis Testing**: Chi-square test for independence
- **Correlation Analysis**: Pearson correlation matrix
- **ANOVA**: Parametric testing assumptions

### **🤖 Machine Learning**
- **Linear Regression**: Rating prediction model
- **Feature Engineering**: Sentiment polarity, subjectivity, reviews, installs
- **Model Evaluation**: Coefficient analysis

### **📝 Natural Language Processing**
- **Text Preprocessing**: Lowercase conversion, special character removal
- **Stopword Removal**: NLTK English stopwords
- **Tokenization**: Word-level tokenization
- **Frequency Analysis**: Most common word identification

### **📈 Data Visualization**
- **Histograms**: Distribution analysis
- **Bar Charts**: Category comparisons
- **Correlation Heatmaps**: Relationship mapping
- **Time Series**: Update patterns

---

## 📊 Key Numerical Findings

### **💰 Pricing Insights**
- **Highest Total Price Category**: MEDICAL ($1,540.13)
- **Price Range**: $0 - $400 (after cleaning)
- **Free vs Paid Distribution**: 98.98% Free vs 1.02% Paid

### **⭐ Rating Analysis**
- **Overall Average Rating**: 4.32 ± 0.31
- **95% Confidence Interval**: (4.315, 4.323)
- **Highest Rated Genre**: Board;Pretend Play (4.81)
- **Most Common Rating Range**: 4.1 - 4.3

### **📥 Installation Metrics**
- **Highest Average Installs Category**: PHOTOGRAPHY (256,591,900)
- **Install Distribution**: Heavily right-skewed
- **Recommended Transformation**: Logarithmic

### **👥 User Engagement**
- **Highest Average Reviews Category**: SOCIAL (14,674,170)
- **Review Statistics**: 
  - Mean: 2,196,996.3
  - Median: 110,877.0
  - Skewness: Positively skewed (mean ≫ median)

### **📱 App Metadata**
- **Largest Category**: GAME (135 apps)
- **Most Common Genre**: Action (2,378 apps)
- **Median App Size**: 25.3 MB (after cleaning)
- **Latest Angry Birds Update**: May 24, 2018

### **😊 Sentiment Analysis**
- **Highest Sentiment Polarity Category**: COMICS (0.44981)
- **Best Positive/Negative Ratio**: Calorie Counter - MyNetDiary (41.0)
- **Most Frequent Negative Word**: "game" (4,773 occurrences)

### **📈 Correlation Insights**

- **Installs vs Reviews**: +0.576 (Strong Positive)
- **Installs vs Price**: -0.023 (Weak Negative)
- **Installs vs Rating**: +0.045 (Very Weak Positive)
- **Reviews vs Rating**: +0.095 (Weak Positive)


---

## 🎯 Key Analysis Results

### **🏆 Top Performers by Category**
1. **Highest Total Revenue**: MEDICAL
2. **Most User Reviews**: SOCIAL  
3. **Most Installations**: PHOTOGRAPHY
4. **Best User Ratings**: Board;Pretend Play genre
5. **Highest Sentiment**: COMICS category

### **📊 Statistical Tests**
- **Chi-square Test**: p-value = 0.00046 → App Type and Sentiment are **dependent**
- **Confidence Interval**: 95% confident true rating mean lies between 4.1-4.3
- **Outlier Percentage**: FAMILY category has 6.36% review outliers

### **🤖 Machine Learning Model**
**Linear Regression Equation**:

- Rating = 4.27 + 0.045 × Sentiment_Polarity + 0.077 × Sentiment_Subjectivity + 4.80e-09 × Reviews - 3.06e-11 × Installs

---

## 📈 Business Implications

### **For Developers**
- Focus on **COMICS** and **BOARD games** for higher user satisfaction
- **SOCIAL apps** generate most user engagement  
- **PHOTOGRAPHY apps** have highest installation rates

### **For Marketers**
- **Free apps dominate (98.98%)** - freemium model recommended
- **Medical apps** can command highest prices
- **User reviews** strongly correlate with installations

### **For Product Managers**
- **Rating range 4.1-4.3** is most common - aim for this benchmark
- **Size optimization** important (median 25.3 MB)
- **Regular updates** crucial for user retention

--- 

👤 Author
Krishna Kishore K
Participant — Innomatics GenAI Hackathon
Date: November 15, 2025




