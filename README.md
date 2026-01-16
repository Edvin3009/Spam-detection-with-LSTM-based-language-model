### Spam detection with LSTM based language model

The goal of the language model is to classify SMS texts into spam and not spam (ham). The dataset used for training is from UC Irvine Machine Learning Repository and can be found here:
https://archive.ics.uci.edu/dataset/228/sms+spam+collection 

## Results

The dataset was split into 70% training data and 30% test data

Testing results:
              precision    recall  f1-score   support

         Ham       0.98      0.98      0.98      1435
        Spam       0.87      0.90      0.89       238

    accuracy                           0.97      1673
   macro avg       0.93      0.94      0.93      1673
weighted avg       0.97      0.97      0.97      1673


The results show that the model is slightly biased towards predicting ham, leading to a higher recall for ham than spam.
This is a good thing, considering marking a spam SMS as ham is less critical of a mistake than marking a ham SMS as spam.