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
<img width="922" alt="District_Summary_Old" src="https://user-images.githubusercontent.com/99817571/159043550-e42909ec-fab6-429e-9dc1-b443ed514962.png"> District Summary New <img width="923" alt="District_Summary_New" src="https://user-images.githubusercontent.com/99817571/159043637-d40e5ce8-ee99-46c3-8622-c6879190e64e.png">


  * The school summary remained entirely the same even for Thomas High School after we removed the scores for its 9th graders and recalculated the high school’s performance metrics, which only took a slight dip in its performance metrics of less than .5 percentage point. 

  * As a result, Thomas High School remained as the second best performing high schools in the district after we removed the scores for the 9th grade.

  * The removal of the 9th graders impacted the following metrics as such:

    * The scores by grade for both math and reading for each high school remained the same except for the 9th grade of Thomas High School which has an empty of value of NaN

    * The other three metrics of score by school spending, school size, and school type were all unaffected by the removal of the 9th grade scores from Thomas High School.





