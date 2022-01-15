# School_District_Analysis

## Purpose of Analysis
    In this excercise, we are being asked to alter the data from its original state after being informed that a certain portion of test takers cheated.  We are meant to update the grades of these students and then preform the same analysis we originally conducted. Ultimately, comparing the two results to see how the change in data affected the outcomes.

# Results of the Compared Analyses 

## 1. School District Analyses Comparison 
    When comparing the results of the original data with the updated data, where we eliminated the cheating student's grades, we found the the overall data matched fairly similarly to our original report.  For the most part we saw roughly a .02% drop in performance between the original school district Analysis and the updated report (see images below for comparison).  
    This isn't very surprising when considering the small portion of students that were removed (461) from the total number of students in the data (39,170).  The cheaters represnt just a little more than 1% of the total popuraltion, so removing them from the data shouldn't change the data too drastically.  The exceptions would be if the entire grade 9th grade of Thomas High School was scoring signficatnly higher or significantly lower than the rest of the population.  The law of averages would suggest that this is highly unlikely and the results of our analysis confirm the hypothsis. 

### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********

## 2.  Per School Summary Analyses Comparison
    Comparing the results of the Analyses between the per school summary we see the first significant shift in performance for Thomas High School.  While we only lost a small subset of data in the Total School District Analysis, roguhly 1%. 
    In comparison when we look at the 9th grade data loss that impact Thomas Middle School, specifically that percetnage of data loss jumps from just over 1% to 28%. We see an average of roughly 26 percent being lost across the board for our recalculated metrics in % Passing Math, % Passing Reading & Overall % Passing.  
    Losing a little more than a quarter of your scoring data for the school we expect to see more drastic changes, as seen in the images below. However, after reviewing the significance of that change in caluclation, we resolve to remove the 9th graders from the count of students amongst Thomas High School population, which will result in a more accurate representation of those students who preformed faily in the testing process.   

### Original Analysis
            *********OLD IMGAGE INSERT**********

### Mid-point Results



### Updated Analysis
            *********NEW IMGAGE INSERT**********


## 3. Top Prefroming Schools
    Moving into the Top Preforming schools we return to the scenario we saw intitially between the School District Analysis.  In the images below you see the updated performance metrics return to the within .1% of original perfromance metrics that we ran.  


### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********



## 4. Bottom Prefroming Schools
    The Bottom preforming schools saw no real impact from our updated analysis.  Since the student at these schools did not have any updates to their scores as Thomas High School did.  The results are identical. 
### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********


## 5. Average Math by Grade
     In the Average Math Grades analyses we see the first instance of "nan" appear in one of our summary report outputs.  Having successfully replaced the 9th grade Thomas High School students with the "nan" value; we see the output in our updated summary.  Which is the only change between the two reports.  Since no other school or grade has had updated values the scores and outputs are identical the original output we created; as seen below.
### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********

## 6. Average Reading by Grade
    Similarly to the Math by Grade analysis I just described, we see here that the only impacted grade or school is the 9th grade Thomas High School. Again the output shows "nan" showing we had successfully replaced those "cheating" students scores.  The remainder of the values are identical to our original summary. 
### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********

## 7. Scores by School Spending per Student
    Since we have removed the cheating students from our count and are only accounting for the 10th - 12th grade students. As I stated back in the top preforming schools - since we aren't accounting for the additional students with no grade, the overall percentages return to roguhly the same as in the original analayses.  Since that is only a tenth of a percent for all the calculations when we have all figures rounded off to a whole number the scores come out identical to our original summary output. 


### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********

## 8. Scores by School Size
    As explained in the other analyses above - since we have corrected for both the cheating scores and updated the count for Thomas High school to only include non-cheating grades, we see results are virtually identiacal to our initial analysis. 
### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********

## 9. Scores by School Type
    Similar to the School Spending per student and scores by school size before, these updated outputs are very similar to our original analysis results, as shown below. 
### Original Analysis
            *********OLD IMGAGE INSERT**********
### Updated Analysis
            *********NEW IMGAGE INSERT**********



# Summary of Analyses

    Having updated the 9th grade Thomas High School grades to "nan" cause several signifcant changes within our calculations.  Primarily, and most easily observable, we can now see in both the Average Math Score by Grade & Average Reading Score by Grade; for Thomas High School's 9th grade values have been replaced with "nan", see images in subsections 5 & 6, respectively.  
    
    Additionally we saw how while replacing their grade values as "nan" is equivalent punishment for those who cheated; it is rather unfair to include those same cheating students in the student population count of Thomas High School - for purposes of averages and percentages(see the midpoint results image posted in subsection).  For this reason we had to change how the overall student population would need to be calculated for when including Thomas High School.  This was achieved in the excercise by using the loc method to identify and remove the total count of Thomas High school ninth graders from the entire population of students in the school district analysis.  The ultimate outcome being the "clean student count"   
    
    This recalculation of student population impacted several other functions, including how we should be caculting our counts for each of the passing grades.  We need to update our functions to include the loc method identifying who among the entire population achieved a passing grade for either and eventually both subjects.  However we now need to subtract the total number of "cheating students" from those totals in order for their counts to be accurate resulting in "clean passing counts". 

    Of course changing our counts creates a more accurate set of data for each of the % Passing results(i.e. % Passing Math, % Passing Reading and % Overall Passing)  These formulas need to be to updated to include the the respective subjects clean passing counts which are to be divided by the clean student count; creating the clean passing percentages.  

    Finally we need to update the Summary dataframe with these updated values to accurate reflect the passing %'s for the entire school district. 

