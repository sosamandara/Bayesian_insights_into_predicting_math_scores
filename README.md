# Bayesian_insights_into_predicting_math_scores

It appears that there may be some errors in the PDF document provided in the README file. These errors may be attributed to the fact that the original file was in HTML format.
If possible take a look of the html file 'math_score'.

## Brief Introduction
The major objective of this project is to construct a regression model that makes use of Bayesian inference to forecast results in mathematics depending on available factors. Understanding the variables that affect arithmetic performance can give educators and decision-makers new perspectives on how to raise student achievement

Why this study can be helpful:

- Math score predictions can offer insightful information about a student’s academic achievement, according to the *Academic achievement Assessment*. It enables teachers to recognise kids who might require more assistance or resources in mathematics and to design interventions accordingly.

- *Identifying Influential elements*: Examining the correlation between math test results and different demographic and academic variables can aid in determining which elements have the greatest influence on a student’s success. This knowledge can direct educational initiatives and policies aimed at enhancing math instruction.

## The data set

The dataset consists of the following variables:

- *Gender*: Categorical variable indicating the gender of the student.

- *Race/Ethnicity*: Categorical variable representing the race or ethnicity of the student.

- *Parental Level of Education*: Categorical variable indicating the highest level of education attained by the student’s parents.

- *Lunch*: Categorical variable indicating whether the student receives free/reduced lunch or standard lunch.

- *Test Preparation Course*: Categorical variable indicating whether the student completed a test preparation course.

- *Reading Score*: Numerical variable representing the score obtained by the student in the reading subject.

- *Writing Score*: Numerical variable representing the score obtained by the student in the writing subject.

- *Math Score*: Numerical variable representing the target variable, the score obtained by the student in the math subject.

Some plots for the Exploratory Data Analysis
|       |       | 
:-------------------------:|:-------------------------: 
<img width="485" alt="plot1" src="https://user-images.githubusercontent.com/113529675/271363258-a6718f0f-454a-4d0d-b8c9-9d581a6e537a.png"> | <img width="485" alt="plot2" src="https://user-images.githubusercontent.com/113529675/271363384-7c15c59a-c829-4dd7-82d9-16b6df787a95.png">

The scatter plots between the Math Score (target variable) and the Writing Score, as well as the Reading Score, clearly demonstrate a strong positive correlation. This correlation can be observed from the overall upward trend in the scatter plots, as well as the fitted regression lines that show a positive slope.

<img width="400" alt="plot3" src="https://user-images.githubusercontent.com/113529675/271363431-212d17f9-ec51-46cc-80ba-82fcf13b0a7f.png"> | <img width="400" alt="plot4" src="https://user-images.githubusercontent.com/113529675/271363493-b469ec03-142d-41b9-b9c8-ab50f8beb45c.png">

See the `math_score.pdf` file for a deeper analysis.

## The models 

In the `math_score.rmd` file you can find the bayesian analysis (complete of convergence analysis of the MCMC).
By examining the relationship between the Math Score and the predictors, we can estimate the model coefficients and make predictions on the Math Score for new observations.

Traceplots and posterior distributions can be examined to determine the reliability of MCMC samples. These graphs offer useful details about the convergence and behaviour of the MCMC chain.

To ensure the accuracy of the posterior estimates, it was essential to evaluate the convergence of MCMC samples. The Geweke diagnostic, which compares the means of the early and late regions of the Markov chain, is one often used diagnostic technique, and we opted for that.

By calculating the auto-correlation at various lags, we were able to determine the level of independence between MCMC samples.

# Used technologies

![RStudio](https://img.shields.io/badge/RStudio-4285F4?style=for-the-badge&logo=rstudio&logoColor=white)
![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white)

