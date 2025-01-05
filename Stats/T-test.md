# Table of Contents

- [Table of Contents](#table-of-contents)
  - [Understanding the t-test](#understanding-the-t-test)
  - [what is a t-test?](#what-is-a-t-test)
  - [types of t-tests](#types-of-t-tests)
    - [**one sample**](#one-sample)
    - [**independent**](#independent)
    - [**pair-sample**](#pair-sample)
  - [what are the assumptions for a t-test](#what-are-the-assumptions-for-a-t-test)
  - [what are the hypothisys for a t-test](#what-are-the-hypothisys-for-a-t-test)
    - [**one sample**](#one-sample-1)
    - [**independent**](#independent-1)
    - [**pair-sample**](#pair-sample-1)
  - [Why do we need a t-test?](#why-do-we-need-a-t-test)
  - [How to do a t-test](#how-to-do-a-t-test)
  - [small recap](#small-recap)
  - [how to actually use our t-value](#how-to-actually-use-our-t-value)
    - [**what is the p value**](#what-is-the-p-value)
    - [critical t-values](#critical-t-values)
    - [2 tailed vs 1 tailed](#2-tailed-vs-1-tailed)



## Understanding the t-test
 - after this section we should know 
 - what a t-test is and when to use it 
 - what types of t-tests there are
 - what is hypotheses and what are the assumptions 
 - how a t test is calculated

## what is a t-test?
 - a t-test is a statical test procedure
 - a t-test aims to see whether there is a significant difference between the mean of 2 groups
 - ex -> lets say that we want to see how well some drug tests are doing we can have drug A and drug B if we want to know if there is a difference in the blood pressure of the 2 groups 

## types of t-tests
 ### **one sample**
 - this is used when we want to compare the mean of a sample with a known reference
 - ex ->  someone that makes chocolate says their bars weigh an average of 50 grams to check this we can weigh 30 bars from that person and we find that the mean value of the weight is 48 grams then we check if the 48 grams is significantly different from the 50 grams 
 ### **independent**
 - this is when we want to compare the means of 2 independent samples 
 - we want to see if there is a significant difference between these means
 - ex -> we want to see the effectiveness of 2 painkillers to do this we can take 60 people and put them into 2 groups we can look at the mean difference in pain relief to see if their is a significant difference between the 2 groups
 ### **pair-sample**
 - ex -> lets say that we want to see if a diet plan works we can see how much people weighed before they started the diet and then how much they weighed after their diet 
 - similar to one sample 
 - its like one sample measured twice we can just do weight - new Weight then take the mean of the difference and compare that value to 0 this will show how much people have deviated from their average weight

## what are the assumptions for a t-test
 - in all kinds of t-tests we will need to make sure that we have the right sample data being metric data 
 - in all types of t-tests the metric data must be normally distributed (we can test if our data is normally distributed) 
 - for a independent t-test the variance has to be approximately equal we can test for this using levenes test

## what are the hypothisys for a t-test
 ### **one sample**
 - null: sample mean is equal to given refrence value 
 - ex -> if we say that our avrage weight of a choclate bar os 50g then our null is that our averag weight of our bars is 50g
 - our alternative hypothisys is that the average weight of our bars is not 50g
 ### **independent**
 - null: mean values in both groups are the same
 - alt: both groups have diffrent mean values
 ### **pair-sample**
  - null: mean of the diffrence between the pairs is 0
  - alt: mean of the diffrence between the pairs is not 0

## Why do we need a t-test?
 - lets say that there is a diffrence in time it takes to get a batchlord dagree for somone in germany 
 - population: evreyone who has a batchlors dagree in germany 
 - because we cant find evreyone in germnay we get as many people as we can to get a repersentave sample
 - in this senero we would use a independent t-test and see how long it took men and woman after that we would get our average
 - so its not realistic to have the 2 groups have the exact same amout of study time but we try to see if the diffrence between the groups is significant
 - this is what the t-test actually does 

## How to do a t-test
 - to calculate a t test we first have to get a t-value
 - we first need the duffrence between the mean values and the standard devation from the mean (also known as standard error)
 - formulas are found in notebook 

## small recap
 - t value goes up if we have a large diffrence between the means
 - t value will be smaller if the diffrence between the mean is smaller 
 - having normally distributed data is better for the t-test if we have super scattered points our t-test will be messed up

## how to actually use our t-value
 - we can read the crtitical values from a table
 - or we can use the t-value to find the p-value
 ### **what is the p value**
 - so first remember that a t-test tests that there is no diffrence
 - when we draw a sample the sample will devate from the null hypothsys by a certian amount 
 - the p-value will tell us how likley it is that we draw a value that deveates by the same amount or more
 - so we can think that crazy outliers will usually result in a very low p value because there will be less likley to find a sample that has a crazy diffrence from the mean
 ### critical t-values
 -  we can understand our t-values by looking at a t-table
 -  the col's of this table repersents our signifance level 
 - if we want to have a significance level of 0.05 we will take 1 - 0.05 which will be 0.95 
 - the rows repersent the dagrees of freedom which is the number of cases - 1
 - ex -> if we have a sample of 10 people there are 9 degrees of freedom 
 - in a independent t-test we take both samples -2 ex -> (n1 + n2) - 2 
 
 ![alt text](<../images/Screenshot 2024-12-28 083842.png>)

 - looking at this table if we have a 0.05 level of significnance (0.95) and a df of 9 we will have a critical t value of 2.262
 - if our calaulated t-value is larger than the critical t-value
 - we reject the null hypothisys
 - ex -> we get a t-value of 2.5
 ### 2 tailed vs 1 tailed
 - in a 2 tailed test we could reject the null hypothsys if we are too far away from the bell curve on either side
 - in a one tailed test we will only reject null if we are too far away from the bell curve on one side
 
 ![alt text](<../images/Screenshot 2024-12-28 090054.png>)
  


 