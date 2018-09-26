# Titanic Survivor Analysis and Prediction

## Dataset
This is th first dataset I explored on Kaggle platform.   
Dataset is available here:
https://www.kaggle.com/c/titanic/data

Survived column indicates if the passenger survived (1) or not (0), it is not a highly skewed dataset. It has several categorical as well as continuous numerical columns as input variable. 

## Analysis, model building and conclusion
Trends of different parameters with survival of the passengers are explored with groupby summary tables, distribution and correlation plots. Final input parameters for model building are: Pclass, Sex, Age,	Fare, Embarked,	Title,	isAlone,	Age x Class where all are numerical categorical parameters. Other parameters are ignored. Titles (Mr. Mrs. etc) are derived from ech person's name. isAlone defines if the person boarded alone without family member or sibling. Age x Class is a cross term introduced in the dataset. Based on Random Forest variable importance on training dataset, top three parameters driving the survival are title, ses and passenger class. Among the models compared, tree based models: Random Forest and Decision Tree gave the highest test accuracy of 86.64%.  
Accuracy obtained on the competition dataset (not shown) were 76%. There is more room to improve variance in the model to match the accuracies. 
