# Machine-Learning---income-prediction-project
This project is a machine learning one. I used random forests to build a model that is able to pedict the cases income if it is over or under 50k annually. 
the used dataset is relatively old since 1994. For more information describing the dataset is available on the link: https://cseweb.ucsd.edu/classes/sp15/cse190-c/reports/sp15/048.pdf 
The project includes data cleaning, visulization, modeling, pca development, model tuning, and most important features visualization. 

# General notes about the project and the dataset:
- The target of this project is to predict the adults income.
- Each row represents an adult case, where 15 features are included for each case.
- The dataset contains 48,842 cases.
- Capital gain and capital loss features can be combined into one feature taking different signs.
- fnlwgt feature needs exploration to see if it can be considered as an index.
- many features contain inconsistant data that needs cleaning.
- 'education' and 'educational-num' need exploration to see if it can be combined into one feature.
- Some features need encoding first, to be modeled later.

# Some exploratory images to understand the dataset features and its relation with the target feature:
- below is a sample of figures used to explore visualize and understand the dataset.
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/c459c8c7-2fd9-4f1f-9741-1288b6e900f2)

![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/aa96f2be-a6b6-4957-8ce0-3cd13e00a075)

![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/c672fa08-a375-4072-80ba-0ee7259d6f06)

![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/a8d0a477-cf8c-4492-b6b3-a2372e0ec2d8)

- **conclusions related to the data visualization:**
- when focusing on 'workclass' feature, most of the data comes from private sector (around 75%).
- most of the data rows are for males (67%).
- 91% of the included data is from united states.
- most of the data target feature 'income' is <=50k (around 76%).
- 'white' and 'asian-pac-islander' races seems to have better chance in earning >50k.
- most of people earning >50k income relationship is either 'husband' or wife'.
- 'self-employed' and 'federal-gov' workclasses have better chance in earning >50k income.
- number of males taking >50k income is way higher than number of females.

# Results of RandomForest Classifier - base model:
- On the training data:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/f806f1f0-aa62-4d18-8716-5739ef949c00)
- On the testing data:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/6396aa03-fbdb-436c-84e1-e8f82869e6bf)

# Results of exploring the 10 most important features:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/37204d9d-8985-4652-8c17-d546054abeac)

# Results of repeating the same model using feature engineering - base model:
- On the training data:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/edb4bf0f-2f6f-4a57-8dcb-5dd33422e519)
- On the testing data:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/6f237c31-5581-482f-a47e-84b851e269e2)

# Repeating the same feature engineering model by applying feature selection meathod:
- On the training data:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/8963c5cb-0fbe-48b9-90aa-bc5def6cd541)
- On the testing data:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/4b8519df-a9d5-4b79-8fe9-c9529745348e)

# Results of applying neural network - base model:
![image](https://github.com/MoAlsayed/Machine-Learning---income-prediction-project/assets/144434790/11e8fb6d-65ab-4c89-9aad-6707957e368a)

# Final Consulsion:
- the best model was the one were feature selection method was implemented with estimated accuracy on both training and testing data sets equals to 86%.



