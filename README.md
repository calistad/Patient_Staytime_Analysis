# Patient_Staytime_Analysis

## Overview

Predict the Length of Stay for each patient on case by case basis, so that the Hospitals can use this information for optimal resource allocation and better functioning.

### Purpose
Help hospitals to identify patients who will stay longer at the time of admission, so their treatment plan can be optimized to minimize time and lower the chance of staff/visitor infection.

## Approach

The dataset consists of 18 features along with 318,400 entries.
![Screen Shot 2024-08-13 at 3 25 27 PM](https://github.com/user-attachments/assets/9c642d63-36fc-42a2-9d0c-f73b7bc11c8d)

![Screen Shot 2024-08-13 at 3 25 41 PM](https://github.com/user-attachments/assets/4658a51b-0bd7-4b2f-a8fe-8ad53688e769)

* Available extra rooms range from 0 to 24.
![Screen Shot 2024-08-13 at 3 26 31 PM](https://github.com/user-attachments/assets/1c4d3e41-d02f-4567-bca6-09307ea83a1d)

![Screen Shot 2024-08-13 at 3 34 35 PM](https://github.com/user-attachments/assets/63057308-ccd8-4c6e-a251-df98bf648916)
![Screen Shot 2024-08-13 at 3 34 45 PM](https://github.com/user-attachments/assets/12194357-322c-44f7-ac62-ccf503f293c1)
![Screen Shot 2024-08-13 at 3 34 56 PM](https://github.com/user-attachments/assets/8fe640d0-1b13-4a0a-8efc-16c465d5e3e3)

* The gynecology department has the most patients.
![Screen Shot 2024-08-13 at 3 27 32 PM](https://github.com/user-attachments/assets/043419ca-30eb-4c37-b0fa-cde5cfa0bdaa)

* Most patients are between 31 to 50 years old.
![Screen Shot 2024-08-13 at 3 27 46 PM](https://github.com/user-attachments/assets/7481ac53-5043-465d-903a-2da9c7c7f116)

* Most patients stay for 11-30 days hospitalized.

![Screen Shot 2024-08-13 at 3 27 54 PM](https://github.com/user-attachments/assets/0d889b6e-6a28-450b-ad2f-8b2cb92a1cf6)

#### Categorical columns encoding

![Screen Shot 2024-08-13 at 3 37 07 PM](https://github.com/user-attachments/assets/e64d58b9-17f0-42af-a638-98994b2b9db1)
![Screen Shot 2024-08-13 at 3 37 27 PM](https://github.com/user-attachments/assets/ebcf3f71-1893-4e28-9f55-3e1ce5448359)

`Available Extra Rooms in Hospital` is correlated with `Ward_Type` negatively.

`Vistors with Patient` is correlated with `Stay` positively.

![Screen Shot 2024-08-13 at 3 38 36 PM](https://github.com/user-attachments/assets/0cc45b04-e94a-40ec-8316-b50fc9d7ce5c)
![Screen Shot 2024-08-13 at 3 49 36 PM](https://github.com/user-attachments/assets/d5547aed-c3a5-4923-8561-23207d5c59cb)


## Findings

* Training and comparing various models.

![Screen Shot 2024-08-13 at 3 44 30 PM](https://github.com/user-attachments/assets/9c137957-8b5b-414b-aecd-4ea445c565e2)
![Screen Shot 2024-08-13 at 3 44 39 PM](https://github.com/user-attachments/assets/9d1e0874-80bb-41cd-9332-f93f1c4c0d66)

* Training Voting Classifier model.
  
Logistic Regression, Ada Boost, and Bagging Classifier were selected as the estimators because of their high accuracy and low runtime.

* The accuracy is 93.1%, so **Voting Classifier** is the best model for prediction.

![Screen Shot 2024-08-13 at 3 46 39 PM](https://github.com/user-attachments/assets/53491a1c-3619-4b54-af66-7849b2200abf)

