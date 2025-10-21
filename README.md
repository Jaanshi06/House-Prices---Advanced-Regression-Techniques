🏡 # House Price Prediction using Machine Learning

📘 ## Project Overview

This project predicts house sale prices using advanced regression techniques on the famous Kaggle House Prices Dataset.
We preprocess the data, perform feature engineering, apply scaling and encoding, and finally train multiple ML models including Linear Regression, Ridge, Random Forest, and LightGBM (with Optuna Tuning) to achieve optimal performance.

🎯 # Goal

To accurately predict the SalePrice of residential homes based on various attributes like:

Lot area

Neighborhood

Building type

Year built

Quality & condition

Garage, basement, and more!

⚙️ # Tech Stack
Category	Tools / Libraries
Language :	Python 🐍
Data Handling	: Pandas, NumPy
Modeling: Scikit-learn, LightGBM
Hyperparameter Tuning	: Optuna 🎯
Environment	: Kaggle Notebook 💻

🧹 # Data Preprocessing

✨ ## Major preprocessing steps performed:

Handled missing values

Log-transformed target (SalePrice) → np.log1p()

One-hot encoded categorical features

Combined train & test before encoding

Scaled numeric columns with StandardScaler

✅ ## Best parameters were then used to train the final LightGBM model with:

n_estimators = 5000

Log-transformed target values

Validation via K-Fold Cross-Validation

📊 # Evaluation

RMSE computed both in log-space and original scale

Kaggle submission achieved Public Score ≈ 0.166 RMSE (log-scale) 🎉

Model generalized well without overfitting

🏆 # Results

Best RMSE (Validation Log Space): ~0.10

Kaggle Submission RMSE: ~0.166

Model: LightGBM + Optuna Tuning

📬 # Author

👩‍💻 Jaanshi Bansal
