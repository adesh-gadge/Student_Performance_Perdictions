# Student Performance Predictions using Ordinal Regression, ANN and Random Forest
A kaggle dataset on student academic performance (available through https://www.kaggle.com/aljarah/xAPI-Edu-Data and also included as the attachment in this instruction) is gathered to identify the influential factors for students’ performance. To predict the students’ performance, the collected data was organized into four kinds of features: demographic, academic background, parents’ participation on learning process and behavioral features. The demographic features consisted of demographic details of the students like gender, nationality, place of birth etc. The section, grades and semester details of the students were included under the academic features and behavioral features consisted of fields demonstrating students’ engagement with the learning management system like viewed announcements, interaction with discussion groups, resources etc. To analyze the students’ performance, the target “Class” attribute was discretized into orindal values based upon students’ grades. Hence, we had three categories of student classes: High/H, Low/L and Medium/M.

* Here I compared performance of different algorithms performance on this ordinal classification problem.
<br/>
### 1. Ordinal Logistic Regression:
  The categorical variables like TopicEnglish can be interpreted as: a student with topic Eng, as opposed to a base Topic student, is associated with a higher likelihood of having a higher performance. The t-value is greater than 2 and therefore is statistically significant at the 5% level
The continuous variables like raised hands can be interpreted as : with one unit increase in raisedhands the log of odds of having a higher student performance increases by 0.73924
Intercepts:
L|M: Log of odds of having student performance ‘Low’ versus having student performance ‘Medium’ or ‘High’ = 2.5881
M|H: Log of odds of having student performance ‘Medium’ versus having student performance ‘High’ = 9.1711
<br/>
### 2. Artificial Neural Network:
<br/>
#### Before regularization:
![before regularization](https://github.com/adesh-gadge/Student_Performance_Predictions/blob/master/Before_regularizations.png)
<br/>
#### After regularization:
![after regularization](https://github.com/adesh-gadge/Student_Performance_Predictions/blob/master/after_regulatization.png)
<br/>
### 3. Random Forest Classifier:
<br/>
#### Feature importance according to Random Forest
![feature importance](https://github.com/adesh-gadge/Student_Performance_Predictions/blob/master/random_forest_importance.PNG) 
<br/>
## Model Comparison:
<br/>
**Highest Accuracy:** random forest could achieve the highest accuracy, of around 76%(test accuracy),compared to the other two models, neural networks did come close to 75% but neural networks require lots of data to become very good.
<br/>
**Faster Running speeds:** The logsitic regression is the fastest to run because it doesn’t have many parameters to learn, As compared to neural network which takes the longest to train and random forest is in-between.
<br/>
Code, results and interpretations are in the document file attached.




