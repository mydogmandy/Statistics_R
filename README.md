# Statistics_R

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

## PART A:

  Using multiple linear regression, design a linear model that predicts the mpg of 
  MechaCar prototypes using a number of variables within the MechaCar mpg dataset. 

  1.  Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
        - Referencing the below data, vehicle length & ground clearance provided a significant non-random amount of variance.
        - Vehicle weight may have contributed, but not with the confidence of length & clearance due to low p value.

![](/Image_Resources/Coefficients.png)


  2. Is the slope of the linear model considered to be zero? 
       - No, the slope is not zero
          2a. Why or why not?
              - p-value = 5.35e-11, or 0.0000000000535

  3. Does this linear model predict mpg of MechaCar prototypes effectively?
       - Yes
    3a. Why or why not?
        - The multiple R-squared value = 0.7149, which predicts at 71% of the time.

## PART B:

  Create a summary statistics table for the suspension coil’s pounds-per-inch continuous variable.
  
![](/Image_Resources/Summary_Statistics.png)


  The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils 
  must not exceed 100 pounds per inch
  
  1.Does the current manufacturing data meet this design specification? 
      - Yes. Overall, the variance is under 100 psi at 62.29356, but only lots 1 & 2 meet the variance specifications
    1a. Why or why not?
        - Lot 3 does not meet specifications, as psi exceeds 100 pounds per square inch at 170.2861224
  
  2. Using the same suspension coil data and the MechaCarChallenge.RScript file, determine if the suspension coil’s 
        pound-per-inch results are statistically different from the mean population results of 1,500 pounds per inch.
  
      - Assuming our significance level is the common 0.05 percent, out p-value is above our significance level.  
        Therefore, we do not have sufficient evidence to reject the null nypothesis, and can state that the two 
        means are statistically similar.
      
![](/Image_Resources/One_Sample_t-test.png)
 

## PART C:

  Design a study that compares the performance of the MechaCar prototype vehicle to other comparable vehicles on the market. 
  Write a short description of a statistical study that can quantify how the MechaCar outperforms the competition. 
  In your study design, be sure to write about the following considerations:

  1. Think critically about what metrics you would think would be of interest to a consumer (cost, fuel efficiency, color options, etc.).
       - MSRP, MPG (City & Highway), Horsepower, Transmission, Seating Capacity, Braking, Acceleration, Options
    
  2. Determine what question we would ask, what the null and alternative hypothesis would be to answer that question, 
       and what statistical test could be used to test this hypothesis.
       - Null hypothesis = For each metric of interest listed, out-performing the competition (e.g. Horsepower), will have no effect on a
         consumer's decision to purchase the MechaCar.
       - Alternative hypothesis = There is a clear statistical significance between out-performing the competition when it comes to deciding
         whether or not to purchase a vehicle - such as greater seating capacity, better braking, or faster acceleration.
       - Statistical test = Chi-Squared Test to determine the catagorical frequencies between the metrics tested.
        
  3. Knowing what test should be used, what data should be collected?
       - Data collected = Consumer reported data in the form of surveys, vehicle registration data for new vehicles, competition sales numbers.
 
