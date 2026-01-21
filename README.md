# ML-course-final-project
![glassdoor](https://github.com/user-attachments/assets/211f66a7-88a5-4cd6-8da8-0c180961536c)

## Problem
The data are Glassdoor reviews. Training data sets (small: 100,00 observations, large: 500,000 observations; small is not a subset of large; you can use both training sets) are posted on Learn. The test data set has 100,000 observations. Test data set without the response variable is also already posted on Learn.

Some feature variables may have missing values. In the prediction competition you cannot skip observations
with missing values on some features: you must give some prediction for all 100,000 observations
in the test set.
</br>
</br>
</br>

Construct features from the available data. Then use these features to predict the overall rating
using any machine learning model. (For this question, you should not use LLM APIs.)

You can utilize either or both training data sets to train the model.

Performance of the algorithm is measured by the accuracy percentage in the test set.

## Given
- `424_F2025_Final_PC_large_train_v1.csv` ($100\ 000\ \text{observations}$)
- `424_F2025_Final_PC_small_train_v1.csv` ($500\ 000\ \text{observations}$)
- `424_F2025_Final_PC_test_without_response_v1.csv` ($100\ 000\ \text{observations}$)
  - Note: the `ratings` feature is empty, as this is the target variable we are supposed to predict, and has a domain $[1,5]\in\mathbb{Z}$
## Output

Using all the other features in `424_F2025_Final_PC_test_without_response_v1.csv`, our model will predict the `ratings` feature for each row, and output a $100\ 000\ x\ 1$ csv file containing these predicted values.
