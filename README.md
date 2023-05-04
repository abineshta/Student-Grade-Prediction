# Student Grade Prediction
![16 Ways to Celebrate Your Star Student's Good Grades](https://fthmb.tqn.com/nlfwL1YDjA-H9cO-V2JddhtOsMk=/2001x1500/filters:fill(auto,1)/good-grades-rewards-57cc4f8c5f9b5829f40a4071.jpg)

## Objectives
- To perform necessary exploratory data analysis to know some interesting fact about the students in Portuguese school. 
- Finding out the factors contributed to the final grades of the students.
- Create a model using the decision tree regressor and create a decision tree out of it.
- Comparing the accuracy of model with multiple linear regressor. 
- Create a function that predicts the students grade according to the user input.
##  About the dataset
The Portuguese student prediction dataset is a collection of data about the academic performance of secondary school students in two subjects: Mathematics and Portuguese language. The dataset contains 33 attributes, including student grades, demographic, social and school-related features. The dataset was collected by using school reports and questionnaires.
## For whom?
- Educators
- Policy makers
- Researchers
## Attribute Information
1. school - student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)
2.  sex - student's sex (binary: 'F' - female or 'M' - male)
3.  age - student's age (numeric: from 15 to 22)
4.  address - student's home address type (binary: 'U' - urban or 'R' - rural)
5.  famsize - family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)
6.  Pstatus - parent's cohabitation status (binary: 'T' - living together or 'A' - apart)
7.  Medu - mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 â€“ 5th to 9th grade, 3 â€“ secondary education or 4 â€“ higher education)
8.  Fedu - father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 â€“ 5th to 9th grade, 3 â€“ secondary education or 4 â€“ higher education)
9.  Mjob - mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
10.  Fjob - father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
11.  reason - reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')
12.  guardian - student's guardian (nominal: 'mother', 'father' or 'other')
13.  traveltime - home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)
14.  studytime - weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)
15.  failures - number of past class failures (numeric: n if 1<=n<3, else 4)
16.  schoolsup - extra educational support (binary: yes or no)
17.  famsup - family educational support (binary: yes or no)
18.  paid - extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)
19.  activities - extra-curricular activities (binary: yes or no)
20.  nursery - attended nursery school (binary: yes or no)
21.  higher - wants to take higher education (binary: yes or no)
22.  internet - Internet access at home (binary: yes or no)
23.  romantic - with a romantic relationship (binary: yes or no)
24.  famrel - quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
25.  freetime - free time after school (numeric: from 1 - very low to 5 - very high)
26.  goout - going out with friends (numeric: from 1 - very low to 5 - very high)
27.  Dalc - workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
28.  Walc - weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
29.  health - current health status (numeric: from 1 - very bad to 5 - very good)
30.  absences - number of school absences (numeric: from 0 to 93)
31. G1 - first period grade (numeric: from 0 to 20)
32. G2 - second period grade (numeric: from 0 to 20)
33. G3 - final grade (numeric: from 0 to 20, output target)

#  Insights
-  The age of the kids does not matter to tell their intelligence. So, we must analyze further factors to know the triggers for good grades.

- The study timing of the students have affected the final grades but not very significantly. Although the highest grade is scored by a kid who studies more than ten hours a day, there are students who scored less marks compared to the one who studies less time.

- Most of the students who were failed at previous exams, were able to score less marks compared to the successful candidates in previous exams. However, the scores of successful candidate is not that great to be delighted. Only few people scored without failure above 18 marks. Overall, we can conclude that the school lacks bright students in academics.

- There is a positive correlation between the period exam grades and final exam grades. There are students who have improved their scores as well as decreased from their period exams. The difference between two grades is not that high. This shows that students have nailed in their consistency in their grades. The outliers in the might be the one's who failed to attend the final exams.

- On average boys have scored much higher than girls. Even the maximum scorer for this final exam is also a boy. On the other side girls have scored the lowest marks too. This result is little surprising for the school which has equally ditributed gender division. Althought the conclusion is told in a eagle's eye view, in actual result there is not much difference of marks between girls and boys.
- There is no proper correlation between the absenteeism and the final exam grades. This shows that even if students take some leave there is no much difference in their marks. LoL, surprisingly there students who have not even taken a single leave in their school life but scored very low marks. I hope these people do not come to study to school.

##  Modelling
Using this dataset, decision tree regressor model was performed. Another data frame was made that only contains the categorical columns, so that label encoder can be applied. The data frame was joined with the one that had all the numerical values. The data was finally splitted to create the testing and training data. From sklearn model tree the decision tree classifier was performed and then it was fitted to the training data. Predictions of both training and testing data was carried out. From sklearn.metrics the r2 score, mean squared error was imported to know the accuracy of the prediction. Minimum samples of 100 was taken to fit in the decision tree regressor. From sklearn the tree was imported and plotted the decision tree regressor. Multiple regression was also carried to check the accuracey of the predictions made. Finally, a function was created for any user who wish to predict whether the client will subscribe the term deposits.
## Conclusion
The training data for both decision tree regressor and multiple linear regression model the predicted values have higher accuracy compared to their testing data. If we look more closer in training data, multiple linear regression is producing more accurate data than decision tree regression model
## Evaluation performed
- Mean squared error
- R2 score
![Study: Students with Good Grades Are More Popular, Secure - Council for ...](https://www.cdacouncil.org/storage/CounciLINK/April_2019/STUDY_STUDENTS_WITH_GOOD_GRADES_ARE_MORE_POPULAR_SECURE.jpg)


