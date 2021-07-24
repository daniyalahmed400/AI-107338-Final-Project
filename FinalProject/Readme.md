# AI-107338-Final-Project
**Repository of AI Semester Final Project (Course Instructor: Syed Farooq Zaidi)**


### Members:
Student Name | Student ID
------------ | -------------
**Hafiz Daniyal Shakeel** | **64299**
**Anusha Iqbal** | **64011**
**Syed Muhammad Uzair** | **64239**

PREDICTIONS USING SVM AND KNN AND Classifiers

**OUR FINDINGS:**

![Screenshot (22)](https://user-images.githubusercontent.com/60693890/126153194-a0f30d50-1bc2-4405-9d74-134a749e444b.png)

![Screenshot (23)](https://user-images.githubusercontent.com/60693890/126153202-58dce7d9-0142-45c2-9452-45c0afe3ca59.png)

![Screenshot (24)](https://user-images.githubusercontent.com/60693890/126153203-ce5834fb-4289-4692-884c-b618b5bf1198.png)

![Screenshot (17)](https://user-images.githubusercontent.com/60693890/126153204-47d9543d-ab04-4aeb-b2fb-8d1cb559037c.png)

![Screenshot (18)](https://user-images.githubusercontent.com/60693890/126153209-0fab7a43-f6fb-44e6-b3b8-c7abbfb6b695.png)

![Screenshot (19)](https://user-images.githubusercontent.com/60693890/126153212-6436c34a-4bfb-4e18-a8c5-94d0aad4297c.png)

![Screenshot (20)](https://user-images.githubusercontent.com/60693890/126153216-0d7253da-2ce9-4845-969e-bb68b8d71bd3.png)

Introduction
The goal of the project was to predict the survival of passengers based off a set of 
data. We used Kaggle competition "Titanic: Machine Learning from Disaster" (see 
https://www.kaggle.com/c/titanic/data) to retrieve necessary data and evaluate 
accuracy of our predictions. The historical data has been split into two groups, a 
'training set' and a 'test set'. For the training set, we are provided with the outcome 
(whether or not a passenger survived). We used this set to build our model to 
generate predictions for the test set.
For each passenger in the test set, we had to predict whether or not they survived 
the sinking. Our score was the percentage of correctly predictions. 
In our work, we learned
 Programming language Python and its libraries NumPy (to perform matrix 
operations) and SciKit-Learn (to apply machine learning algorithms)
 Several machine learning algorithms (decision tree, random forests, extra 
trees, linear regression)
 Feature Engineering techniques.
Work Plan
1. Learn programming language Python
2. Learn Shennon Entropy and write Python code to compute Shennon 
Entropy
3. Get familiar with Kaggle project and try using Pivot Tables in Microsoft 
Excel to analyze the data.
4. Learn to use SciKit-Learn library in Python, including
a. Building decision tree
b. Building Random Forests
c. Building ExtraTrees
d. Using Linear Regression algorithm
5. Performing Feature Engineering, applying machine learning algorithms, and 
analyzing results

Training and Test Data
Training and Test data come in CSV file and contain the following fields:
 Passenger ID
 Passenger Class
 Name
 Sex
 Age
 Number of passenger's siblings and spouses on board
 Number of passenger's parents and children on board
 Ticket
 Fare
 Cabin
 City where passenger embarked

Feature Engineering
Since the data can have missing fields, incomplete fields, or fields containing hidden 
information, a crucial step in building any prediction system is Feature Engineering. 
For instance, the fields Age, Fare, and Embarked in the training and test data, had 
missing values that had to be filled in. The field Name while being useless itself, 
contained passenger's Title (Mr., Mrs., etc.), we also used passenger's surname to 
distinguish families on board of Titanic. Below is the list of all changes that has been 
made to the data.
Extracting Title from Name
The field Name in the training and test data has the form "Braund, Mr. Owen 
Harris". Since name is unique for each passenger, it is not useful for our prediction 
system. However, a passenger's title can be extracted from his or her name. We 
found 10 titles:
Index Title Number of occurrences
0 Col. 4
1 Dr. 8
2 Lady 4
3 Master 61
4 Miss 262
5 Mr. 757
6 Mrs. 198
7 Ms. 2
8 Rev. 8
9 Sir 5
We can see that title may indicate passenger's sex (Mr. vs Mrs.), class (Lady vs 
Mrs.), age (Master vs Mr.), profession (Col., Dr., and Rev.).
Calculating Family Size
It seems advantageous to calculate family size as follows
Family_Size = Parents_Children + Siblings_Spouses + 1

Conclusion
As a result of our work, we gained valuable experience of building prediction 
systems and achieved our best score on Kaggle: 80.383% of correct predictions (in 
Kaggle leaderboard, it corresponds to positions 477 - 881 out of 3911 participants).
• We performed featured engineering techniques 
• Changed alphabetic values to numeric
• Calculated family size
• Extracted title from name and deck label from ticket number
• Used linear regression algorithm to fill in missing ages
• We used several prediction algorithms in python
• Decision tree
• Random forests
• Extra trees
• We achieved our best score 80.383% correct predictions

