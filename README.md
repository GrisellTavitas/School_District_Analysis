# School_District_Analysis
Pandas

1. **Overview of the school district analysis:** Explain the purpose of this analysis.

In this module we helped Maria, who is a chief data scientist for a City School System; so we prepared all the school and student's standarize test scores, in order to show trends and school's performace and to give to the School Board and Superintendent the necessary information for them to take decisions regarding the school budgets and priorities.

After the genral summary that we had made during the module, the School Board notified Maria, they found some evidence of academic dishonesty, in reading and math grades for Thomas High School ninth graders, which seems to be alteraded.

So then we must replace the math and reading scores with "NaNs", but keeping the rest of the data for Thomas High School intact. After previously said, we'll see how these changes affected the overall analysis.

2. **Results**: Using bulleted lists and images of DataFrames as support, address the following questions.

  - How is the district summary affected?

On the initial results, we obteined the following outcomes:

![Outcomes before cleanup](https://user-images.githubusercontent.com/90433064/137658905-e68cd2e1-bf0c-46cd-8215-50907c16598c.png)

And these are the results after the cleanup on the data:

![Outcomes after cleanup](https://user-images.githubusercontent.com/90433064/137659002-755e4030-f946-4eba-8d44-38e8b9494c80.png)

As you can see, the parameter that affected was only the "School Type": Charter; since this is the parameter which Thomas Highschool belong. And actually overall results for the Charter School Type shows a tiny difference of .04 points of% Overall Passing affected by the modification on the results of THS. So then, the district summary was not affected by the incident of THS.

  - How is the school summary affected?

Even though the Thomas High School % Overall Passing, was affected by the deduction of the ninth grade performance; its overall results did not change that much, so it allow THS to mantein the second place of the top 5 schools, based on their % Overall Passing. Because of that  the order of the schools in that mentioned DF, kept the same order as well.

Outcomes before the incident:

![school_summary_1](https://user-images.githubusercontent.com/90433064/137666293-32871276-12e2-42de-971d-7d6753fd69ea.png)

Outcomes after the incident:

![school_summary_2](https://user-images.githubusercontent.com/90433064/137666324-970ae83f-7061-46e7-97df-02e0f2623b9f.png)

  - How does replacing the ninth graders??? math and reading scores affect Thomas High School???s performance relative to the other schools?

Since the % Overall Passing for THS from the beggining was good, at the end the ninth graders's score, did not affected its possition in compairs to the rest of the schools; because the difference from the first and the second outcome for % Overall Passing for THS was only .31 points, and the difference from its first outcome and the third place on the top 5 schools it was .35 points; that is why THS was able to mantain its position on the chart.

  - How does replacing the ninth-grade scores affect the following:
      - Math and reading scores by grade

As you can see on the DF on the first image,, the first result for math scores by grade for THS on the ninth grade, was placed as 83.6 and 83.7 for reading scores; but after the incident per the school board instruction, you can see that the score for the ninth grade on math and reading, its represented by the variable "nan":

![math_scores_by_grade_1](https://user-images.githubusercontent.com/90433064/137668728-f75e82be-bebd-484f-9d08-9f1f1e052014.png)

![math_scores_by_grade_2](https://user-images.githubusercontent.com/90433064/137668737-cc98e521-aa7a-402f-9de3-942c950a3256.png)

![reading_scores_by_grade_1](https://user-images.githubusercontent.com/90433064/137668750-d438a8c1-c48d-4daa-9cb2-9ab034e75d60.png)

![reading_scores_by_grade_2](https://user-images.githubusercontent.com/90433064/137668760-25b80a42-e4a9-465d-a2d6-0dacc58820ee.png)


      - Scores by school spending

Taking into account that THS is on the range from $630-$644, it's suppoused to be this range the one affected by the NaN variable: 

![school_spending_1](https://user-images.githubusercontent.com/90433064/137670127-917d82d1-1049-45a8-ba64-8158c9832ccb.png)

![school_spending_2](https://user-images.githubusercontent.com/90433064/137670135-2796ed4e-608a-43df-b2f1-dc0166aa8b7f.png)

As you can see only the reading scores were the unique value (besides the % passing reading) that grows up per decimals, from the rest were affected negativatly from -.01 to -.08 points by the incident.

      - Scores by school size

Having that THS belongs to the Medium size category:

![school_size_1](https://user-images.githubusercontent.com/90433064/137670144-fc1595ee-0a95-4b3b-a310-9cb50de0eb26.png)

![school_size_2](https://user-images.githubusercontent.com/90433064/137670155-c9082f16-801d-4d30-8e95-39ec486a2c3a.png)

We can see, that it happened the same than  for the spending analysis, the unique value that was affected in a positive way by +.01 points, it were the reading scores (besides the % passing reading).

      - Scores by school type
      
As we said previously, since the THS is part of the Charter type's school, we can determine that the district's scores did not received an affectation:
      
![school_type_1](https://user-images.githubusercontent.com/90433064/137670168-6e1c395a-52cb-48cc-b53c-eb6b86544c7d.png)

![school_type_2](https://user-images.githubusercontent.com/90433064/137670183-ae2f2a82-c9c2-4c93-8001-582a7ab6cd78.png)

We can mention as well, that in this case the positive affectation for the reading scores, is only for .005 points, from the first result and the one after the incident. 

3.- Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

So we can conclude that the ranges affected mainly were:

    - The % Overall Passing ofcourse related to the THS.
    - Reading scores for the range of $630-$644 on the spending analysis.
    - Reading scores for the range of Medium Size (1000-2000) on the size analysis.
    - Reading scores for the range of Charter Type on the type analysis.
