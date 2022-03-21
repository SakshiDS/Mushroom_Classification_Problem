# Final-Project

## Mushroom Classification: Determining whether a mushroom is poisonous or edible
*Sakshi and Abbie*

*Presented on March 9, 2022*

## Link to presentation
https://docs.google.com/presentation/d/1X5cE83nUAi4FVP8rXjQyWnQ9bt47O6GV9KAN8dsO5Bg/edit?usp=sharing 

## How to Navigate this Repo:
This repo is organized into 3 primary deliverables
1. ETL code, entitled "Mushroom_ETL"
2. Exploratory Analysis, entitled "Part1_Mushroom-Exploratory-Analysis"
3. Data Models, entitled "Part2_Mushroom-Models"

Please note: It is advised to view "Part1" before "Part2"

The "codebook" for our data set is also included in this repo, for anyone interested in additional detail. 

## Data Science Techniques Utilized in this Project:
1. Logistic Regression
2. KNN
3. SVM Classification
4. Random Forest

## Data Model
![mushroom data model (5)](https://user-images.githubusercontent.com/90784468/157198105-8e299299-b375-4330-aa79-e1b893a4e3bd.png)

## Findings from our Project:
If you have any doubt whether a mushroom is poisonous or edible, you might just need to do a "sniff" test! If the odor is unpleasant, it is almost certainly poisonous. Otherwise, the mushroom is likely safe to eat.

To determine this, we computed 4 different classification models, each with their own tuning methods applied. We split our data into training (70%) and testing (30%) sets. We fit our model to the training data and evaluated the model on our testing data. Using these methods, we achieved extremely high accuracy with every model. More details below.

**Which model was the best?**

Every model we tested had extremely high performance. Therefore, we were able to select the "best of the best." The Random Forest Model and the SVM Model both performed equally well, with accuracy of 99% and AUC score of 99.91%. However, because Random Forest is an ensemble method (which helps guard against overfitting) we can select that as our best model.

**How we determined which model is the best.**

There are several ways to evaluate a classification model's performance, such as:

Precision/Recall
Accuracy score
AUC score
Considering all these parameters we evaluated our models accordingly. Because each individual metric was so high, we selected the most superior model based on the highest overall accuracy score, as well as the AUC score. This left the Random Forest and the SVM. We selected the Random Forest, as it is an ensemble learning method, which means it is less likely to overfit.

*For more details, please refer to Part2 notebook in this repo


## Our data source

Link to UCI repository:

https://mushroom.mathematik.uni-marburg.de/files/data/data/ - UCI

https://www.kaggle.com/uciml/mushroom-classification?select=mushrooms.csv - Kaggle
