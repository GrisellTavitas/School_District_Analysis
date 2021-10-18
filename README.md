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
  - How does replacing the ninth graders’ math and reading scores affect Thomas High    School’s performance relative to the other schools?
  - How does replacing the ninth-grade scores affect the following:
      - Math and reading scores by grade
      - Scores by school spending
      - Scores by school size
      - Scores by school type

3.- Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
