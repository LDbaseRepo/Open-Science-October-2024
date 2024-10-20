![Open Science October 2024 - Week 3 Banner](https://github.com/user-attachments/assets/1da54f7a-96cd-4b6f-86d3-c226130f487f)

# Week 3 - Math Anxiety and Attitudes
Week 3 of #OpenScienceOctober features the [MU Math Study Agebra/Math Anxiety Dataset](https://ldbase.org/datasets/7e729b59-761d-4332-a468-d7b86e0ceaa8) from the [MU Math Study Team at the University of Missouri](https://mumathstudy.missouri.edu/)!

# Project Description
This week's data sets come from a larger ongoing study focused on predicting student success in algebra. The project highlighted here focused specifically on understanding sex differences in the relationships among math anxiety, attitudes, and achievement in a sample of middle school students. The 6th grade data include over 1,000 students and feature summary variables reflecting different aspects of mathematics anxiety, attitudes towards math and English, and a standardized math competence score. The 7th grade data set includes similar variables for a subset of 190 students who were also assessed in 7th grade. 

Fun Fact: This project shows off a cool feature of LDbase - linking to data stored elsewhere! Creating a project on LDbase that contains a link to your data allows you to share your project wherever makes the most sense for your team, while still taking advantage of LDbase's community and metadata terms to enhance findability for researchers studying learning and development.

## Papers Associated with Dataset
**Citation**: Geary, D. C., Hoard, M. K., Nugent, L., Chu, F., Scofield, J. E., & Ferguson Hibbard, D. (2019). Sex differences in mathematics anxiety and attitudes: Concurrent and longitudinal relations to mathematical competence.Journal of Educational Psychology, 111(8), 1447–1461. https://doi.org/10.1037/edu0000355 
**Link**: [https://psycnet.apa.org/fulltext/2019-12585-001.html](https://psycnet.apa.org/fulltext/2019-12585-001.html)   
**Additional Publications Associated with this Project**: [https://mumathstudy.missouri.edu/publications.html](https://mumathstudy.missouri.edu/publications.html)

# Dataset
**Link to the Dataset**: [Dataset Link](https://ldbase.org/datasets/7e729b59-761d-4332-a468-d7b86e0ceaa8)  
  
**NOTES ABOUT THE DATASET**:
- This is an example of an LDbase project page that is linked to OSF. Click the OSF link under "External Resource" to access the datasets and codebooks for this week's challenge.
- The codebooks shared below contain SAS syntax for reading in and naming the variables. For R users, please see the bottom of this page for syntax you could use to similarly read in and label the variables.
- There are two data sets shared for this project: one for the full sample of 1,091 students assessed in 6th grade, and another for the subset of 190 students who were followed longitudinally. Note that the 6th grade data set includes only the variables assessed in 6th grade, whereas the 7th grade data set includes data for the subset of students at both the 6th and 7th grade timepoints.
- In both data sets, participant sex is coded as 1 = Male and 0 = Female.

# Codebooks
**Link to the 6th Grade Data Set Codebook**: [OSF Codebook Link](https://osf.io/6npuk)  
**Link to the 7th Grade Data Set Codebook**: [OSF Codebook Link](https://osf.io/6tyfa) 

# How do I participate?
-  Take a look at the data and keep an eye out for interesting relationships. Remember, be careful about drawing conclusions about causation!
   -  Take a look at the free resource [R for Data Science](https://r4ds.hadley.nz/) if you need some help
- **Make a data visualization!**
- **Share** your data viz on [Twitter](https://twitter.com/LDbaseRepo), [LinkedIn](https://www.linkedin.com/company/ldbaserepo/?viewAsMember=true), or [Instagram](https://www.instagram.com/ldbaserepo/) using the hashtags **#OpenScienceOctober**, **#DataSharingIsntSpooky**, and tag LDbase **@LDbaseRepo**!

# Citation
*You can also access this citation from the "Get Citation" link on the sidebar of the Project page, Dataset, and Codebook!* 
Geary, D. C., Scofield, J. E., & Hoard, M. K. (2023). *Sex Differences in Mathematics Anxiety and Attitudes.*https://doi.org/10.1037/edu0000355

# Supplemental R Syntax
dat6th <- read.table("MathAnxSixth.csv") # Read in data file for 6th grade
dat7th <- read.table("MathAnxSeventh.csv") # Read in data file for 7th grade

colnames(dat6th) <- c("ID", "Sex", "School", "MathStan_6s", "EAttMn_6", "MAttMn_6", "MAnxEval_6", "MAnxLearn_6")
colnames(dat7th) <- c("ID", "Sex", "MathStan_6s", "EAttMn_6", "MAttMn_6", "MAnxEval_6", "MAnxLearn_6",
                      "NO_SS_7", "EAttMn_7", "MAttMn_7", "MAnxEval_6_dup", "MAnxLearn_7", "IQ_7", "WR_SS_7", "JLAP_7")
