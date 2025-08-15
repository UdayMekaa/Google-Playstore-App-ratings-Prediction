# 📱 Google Play Store App Ratings Prediction

This project analyzes **10,000+ Google Play Store apps** and **60,000+ user reviews** to uncover the factors influencing app ratings and to predict them using Machine Learning.

---

## 📊 Project Overview
The objective was to:
- **Understand** what drives high app ratings
- **Process & merge** app metadata with user reviews
- **Engineer sentiment-based features** from textual reviews
- **Build predictive models** to estimate ratings

---

## 📂 Dataset
- **Apps Data**: Metadata for apps (Category, Size, Installs, Price, etc.)
- **Reviews Data**: User reviews with sentiment analysis (Polarity, Subjectivity, Sentiment)

---

## 🛠️ Tools & Libraries
- **Python**: Core programming language
- **Pandas, NumPy**: Data manipulation
- **Matplotlib, Seaborn**: Data visualization
- **Scikit-learn**: Model building & evaluation
- **TextBlob**: NLP sentiment analysis

---

## 🔍 Steps & Methodology
1. **Data Cleaning & Preprocessing**
   - Handled missing values
   - Standardized size and price formats
   - Log transformation for skewed variables

2. **Merging Datasets**
   - Left-joined apps and reviews on the `App` column

3. **Feature Engineering**
   - Created sentiment metrics: Polarity_Mean, Subjectivity_Mean
   - Added sentiment shares (Positive, Neutral, Negative)
   - Encoded categorical variables (Type, Content Rating)

4. **Modeling**
   - **Linear Regression**
   - **Random Forest Regressor** (Best performer)
   - Evaluation metrics: MAE, RMSE, R²

5. **Key Insights**
   - Sentiment-based features had the highest influence on ratings
   - Random Forest achieved **R² = 0.48**, **MAE = 0.167**

---

## 📈 Results
| Model              | MAE     | RMSE    | R²     |
|--------------------|---------|---------|--------|
| Linear Regression  | 0.210   | 0.283   | 0.264  |
| Random Forest      | 0.167   | 0.238   | 0.480  |

---

## 💡 Insights
- Positive user sentiment strongly correlates with higher app ratings.
- Subjectivity in reviews also plays a significant role.
- App size and install count were weaker predictors compared to sentiment.

---

## 📦 How to Run
```bash
# Clone the repository
git clone https://github.com/<your-username>/google-play-ratings-prediction.git

# Navigate to the project directory
cd google-play-ratings-prediction

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook
```
**Author:** Uday Meka \
**Mail:** satyaudaymeka@gmail.com \
**Linkedin:** https://www.linkedin.com/in/uday-meka/
