# ML-course-final-project

## Problem
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
