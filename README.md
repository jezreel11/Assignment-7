# Assignment-7

## Explanation of Jez's code (Predicting if a booking will be cancelled or not)


### What the code does

- **Selects important features** from the dataset that are likely to affect cancellations  
  (ex: lead time, customer type, deposit type, etc.)

- **Keeps only these features + the target** (`is_canceled`) to focus the model

- **Cleans the data:**
  - Numeric missing values are replaced with the **median**
  - Categorical missing values → replaced with `"UNKNOWN"`

- **Encodes categorical variables** using one-hot encoding so they become numeric and can be used by the model

Makes predictions** on the test dataset

- **Evaluates performance** using:
  - A **classification report** (precision, recall, f1-score)
  - A **confusion matrix** (colored in **red**) to show correct vs incorrect predictions

- **Displays feature importance** to show which booking features had the most impact on predicting cancellations
