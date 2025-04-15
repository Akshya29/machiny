# Normalization
Standardization and log-transformation are common steps in gene expression analysis, used to remove technical biases and make the data more comparable across genes.

Log transformation- Gene expression data are usually highly skewed; a few genes have very high expression, and the rest are low. Log transformation compresses the range and stabilizes the variance, making the data more symmetric.
Standardization- Rescales each feature to have a mean of 0 and a standard deviation of 1. This helps the model to treat all features equally and prevents high-variance genes from dominating the results.

![My Image](https://github.com/Akshya29/machiny/blob/main/Screenshot%202025-04-15%20153214.png)

This histogram is for the raw gene expression data before standardization-
It's highly right-skewed, meaning most of the values are clustered near zero, with a long tail of higher expression values. 

![My Image](https://github.com/Akshya29/machiny/blob/main/Screenshot%202025-04-15%20144503.png)
This hitogram is after the standardization and log transformation- 
The plot is now symmetric, bell-shaped curve centered around 0, which has now removed the extreme right skew, showing proper standardization.
