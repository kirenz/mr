# Solutions


## Chapter 5

### Exercise 11

Air quality.


- a: The median is the 50% of the distribution, which is about **30**.

- b: Since the distribution is right skewed the **mean is higher** than the median.

- c: Quartile
  - Q1: between 15 and 20. 
  - Q3: between 35 and 40. 
  - IQR: about 20.

- d: Values that are considered to be unusually low or high lie more than 1.5×IQR away from the quartiles. 
  - Upper fence: Q3 + 1.5 × IQR = 37.5+1.5×20=67.5
  - Lower fence: Q1 - 1.5 × IQR = 17.5+1.5×20=−12.5
  - The lowest AQI recorded is not lower than 5 
  - The highest AQI recorded is not higher than 65, which are both within the fences. 
  - Therefore none of the days in this sample would be considered to have an unusually low or high AQI.


## Chapter 9

### Exercise 5


a) 33.5095 − 1.4207×𝚜𝚎𝚡𝚖𝚊𝚕𝚎 − 0.2787×𝚜𝚔𝚞𝚕𝚕_𝚠 + 0.5687×𝚝𝚘𝚝𝚊𝚕_𝚕 − 18057×𝚝𝚊𝚒𝚕_𝚕
 
b) log (p'/1-p')= 33.5095 − 1.4207×1 − 0.2787×63 + 0.5687×83 − 1.8057×37 = −5.0781

auflösen nach p':

e^-5.0781 / 1 + e^-5.0781 = **0.0062**



## Chapter 12

### Exercise 1

Outside YouTube videos. 


- a: The statistic is the proportion of outside videos among the 128 sampled. 
  - The statistic is **0.289**. 
  - The parameter is the proportion of outside videos among all YouTube videos. 
  - The parameter is not a number we can calculate (we cannot watch all YouTube videos).

- b: Notation
  - The notation used to describe the statistic is **p'**.
  - The notation for the unknown parameter value is **p**.

