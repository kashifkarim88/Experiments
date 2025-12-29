Feature Transformation in Linear Regression
Box-Cox vs Yeo-Johnson on Concrete Strength Data

Overview:

This experiment evaluates the impact of feature transformation on linear regression performance when input features are not normally distributed.
Two power transformation techniques Box-Cox and Yeo-Johnson are applied and compared using the Concrete Compressive Strength Dataset.

Dataset :

Target: Strength

Features: All numerical concrete composition variables

Missing Values: None

Methodology :

Train a baseline Linear Regression model without transformation

Analyze feature distributions using histograms and Q–Q plots

Apply Box-Cox transformation (positive-valued features)

Apply Yeo-Johnson transformation (handles zero/negative values)

Train Linear Regression on transformed data

Evaluate using R² score and cross-validation

Key Results :

Feature distributions showed significant skewness before transformation

Both transformations improved model performance and stability

Yeo-Johnson slightly outperformed Box-Cox, with fewer constraints

Cross-validation confirmed better generalization after transformation

Takeaway :

Proper feature transformation can significantly improve model performance, often more than changing or tuning models.
Making data more Gaussian benefits not only linear models, but also deep learning optimization and feature learning.

Tools :

NumPy, Pandas, Matplotlib, Seaborn, SciPy, Scikit-learn