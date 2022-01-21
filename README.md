# School_District_Analysis

## Overview

The purpose of this analysis is to use district, school, and student data to provide insight about performance trends and patterns to inform discussions and strategic decisions at the school and district level. We look at various data including the school's budget, school type, student's standardized math and reading scores, and student's classification. We aggregate different datasets to analyze trends in school's performance. We are informed about the academic dishonesty in our data with Thomas High School's ninth grade class and their standardized test scores and update our analysis accordingly by nulling their scores. In this analysis we are using Python 3.9.7, Jupyter Notebook 6.4.5, and Conda 4.10.3.


## Results

### How is the district summary affected?

For our district summary, the columns "Total Schools", "Total Students", "Total Budget", "Average Math Scores", and "Average Reading Scores" were not affected. When changing Thomas High School's ninth grade scores, we notice it affected the columns "% Passing Math" from 75.0% to 74.8%, "% Passing Reading" from 85.8% to 85.7%, and "% Overall Passing" from 65.2% to 64.9%. 

![old_district_summary]("images/district_summary_old.png")
![new_district_summary]("images/district_summary_new.png")

### How is the school summary affected?

For our school summary, the columns "School Type", "Total Students", "Total School Budget", and "Per Student Budget" were not affected. When changing Thomas High School's ninth grade scores, it affected the columns "Average Math Scores" from 83.42% to 83.35%, "Average Reading Score" from 83.85% to 83.90%, "% Passing Math" from 93.27% to 93.19%, "% Passing Reading" from 97.31% to 97.02%, and "% Overall Passing" from 90.95% to 90.63%.

![ths_school_summary_old]("images/ths_school_summary_old.png")
![ths_school_summary_new]("images/ths_school_summary_new.png")

### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?

Although Thomas High School's ninth grade scores were ommitted from the overall analysis, it did not change the overall performance compared to other schools in the district. Thomas High School still ranks second in "% Overall Passing".

![top_five_old]("images/top_five_old.png")
![top_five_new]("images/top_five_new.png")

### How does replacing the ninth-grade scores affect the following:

- Math and reading scores by grade

For both math and reading scores, the 9th grade scores are replaced with `NaN` for Thomas High School because we changed their scores to `NaN`.

![math_school_old]("images/math_school_old.png")
![math_school_new]("images/math_school_new.png")
![reading_school_old]("images/reading_school_old.png")
![reading_school_new]("images/reading_school_new.png")

- Scores by school spending

Thomas High School spends about $638 per student, so we see that there was little change in all the columns on the Spending Summary data frame. We see that "Average Math Score" changed from 78.52% to 78.50%, "Average Reading Score" changed from 81.62% to 81.64%, "% Passing Math" changed from 73.48% to 73.46%, "% Passing Reading" changed from 84.39% to 84.32%, and "% Overall Passing" changed from 62.86% to 62.78%.

![per_student_old]("images/per_student_old.png")
![per_student_new]("images/per_student_new.png")

- Scores by school size

Thomas High School has 1,635 students, so it is considered a medium-sized school by the district. We see that there was little change in all the columns on the Size Summary data frame. We see that "Average Math Score" changed from 83.37% to 83.36%, "Average Reading Score" changed from 83.86% to 83.87%, "% Passing Math" changed from 93.60% to 93.58%, "% Passing Reading" changed from 96.79% to 96.73%, and "% Overall Passing" changed from 90.62% to 90.56%.

![school_size_old]("images/school_size_old.png")
![school_size_new]("images/school_size_new.png")

- Scores by school type

Thomas High School is a charter school, so we see that there was even smaller change in all the columns on the Type Summary data frame. We see that "Average Math Score" changed from 83.474% to 83.465%, "Average Reading Score" changed from 83.896% to 83.902%, "% Passing Math" changed from 93.621% to 93.610%, "% Passing Reading" changed from 96.59% to 96.550%, and "% Overall Passing" changed from 90.432% to 90.393%.

![school_type_old]("images/school_type_old.png")
![school_type_new]("images/school_type_new.png")

## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

After ommitting the reading and math scores for the 9th grade class of Thomas High School, we see that there is a major change in percentages in the school level. When the school data is aggragated in the school size data frame, we still see some change in the metrics, but it is not as noticeable at the school level. When we aggregate the data in the school type, we see very little change in the metrics. We see that the difference is in the hundreths and thousandth's place. In the overall district summary, the changes in metrics is negligible and does not really affect the metrics.