- c: For each bootstrap sample, calculate the proportion of YouTube videos which take place outdoors.   
  - See [code in week 9](https://mr-ws22.github.io/website/code/56-medical-case.html)

- d: The histogram of bootstrap sample proportions will be centered at **0.289** (the sample proportion from the original dataset).

- e: To create the interval, we *count 50* bootstrap repetitions in from each tail of the histogram (leaving 90% or 900 bootstrap repetitions in the middle). 
  - A rough approximation for the inteval is (**0.22**, **0.35**).

- f: We can be 90% confident that between 22% and 35% of all YouTube videos take place outdoors.


### Exercise 3

Twitter users and news.

- 98% confidence interval: 0.98 x 1000 =  980; 2% = 0,02 * 1000 = 20
  - start by finding the bootstrap proportions that separate 10 on the left, 980 in the middle, and 10 on the right (0,0125 steps: 0.475 0.4875 0.5    ...   0.550  0,5625 0,575)
  - lower bound is approximately **0.48**, 
  - upper bound is approximately **0.56** 
  - With 98% confidence, the true proportion of all US adult Twitter users (in 2013) who get at least some of the news from Twitter is between 0.48 and 0.56.


### Exercise 5

Bootstrap distributions of p', II.

- a: The data in *A* or perhaps *D* could have come from **p=0.05**

- b:  The data in *A*, *B*, *C*, or *D* could have come from **p=0.25**

- c: The data in *B* or *C* could have come from **p=0.45**

- d: The data in *B* could have come from **p=0.55**

- e: *None* of the data could have come from **p=0.75**


## Chapter 16

### Exercise 3

Defund the police.


- a: 1/5 = 0.2
  - H_A : **p > 0.20**
  - H_0 : **p = 0.20**

- b: calculate statistic p': 159 / 650 = **0.245** (we will compare this to H_0)

- c: Answers will vary. 
  - Each student can be represented with a card. 
  - Take 100 cards, 
  - 20 black cards representing those who support proposals to defund police departments 
  - 80 red cards representing those who do not. 
  - Shuffle the cards and draw with replacement (shuffling each time in between draws) 
  - 650 cards representing the 650 respondents to the poll. 
  - Calculate the proportion of black cards in this sample, p̂ sim, i.e., the proportion of those who support proposals to defund police departments. 
  - The p-value will be the proportion of simulations where p̂ sim ≥ 0.245.
 (Note: We would generally use a computer to perform the simulations.)

- d: There is only *one* simulated proportion that is at least 0.245, 
  - 1 / 1000 = 0,001
  - therefore the approximate p-value is **0.001.** 
  - Your p-value may vary slightly since it is based on a visual estimate. 
  - Since the p-value is smaller than 0.05, we *reject H_0*.
  - The data provide convincing evidence that the proportion of Seattle adults who support proposals to defund police departments is greater than 0.20, i.e. more than one in five.



### Exercise 7

If it fits, it sits, standard errors

- a: Mathematical model: SE(p')= SQRT[(p x (1-p)) / n] =  SQRT[(0.5 x 0.5) / 7] = 0.189

- b: Steps to come up with the standard error:
  - You first need to get a sense of the data (I find it useful to take the 95% confidence intervall since we know that a 95% confidence intervall equals roughly 2 standard errors)
  - We have 1000 simulations -> 2,5% on the left: 25 ; 2,5% on the right: 25; 950 in the middle
  - The upper value is about 0.875 (this is my best guess)
  - The lower value is about 0.125 (this is my best guess)
  - We know that if we add the standard error about 2 times to the middle of the distribution, we reach the upper value.
  - The middle of the distribution is about 0.5
  - This means: 2xSE = (0.875 - 0.5) = 0.375   
  - and SE = 0.375/2 = 0.1875


- c: Yes! The standard errors from the two methods are approximately the same.

- d: No. There are only 7 observations, so there is no way that the dataset could have at least 10 successes and 10 failures.

- e: Due to the small sample size, the sampling distribution shows that there are only a few possible values for the sample proportion. The mathematical model is a continuous curve which does not take into account that there are only a handful of distinct options. The mathematical model will overestimate some values and underestimate others (when calculating probabilities).





### Exercise 9

- a: The parametric bootstrap simulation was done with p=0.7 and the data bootstrap simulation was done with p=0.6

- b: The parametric bootstrap is centered at 0.7; the data bootstrap is centered at 0.6.

- c part 1: p. Steps to come up with the standard error:
  - You first need to get a sense of the data (I find it useful to take the 95% confidence intervall since we know that a 95% confidence intervall equals roughly 2 standard errors)
  - We have 1000 simulations for p -> 2,5% on the left: 25 ; 2,5% on the right: 25; 950 in the middle
  - The upper value is about 0.9 (this is my best guess)
  - The lower value is about 0.5 (this is my best guess)
  - We know that if we add the standard error about 2 times to the middle of the distribution, we reach the upper value.
  - The middle of the distribution is about 0.7 (we use p in this example)
  - This means: 2xSE = (0.9 - 0.7) = 0.2   
  - and SE = 0.2/2 = 0.1


- c: part 2: p' Steps to come up with the standard error:
  - You first need to get a sense of the data (I find it useful to take the 95% confidence intervall since we know that a 95% confidence intervall equals roughly 2 standard errors)
  - We have 1000 simulations for p' -> 2,5% on the left: 25 ; 2,5% on the right: 25; 950 in the middle
  - The upper value is about 0.8125 (this is my best guess)
  - The lower value is about 0.375 (this is my best guess)
  - We know that if we add the standard error about 2 times to the middle of the distribution, we reach the upper value.
  - The middle of the distribution is about 0.6 (we use p' in this example)
  - This means: 2xSE = (0.8125 - 0.6) = 0.2125   
  - and SE = 2.125/2 = 0.10625
  
- c: part 3: The standard error of the sample proportion is given to be roughly 0.1 for both histograms.



- d: Both histograms are reasonably symmetric. Note that histograms which describe the variability of proportions become more skewed as the center of the distribution gets closer to 1 (or zero) because the boundary of 1.0 restricts the symmetry of the tail of the distribution. For this reason, the parametric bootstrap histogram is slightly more skewed (left).



### Exercise 11



- a: The parametric bootstrap distribution imposes the condition that the true population parameter is p=0.7, so it should be used to test whether the population from which the statistics majors were sample (i.e., the population of all statistics majors) has 70% employed students. The data bootstrap distribution should be used to find a confidence interval for the true proportion of statistics majors who are employed at least 5 hours per week.


- b:  Let p be the true proportion of all statistics majors who are employed at least 5 hours per week, while also being full-time students. 
  - H_A: p ≠ 0.7.
  - The hypotheses can be written as: H_0:p = 0.7; 
  - Approximately *175* of the simulations had a bootstrapped sample proportion which is less than the observed value of 0.6. 
  - Therefore the p-value is (175/1000= 0,175 -> 0,175 * 2 = 0,35) roughly 0.35, much too large to reject. 
  - There is no evidence that the proportion of full-time statistics majors who work is different from 70% (the overall university percentage).


- c: Given 1000 bootstrap repetitions, a 98% percentile confidence interval is built to include:
  -  98% (980) bootstrapped proportions in the middle 
  - with 1% (10) on each end. 
  - By considering the data bootstrap distribution, the confidence interval goes roughly from *0.35* to *0.8*. 
  - We are 98% confident that the true proportion of all full-time student statistics majors who work at least 5 hours per week is between 35% and 80%.


- d: Using the data bootstrap distribution we know that the standard error of the sample proportion is approximately 0.1. 
  - To find 98% of the normal distribution in the middle, we use the 99%, 
  - given by qnorm(0.99) = 2.33. 
  - The 98% confidence interval for the true proportion of all full-time student statistics majors who work at least 5 hours per week is: (0.6−2.33⋅0.1,0.6+2.33⋅0.1)→0.367to0.833.



### Exercise 13

Vegetarian college students.

- a: **False**. 
  - For the distribution of p̂ to be approximately normal
  - we need to have at least *10 successes* and *10 failures* in our sample (on the average).

- b: **True**. 
  - The success-failure condition is not satisfied np=50×0.08=4 and n(1−p)=50×0.92=46,
  - therefore we know that the distribution of p̂ is not approximately normal. 
  - In most samples we would expect p̂ to be close to 0.08, the true population proportion. 
  - While p̂ can be as high as 1 (though we would expect this to effectively never happen), 
  - it can only go as low as 0. 
  - Therefore the distribution would probably take on a right-skewed shape. 

- c: **False**. 
  - p' = 0.12 (is this value different from 0,08?)
  - Standard error of p̂ in samples with n=125
  - SE(p̂) =SQRT(p(1−p)/n)
  - = √ ((0.08 × 0.92) / 125) = *0.0243*
  - Calculate difference: (0.12 − 0.080)/ 0.0243 = 1.65
  - A p̂ of 0.12 is only 1.65 standard errors away from the mean, which would not be considered unusual.


- d: **True**. 
  - Standard error of p̂ in samples with n=250
  - SE(p̂) =SQRT(p(1−p)/n)
  - = √ ((0.08 × 0.92) / 250) = *0.0172*
  - Calculate difference: (0.12 − 0.080)/ 0.0172 = 2.32
  -  A p̂ of 0.12 is 2.32 standard errors away from the mean, which might be considered unusual.

- e: **False**. 
  - Since n appears under the square root sign in the formula for the standard error, 
  - increasing the sample size from 125 to 250 would decrease the standard error of the sample proportion only by a factor of SQRT(2)


### Exercise 15


- a: **True**. 
  - The success-failure condition is not satisfied np=30×0.90=27
  - and n(1−p̂ )=30×0.10=3,
  - therefore we know that the distribution of p̂ s not nearly normal. 
  - In most samples we would expect p̂ to be close to 0.90, the true population proportion. 
  - While p̂ can be as low as 0 (thought we would expect this to happen very rarely), 
  - it can only go as high as 1. 
  - Therefore the distribution would probably take on a *left-skewed* shape. 

- b: **True**. 
  - Since n appears in a square root for SE, 
  - using a sample size that is 4 times as large will reduce the SE by half.

- c: **True**. 
  - The success-failure condition is satisfied np=140×0.90=126
  - and n(1−p)=140×0.10=14,
  - therefore the distribution of p̂ 
  - is nearly normal.

- d: **True**. 
  - The success-failure condition is satisfied np=280×0.90=252
  - and n(1−p)=70×0.10=28,
  - therefore the distribution of p̂ is nearly normal.


### Exercise 23



a)

(i) Let’s prepare for running a hypothesis test. 

- We have a sample proportion of p̂ = 0.55
- and a sample size of n = 617 independents. 
- We want to check for a majority (or minority), so we use the following hypotheses:
  - H0: p = 0.5
  - HA: p ≠ 0.5

(ii) Next, we check whether the conditions are met to proceed. 

- Since this is a random sample, independence is satisfied. 
- The success-failure condition is also satisfied: 
  - 617×0.5
  - and 617×(1−0.5)
  - are both at least 10 (we use the null proportion p0=0.5
 for this check in a one-proportion hypothesis test).


(iii) Next, we can start performing calculations. 

- We can model p̂ using a normal distribution with a standard error of
- SE=SQRT(p(1−p)n) = 0.02
- We use the null proportion, p0=0.5 to compute the standard error for a one-proportion hypothesis test.

- Next, we compute the test statistic:
- Z = (0.55 − 0.50)/ 0.02 = 2.5

- This yields a one-tail area of 0.0062, and a p-value of 2 × 0.0062=0.0124. (*you need software for this*)

(iv) Lastly, we make a conclusion. 

- Because the p-value is smaller than 0.05, we reject the null hypothesis. 
- We have strong evidence that the support is different from 0.5, and since the data provide a point estimate above 0.5, we have strong evidence to support this claim by the TV pundit.


- b: No. Generally we expect a hypothesis test and a confidence interval to align, 
  - so we would expect the confidence interval to show a range of plausible values entirely above 0.5
  - However, if the confidence level is misaligned (e.g., a 99% confidence level and a α=0.05 significance level), then this is no longer generally true.


### Exercise 25

see exercise 23 (the same)

The hypotheses are as follows: H0:p=0.5
. HA:p>0.5
. Before conducting the hypothesis test, we must first check that the conditions for inference are satisfied. Independence (random sample, <10%
 of population) is satisfied, as is the success-failure conditions (using p0=0.5
, we expect 40 successes and 40 failures). The test statistic and the p-value can be calculated as shown below. Since the p-value <α
 (use α=0.05
 since not given), we reject the null hypothesis. The data provide strong evidence that the rate of correctly identifying a soda for these people is significantly better than just by random guessing.

p̂ Zp−value=5380=0.6625=p̂ −p0p0(1−p0)n‾‾‾‾‾‾‾√=0.6625−0.50.5×0.580‾‾‾‾‾‾√=0.16250.0559=2.91=P(p̂ >0.6625 | p=0.5)=P(Z>2.91)=1−0.9982=0.0018
If in fact people cannot tell the difference between diet and regular soda and they randomly guess, the probability of getting a random sample of 80 people where 53 or more identify a soda correctly would be 0.0018.


## Chapter 17

### Exercise 3



Disaggregating Asian American tobacco use, confidence interval.

- a: The bootstrapped difference in proportions 
  - appear to vary from about 0.052 to 0.077, 
  - resulting in a standard error of roughly 0.00625.

- b: The bootstrap SE confidence interval can be constructed using: 
  - p'_Filipino - p'_Chinese +- 1.96 * SE  
  - = 0.065 +- 1.96 * 0.00625
  - = (**0.0528, 0.0772**).
  - We are 95% confident that the true proportion of Filipino Americans who are current smokers is between 5.28 and 7.72 percentage points higher in the control vaccine group than the proportion of Chinese Americans who smoke.

- c: The bootstrap distribution indicates that the bootstrap differences vary from roughly 0.052 to 0.077. (my best guess)
  - We are 95% confident that the true proportion of Filipino Americans who are current smokers is between 5.2 and 7.7 percentage points higher in the control vaccine group than the proportion of Chinese Americans who smoke.


### Exercise 13


- Before we can calculate a confidence interval, we must first check that the conditions are met. 
- There aren’t at least 10 successes and 10 failures in each of the four groups (treatment/control and yawn/not yawn)  


- (p'_C - p'_T) is not expected to be approximately normal 
- -> therefore cannot calculate a confidence interval for the difference between the proportions of participants who yawned in the treatment and control groups using large sample techniques and a critical Z score.


### Exercise 21

**THIS TASK IS NOT EXAM RELEVANT**

Malaria vaccine effectiveness, effect size.

In order to reject the null hypothesis, the difference in sample proportions will need to be more than 2 standard errors from zero. Which means that the difference will be smaller than -2 * standard error.

The question for each part is, what proportion of the normal curve centered at δ
with a standard error of ...



