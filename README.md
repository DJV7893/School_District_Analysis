# School District Analysis
---
## Overview
---
### Purpose

  A school district has hired us to help analyze data in order to assist the school board and superintendent with making decisions regarding the school budgets and priorities. To do so we aggregated datasets from the school and district level related to student funding and standardized test scores, for both math and reading, in order to display school performance trends. This required us to install and use software and applications such as Anaconda, Jupyter Notebook, Pandas Library and Numpy Library. Our initial analysis produced the following deliverables:

  * A high-level snapshot of the district's key metrics, presented in a table format
  * An overview of the key metrics for each school, presented in a table format
  * Tables presenting each of the following metrics:
    * Top 5 and bottom 5 performing schools, based on the overall passing rate
    * The average math score received by students in each grade level at each school
    * The average reading score received by students in each grade level at each school
    * School performance based on the budget per student
    * School performance based on the school size 
    * School performance based on the type of school
 
  After we completed and submitted our initial analysis, the school board informed us that one of the original datasets we analyzed shows evidence of academic dishonesty. Specifically, the school board determined that the standardized test scores for the 9th grade of Thomas High School (THS) have been altered. We have been tasked with excluding those scores while keeping the rest of the data intact and repeating our analysis to gauge the changes in the overall analysis.

---
## Analysis
---
### Results

Our refactored analysis produced the following results:

  * The district summary was only slightly affected by the exclusion of the test scores. Only a couple of the key metrics were reduced by less than a tenth of a decimal point.

District Summary Old
<img width="922" alt="District_Summary_Old" src="https://user-images.githubusercontent.com/99817571/159043550-e42909ec-fab6-429e-9dc1-b443ed514962.png">  

District Summary New 
<img width="923" alt="District_Summary_New" src="https://user-images.githubusercontent.com/99817571/159043637-d40e5ce8-ee99-46c3-8622-c6879190e64e.png">

  * The school summary remained entirely the same even for THS after we removed the scores for its 9th graders and recalculated the high school’s performance metrics, which only took a slight dip in its performance metrics of less than .5 percentage point. 

School Summary Old
<img width="986" alt="School_Summary_Old" src="https://user-images.githubusercontent.com/99817571/159044056-1392eff3-4809-4b5c-8e3b-e6291646f51c.png">

School Summary New
<img width="986" alt="School_Summary_New" src="https://user-images.githubusercontent.com/99817571/159044101-ebe57bce-4ee1-4460-aab1-29bfeba93e22.png">

  * As a result, THS remained as the second best performing high schools in the district after we removed the scores for the 9th grade.

Top 5 Performing Schools Old
<img width="990" alt="Top_5_Performing_Old" src="https://user-images.githubusercontent.com/99817571/159044170-fbbbdb81-4305-47fa-a259-28aa9d479bb9.png">  

Top 5 Performing Schools New
<img width="988" alt="Top_5_Performing_New" src="https://user-images.githubusercontent.com/99817571/159044223-bd2e5a83-ebd6-4145-b4d5-944c60511cfe.png">

  * The removal of the 9th graders from THS impacted the following metrics as such:

    * The scores by grade for both math and reading for each high school remained the same except for the 9th grade of THS which is left as NaN.
Math Scores Old  
<img width="294" alt="Math_Scores_Old" src="https://user-images.githubusercontent.com/99817571/159044706-cff35cb4-f68e-4652-8ad4-afcd5c8e283a.png">       

Math Scores New
<img width="295" alt="Math_Scores_New" src="https://user-images.githubusercontent.com/99817571/159044933-02e495c4-3437-4fa3-a317-17929ea56e4c.png">

Reading Scores Old     
<img width="295" alt="Reading_Scores_Old" src="https://user-images.githubusercontent.com/99817571/159045378-9a8a7a51-ba79-4986-bdb7-76840e352477.png">  

Reading Scores New
<img width="296" alt="Reading_Scores_New" src="https://user-images.githubusercontent.com/99817571/159045403-e5b7b83e-767d-485b-a990-920b8d46a6f9.png">

  * The other three metrics of score by school spending, school size, and school type were all unaffected by the removal of the 9th grade scores from Thomas High School.
 
Scores by School Spending Old
<img width="815" alt="Scores_by_School_Spending_Old" src="https://user-images.githubusercontent.com/99817571/159045724-61f2db83-7bf6-41bd-a33e-1a635fc8d985.png">

Scores by School Spending New
<img width="817" alt="Scores_by_School_Spending_New" src="https://user-images.githubusercontent.com/99817571/159045736-36d7088c-9511-455a-90d8-8e1250dc151a.png">

Scores by School Size Old
<img width="750" alt="Scores_by_School_Size_Old" src="https://user-images.githubusercontent.com/99817571/159045768-4862506f-20d0-4fb7-9a46-894e2d0e0f0d.png">

Scores by School Size New
<img width="753" alt="Scores_by_School_Size_New" src="https://user-images.githubusercontent.com/99817571/159045789-370a0509-6c56-440f-8647-9378eb5ec485.png">

Scores by School Type Old
<img width="706" alt="Scores_by_School_Type_Old" src="https://user-images.githubusercontent.com/99817571/159045826-dd80a659-6190-458f-93f6-c9414c75c50e.png">

Scores by School Type New
<img width="705" alt="Scores_by_School_Type_New" src="https://user-images.githubusercontent.com/99817571/159045847-f7b85a05-e58a-4200-81ca-8cd893a54a6d.png">

---
## Summary
---
### Observations of Refactored School Data Set

The removal of the 9th graders standardized test scores from THS does not impact significantly the summaries at the school or district level. The four minor changes we can observe are in the district summary. The Average Math Score decreased from 79 to 78.9 percent. The Overall Passing Math Score decreased from 75 to 74.8 percent. The Overall Passing Reading Score decreased from 86 to 85.7 percent. The Overall Passing for both Math and Reading Scores decreased from 65 to 64.9 percent.

---
## Resources
---
Data Source: students_complete.csv, schools_complete.csv

Software: Anaconda 4.12.0, Jupyter Notebook, Python 3.7.6
