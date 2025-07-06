# 🌟 Anime Rating Prediction using Linear Regression

## 📌 Problem Statement

**Streamist**, a global streaming platform, wants to better understand how viewers rate anime on their platform. Each anime is associated with metadata such as number of episodes, viewers, and type. The goal is to identify which factors drive user ratings and build a model that can predict an anime's average rating.

## 🎯 Objective

To build a supervised learning regression model that can accurately predict anime ratings based on historical viewership and content data.

## 📊 Dataset

- **File**: `anime_data.csv`
- **Target Variable**: `Rating`
- **Sample Features**:
  - `Name`: Anime title
  - `Genre`: Type(s) of anime (e.g., Action, Comedy)
  - `Type`: Format (e.g., TV, Movie, OVA)
  - `Episodes`: Number of episodes
  - `Members`: Number of users who interacted with the anime
  - `Watchers`, `Scored_by`, `Favourites`, etc.

## 🧪 Project Workflow

1. **Data Preprocessing**
   - Handled missing values (e.g., in `Rating`, `Episodes`)
   - Removed non-numeric and irrelevant columns
   - Encoded categorical features (`Type`, `Genre`) appropriately

2. **Exploratory Data Analysis (EDA)**
   - Examined distributions and correlations
   - Visualized impact of `Members`, `Scored_by`, and `Type` on ratings

3. **Feature Selection**
   - Used correlation heatmaps and variance thresholding
   - Selected most relevant features for model training

4. **Model Building**
   - Built a **Linear Regression** model using scikit-learn
   - Evaluated with train-test split
   - Compared with Ridge and Lasso Regression (if applicable)

5. **Model Evaluation**
   - Metrics: R² Score, Mean Absolute Error (MAE), Root Mean Squared Error (RMSE)
   - Residual plots to check model assumptions

## 🏆 Results

- **Best Model**: Linear Regression
- **Key Metrics**:
  - R² Score: ~X.XX
  - MAE: ~X.XX
  - RMSE: ~X.XX
- **Important Predictors**: `Scored_by`, `Members`, `Favourites`, and `Type` were among the top factors influencing ratings

## 📁 Repository Structure

├── SL_MLS1_AnimeRatingPrediction.ipynb
├── anime_data.csv
├── README.md


## 🔍 Key Takeaways

- Content popularity (`Members`, `Scored_by`) is highly correlated with higher ratings
- Anime type and number of episodes also influence perceived quality
- Linear regression provides a solid baseline; regularized models can further improve generalizability

## 🚀 Future Enhancements

- Use NLP on `Genre` and `Synopsis` to extract deeper features
- Deploy the model in a dashboard to explore live predictions
- Explore ensemble regressors like Random Forest or Gradient Boosting

## 👨‍💻 Author

**Suhaib Khalid**  
ML Practitioner
