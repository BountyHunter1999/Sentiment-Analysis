# How to evaluate our model?

| &darr; Predicted/Actual &rarr; | Positive              | Negative              |
| ------------------------------ | --------------------- | --------------------- |
| Positive                       | True Positives (TPs)  | False Positives (FPs) |
| Negative                       | False Negatives (FNs) | True Negatives (TNs)  |

## Precision

$$ Precision = {TP \over (TP + FP)} $$

| &darr; Predicted/Actual &rarr; | Positive | Negative |
| ------------------------------ | -------- | -------- |
| Positive                       | TP: 1    | FP: 1    |
| Negative                       | FN: 8    | TN: 90   |

> **What proportion of positive identifications was actually correct?**

- Precision here is: (1/(1+1)) => 0.5, our model predicts a tumor is malignant, it is correct 50% of the time.
- It might be okay but it is still not a good result

## Recall

$$ Recall = {TP \over (TP + FN)} $$

| &darr; Predicted/Actual &rarr; | Positive | Negative |
| ------------------------------ | -------- | -------- |
| Positive                       | TP: 1    | FP: 1    |
| Negative                       | FN: 8    | TN: 90   |

> **What proportion of actual positives was identified correctly?**

- Recall here is: (1/(1+8)) => 0.11, our model correctly identifies 11% of all malignant tumors.
- This is just bad

## F1 score

- Harmonic Mean of Precision and Recall

$$ F1 = {{2 * Precision * Recall} \over {Precision + Recall}} $$

> The goal of F1 score is to combine the precision and recall metrics into a single metric

- It has been designed to work well on imbalanced data

# Which to Use?

- Each metric has advantages and disadvantages and each of them will give us specific information on the strengths and weaknesses of our model
- I would normally just see the 3 results and decide upon my model tuning
