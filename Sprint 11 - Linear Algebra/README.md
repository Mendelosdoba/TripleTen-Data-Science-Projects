
## Conclusions

In this project, we applied machine learning and linear algebra techniques to solve key business problems for the Sure Tomorrow insurance company.

For customer similarity, we demonstrated that kNN is highly sensitive to feature scaling. Without scaling, features with large magnitudes (such as income) dominated the distance calculations, leading to biased results. After scaling, all features contributed equally, significantly improving model performance.

For classification, the baseline random model performed poorly, confirming that it failed to capture any meaningful structure in the data. In contrast, kNN with properly scaled features achieved a very high F1 score, indicating that strong and exploitable patterns exist in the dataset.

For regression, we implemented Linear Regression using matrix operations. We found that feature scaling changes the numerical values of the model coefficients but does not affect prediction quality. Both RMSE and R² remained unchanged, confirming that linear regression is invariant to linear feature scaling.

For data protection, we applied a linear transformation by multiplying the feature matrix with an invertible matrix. Both theoretical analysis and experimental results showed that this transformation does not affect model predictions or evaluation metrics. While the transformed data becomes unreadable, model performance remains identical. Minor reconstruction differences are due to floating-point precision and are not practically significant.

Overall, this project demonstrates that it is possible to build accurate machine learning models while simultaneously ensuring data privacy, and highlights the importance of proper preprocessing and linear algebra techniques in real-world applications.
