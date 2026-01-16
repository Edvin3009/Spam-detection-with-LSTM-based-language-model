## Spam detection with LSTM based language model

The goal of the language model is to classify SMS texts into spam and not spam (ham). The dataset used for training is from UC Irvine Machine Learning Repository and can be found here:
https://archive.ics.uci.edu/dataset/228/sms+spam+collection 

### Results

The dataset was split into 70% training data and 30% test data

| Metric | Value |
|--------|-------|
| **Accuracy** | 0.97 |
| **Macro Average** | 0.93 |
| **Weighted Average** | 0.97 |
| **Total Samples** | 1673 |

.

| Metric | Ham | Spam |
|--------|-----|------|
| **Precision** | 0.98 | 0.87 |
| **Recall** | 0.98 | 0.90 |
| **F1-Score** | 0.98 | 0.89 |
| **Support** | 1435 | 238 |


The results show that the model is slightly biased towards predicting ham, leading to a higher recall for ham than spam.
This is a good thing, considering marking a spam SMS as ham is less critical of a mistake than marking a ham SMS as spam.