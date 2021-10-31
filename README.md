# suicide-EDA
According to the NIMH, in 2019 suicide was the tenth leading cause of death in the United States. It is the second most common cause of death in individuals aged 10 and 34, and the fourth for those aged 35 to 44. As an exercise in exploratory data analysis and to better understand the risk factors behind suicide, I'll be examining a dataset from the WHO that was archived on Kaggle. My focus will be on the United States. The dataset itself contains numbers of suicides across categories such as country, age, and sex, and covers years between 1979 to 2016. Regrettably, the numbers for 2016 are missing for the US. Because the missing values were localized entirely to that year and I could not find another
reliable dataset that offered the information I needed to fill it in, I went ahead and omitted the year entirely. 

As far as my hypothesis goes, I think the data will show two things: that the risk of suicide increases with age, and that men are more likely than women to do it. With age comes problems such as failing health, loneliness, and depression. On the front of sex, Men are less likely to seek therapy for mental illness, and are more prone to a variety of health problems, including many cancers.

To assess risk, I made a new feature of the quotient between the numbers of suicides and the population per row. This feature is called "no_to_pop", or "number to population." For exploratory data analysis, the first thing I did was use a line plot to plot the instances of suicide over the years given. What the figure shows is that since 2005, the occurances of suicide in the United States has been increasing at an alarming rate, with over 12000 more deaths in 2015 than in 2005 (44189 and 32629 respectively). 
Next I made a bar plot using no_to_pop and age, and found that those over the age of 75 were far more likely than any other age group to take their own life. Plotting the same features but dividing the dataframe into subsets for men and women, I found that men were overall dramatically more likely than women to commit suicide. Curiously enough, while men were more likely to do so past the age of 75, women seem to be most at risk between the ages of 35 and 54.

The results are as follows: 
-The most at-risk are men above 75.
-Men are far more likely than women to commit suicide.
-Women tend to take their lives between the ages of 35 and 54.
