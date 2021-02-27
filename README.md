# [뱅크샐러드] MLE Problem

## 01_EDA.ipynb
* text EDA 진행 (text len 설정을 위해)
** 글자단위, 띄어쓰기단위, BertTokenizer 단위로 진행함

## 02-01_Cnnbased_model.ipynb
* cnn + lstm 을 활용하여 모델 구조를 만들고 test를 진행함
* EDA시 title len에 대한 변수를 활용예정이였으나, 현재까지는 정확도에 좋은 영향을 주지 못함
  (향후 변수로 활용 가능 할 것이라고 판단됨)
* 결과
***
model_test_score(loss) : 0.42441055178642273
model_test_score(accuracy)( : 0.9180707931518555
==============================
              precision    recall  f1-score   support

           0       0.92      0.91      0.91       912
           1       0.00      0.00      0.00         0
           2       0.88      0.93      0.91       258
           3       0.80      0.85      0.82       206
           4       0.96      0.94      0.95      1840
           5       0.85      0.87      0.86       223
           6       0.82      0.80      0.81        94
           7       0.83      0.83      0.83       272
           8       0.77      0.79      0.78        58
           9       0.91      0.82      0.86       120
          10       0.89      0.93      0.91       195
          11       0.98      1.00      0.99        90
          12       0.97      0.97      0.97       290
          13       0.97      0.99      0.98       144
          14       0.80      0.89      0.84        18
          15       0.73      0.80      0.76        10
          16       0.90      1.00      0.95        18

    accuracy                           0.92      4748
   macro avg       0.82      0.84      0.83      4748
weighted avg       0.92      0.92      0.92      4748
***
