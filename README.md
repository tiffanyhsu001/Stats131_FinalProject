# Data Analysis: Food Choices of Students at Mercyhurst University
Tiffany Hsu, Susan Chen, Sam Aycock, Michelle Hsieh

# Background of Data
This data was collected by Bora Pajo during her time as an assistant professor at Mercyhurst University in Erie, Pennsylvania. She surveyed 126 students in 2017 regarding the students’ food and eating choices. The survey includes 60 questions where the students self-reported their habits, food preferences, income level, etc. We obtained the dataset from Kaggle: https://www.kaggle.com/borapajo/food-choices.

# Objective
What are the characteristics that define a student’s health consciousness?

# Variables Studied
See 'Food Variables Codebook.pdf'

### Sub Questions:
1. What types of students are best at guessing calories? (Caloric awareness)
   a. Compare students guessing abilities for chicken piadina
   b. Compare students guessing abilities for turkey BLT
2. What types of students will associate healthy foods over unhealthy ones? (Food choice association)
   a. Characteristics that define students who choose coke over OJ, vice versa
3. What types of students will eat out more? (Healthy vs. unhealthy eating habits)
   a. Characteristics that define students who eat out more often

# Analysis, Methods
Before performing any analysis, we created new variables calories_chicken_prop, which took initial variable calories_chicken (students guess for # of calories in chicken piadina) divided by the actual calories in a chicken piadina. This returns a proportion of "correctness" in guessing. The same process was done with calories_turkey to create calories_turkey_prop.

For each sub question, we included histograms, line plots, and correlations (biserial correlation for dichotomous variable) for initial exploratory analysis. To test the validity of initial claims from our graphs, we performed ANOVA tests to test for significant differences in the means between different variable levels. For our second sub question, which involved testing for the differences in proportions, we validated conclusions using Chi Square testing. 

# Results
Most of the studied variables in sub question 1 ended up being insignificant against a students caloric guessing ability, except for GPA with students guessing ability for turkey BLT.
In sub question 2, income & mother_education were statistically significant from Chi Square testing.
None of the selected variables were significant after performing ANOVA against eating_out habits.


# Conclusion
#### What types of students are best at guessing calories? (Caloric awareness)
Students with higher GPAs are better at guessing calories for the turkey sandwich 

##### What types of students will associate healthy foods over unhealthy ones? (Food choice association)
Female students are more likely to choose orange juice and check nutrition facts
Students with higher income & higher mother education associate drinks with coke more

#### What types of students will eat out more? (Healthy vs. unhealthy eating habits)
None of the studied variables can characterize students who eat out more.
