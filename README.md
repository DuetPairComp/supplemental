## Supplemental Materials for "Duet: Helping Data Analysis Novices Conduct Pairwise Comparisons by Minimal Specification"

### Contents

[Links to Videos Introducing Duet’s User Interface](#links-to-videos-introducing-duets-user-interface)
 
[Link to the System](#link-to-the-system)

[Explanations for the “Logistic Regression” Folder](#explanations-for-the-logistic-regression-folder) 

[Explanations for the “User Study” Folder](#explanations-for-the-user-study-folder) 

[Clarification of Literature Review](#clarification-of-literature-review)  

---

### Links to Videos Introducing Duet’s User Interface

Tutorial Video Used in the User Study: [Link](https://youtu.be/JF8Q-PT3xUY)

Analyzing US College Scorecard Data Using Duet: [Link](https://youtu.be/Y4p0h8_EnDU)

---

### Link to the System

Duet’s prototype: [Link](https://duetpaircomp.github.io/)

***README:***  
*1. Use Google Chrome for better experience.*  
*2. Some datasets are provided in the “[Datasets](https://github.com/DuetPairComp/supplemental/tree/master/Datasets)” folder for trying out the system.*

---

### Explanations for the “Logistic Regression” Folder

In the following, we explain the materials in the “Logistic Regression” folder. The “[Logistic Regression](https://github.com/DuetPairComp/supplemental/tree/master/Logistic%20Regression)” folder provides details for the model in Sec. 5.3.2 (Multinomial Logistic Regression for Classification) of the paper.

1. [520 Distribution Pairs](https://github.com/DuetPairComp/supplemental/tree/master/Logistic%20Regression/520%20Distribution%20Pairs)

This folder contains 520 distributions pairs we collected from the 83 [R datasets](https://vincentarelbundock.github.io/Rdatasets/datasets.html). Each row in a csv file is a data point. There are three important columns in each csv file: “newGroupName”, “newAttributeName” and, “attributeValue”. “newGroupName” is the name of the group to which a data point belongs, “newAttributeName” is the name of an attribute. “attributeValue” is the value that a data point has for the attribute.

2. [Bh Coefficient + Labels.csv](https://github.com/DuetPairComp/supplemental/blob/master/Logistic%20Regression/Bh%20Coefficient%20%2B%20Labels.csv)

We used [SPSS](https://www.ibm.com/analytics/spss-statistics-software) to model the data. This csv file is the input to SPSS for modelling. The “fileName” column is the file name of a distribution pair inside the “[520 Distribution Pairs](https://github.com/DuetPairComp/supplemental/tree/master/Logistic%20Regression/520%20Distribution%20Pairs)” folder. “BhCoefficicent” is the [Bhattacharyya coefficient](https://en.wikipedia.org/wiki/Bhattacharyya_distance) for a distribution pair and “class” is the label of distribution pair we collected from people.

3. [Code for Relabelling 150 Marginal Cases](https://github.com/DuetPairComp/supplemental/tree/master/Logistic%20Regression/Code%20for%20Relabelling%20150%20Marginal%20Cases)

It is the code of the interface we used for asking 10 subjects to relabel 150 marginal cases. You need Python 3 and [Flask](http://flask.pocoo.org/) to run the interface. To run the code, go to the directory using the
console if you are using a Mac and enter *“python server.py”*. For those who have difficulties running the tool, we provide the screenshots of the labelling tool as follows:

<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel1.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel2.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel3.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel4.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel5.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel6.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/relabel7.png" width="550"/>

4. [Data Collected From Relabelling](https://github.com/DuetPairComp/supplemental/tree/master/Logistic%20Regression/Data%20Collected%20From%20Relabelling)

Each csv file in the folder contains two columns: “filename” that is the file name of a distribution pair in the “[520 Distribution Pairs](https://github.com/DuetPairComp/supplemental/tree/master/Logistic%20Regression/520%20Distribution%20Pairs)” folder and “class” that is the label provided by a subject.

5. [SPSS Modelling Result](https://github.com/DuetPairComp/supplemental/blob/master/Logistic%20Regression/SPSS%20Modelling%20Result.png)

It is the screenshot of the output generated by SPSS. “[Bh Coefficient + Labels.csv](https://github.com/DuetPairComp/supplemental/blob/master/Logistic%20Regression/Bh%20Coefficient%20%2B%20Labels.csv)” is used as the input to SPSS. The following explains how the model in Sec. 5.3.2 corresponds to the SPSS output. Formally, our logistic regression model is

6. [R Code for Computing Model Accuracy.txt](https://github.com/DuetPairComp/supplemental/blob/master/Logistic%20Regression/R%20Code%20for%20Computing%20Model%20Accuracy.txt)

This text file contains the R code for computing the cross-validation accuracy of our logistic regression model using 10-fold cross validation. The input file is “[Bh Coefficient + Labels.csv](https://github.com/DuetPairComp/supplemental/blob/master/Logistic%20Regression/Bh%20Coefficient%20%2B%20Labels.csv)”. The cross-validation accuracy is around 78.1%. We envision that this accuracy can be improved by using more advanced machine learning models and more predictor variables.

<img src="https://s3.us-east-2.amazonaws.com/github-duet/model.png" width="550"/>

---

### Explanations for the “User Study” Folder

The “[User Study](https://github.com/DuetPairComp/supplemental/tree/master/User%20Study)” folder contains all the materials for the qualitative user study in Sec. 6
(Evaluation) of the paper. The materials inside are described as follows:

1. [Training Session](https://github.com/DuetPairComp/supplemental/tree/master/User%20Study/Training%20Session)

This folder contains the car dataset “[cars.csv](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Training%20Session/cars.csv)” we used for the training session, a link to the [tutorial video](https://youtu.be/JF8Q-PT3xUY) we showed to the participants and the training tasks to get participants familiar with Duet’s interface.

2. [Analysis Session](https://github.com/DuetPairComp/supplemental/tree/master/User%20Study/Analysis%20Session)

During each analysis session, we first showed the participants “[Task Description.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Analysis%20Session/Task%20Description.pdf)”. We then gave them some time to review either “[Description for College Dataset.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Analysis%20Session/Description%20for%20College%20Dataset.pdf)” or “[Description for City Dataset.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Analysis%20Session/Description%20for%20City%20Dataset.pdf)” to get them familiar with the dataset they were about to analyze. The “[Datasets](https://github.com/DuetPairComp/supplemental/tree/master/User%20Study/Analysis%20Session/Datasets)” folder contains the [city dataset](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Analysis%20Session/Datasets/cities.csv) and the [college dataset](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Analysis%20Session/Datasets/colleges.csv) we used for the analysis session.

3. [Interview and Survey](https://github.com/DuetPairComp/supplemental/tree/master/User%20Study/Interview%20and%20Survey)

At the end of the study, we first showed them “[Three Main Features of the Tool.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Interview%20and%20Survey/Three%20Main%20Features%20of%20the%20Tool.pdf)” to ensure the participants know the terminology like “minimal specification” we are going to use in the interview. This folder contains the questions for the semi-structured interview (“[Interview Questions.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Interview%20and%20Survey/Interview%20Questions.pdf)”) and the survey questions (“[Survey Questions.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Interview%20and%20Survey/Survey%20Questions.pdf)”).

4. [Questionnaire Results.pdf](https://github.com/DuetPairComp/supplemental/blob/master/User%20Study/Questionnaire%20Results.pdf)

It is a summary of the survey result.

---

### Clarification of Literature Review

We drew inspiration from the literature to develop the idea of minimal specification. As described in the paper, there are two high-level considerations in designing minimal specification:

1. To address **execution barriers**, minimal specification allows users to focus on what they know (the objects of interest in answering a pairwise comparison question) rather than what they might not know (system operations).

2. To address **interpretation barriers**, the recommendations offered should be explained in order to result in better understanding of the recommendations and stronger feeling of trust.

The following two sections describes the basis of these two components.

***Addressing Execution Barrier***

This idea of allowing users to focus on what they know by shielding them from what they might not know is grounded in the following three ideas that have been explored by the HCI community:

<img src="https://s3.us-east-2.amazonaws.com/github-duet/clarify1.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/clarify2.png" width="550"/>
<img src="https://s3.us-east-2.amazonaws.com/github-duet/clarify3.png" width="550"/>

***Addressing Interpretation Barrier***

Explaining the recommendations help users understand why they are recommended and inspire users’ trust in the system. This idea is grounded in the movement of explainable artificial intelligence (XAI).

<img src="https://s3.us-east-2.amazonaws.com/github-duet/clarify4.png" width="550"/>
