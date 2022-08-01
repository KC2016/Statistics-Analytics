# a_b_testing
Sandbox for SoundCloud


Power Statistic: estimation of an appropriate sample size
- Sample distribution

- alfa: probability of type I error(0.05) , confidence level of 95%

- p-value: probability that the observed statistic occurred by chance alone. We reject the null hypothesis if p-value is very low. The conventional threshold for rejecting the null hypothesis is 5%.

- power:  probability that an experiment will flag a real change as statistically significant. The convention is to require 80% power. Power depends on magnitude of the change, and variance among samples.

- true-effect: the actual difference of mean between the buckets that would have been observed if we had infinitely large sample sizes. It’s a fixed but unknown parameter, which we are trying to infer.

- False positives — the 5% chance of getting a measurement under the null hypothesis that is so far from the mean that we call it statistically significant. 

- Power: 80% of time we call statistical significance under the alternative. 


- **“minimal detectable effect” MDE — estimates the smallest improvement you are willing to be able to detect. It determines how "sensitive" an experiment is. 
With 0.8MDE, given sample size and sample variance, we can calculate the smallest real effect size which we would be able to detect at 80% power.**

- H0: null hypothesis: absence of effect (control)
- H1: alternative hypothesis: presence of effect (treatment)
- Statistical significance: comparison between alfa and p-value
- p-value < 0.05: there is a difference (reject H0) SIGNIFICANT
- p-value > 0.05: there is no diference (fail to reject H0) NOT SIGNIFICANT
- p-value = 0 (CRITICAL VALUE = size of difference + sample size + significance)
- Hₒ: p = pₒ
- Hₐ: p ≠ pₒ

- type II error (beta): failure to reject a false H0
- power: probability of detecting an effect which is really there.
- Power = 1 - beta (inversely proportional)
- Convension: Power+0.8 and beta=0.2

- Note: mu(mean), sigma (standard)


- T-test: hypothesis testing, test statistic is compared to the critical value to determine sgnificance.

- If test statistic > critical value: statistical significance and null hyplothesis rejection (t-value > critical t-value)

- Reletionship between variables
-> Effect size: difference of biological interest and variabilidade (std deviation)
-> power of the experiment (80%)
-> significance level (5%, being 5% from one-sized test and 2x2.5% for two-sized test) 
-> sample size
-> alternative hypothesis (one or two-sized test)

- The larger the effect size, the smaller the experiment will need to be to detect it.


Cronology

1- Hypothesis

2- Experimental design/choice of a Statistical test

3- Power Analysis: Sample size

4- Experiment(s)

5- Data exploration

6- Statistical Analysis of the results

<!-- ![01](images/01.png) -->
<img title="01" alt="Alt text" src="images/01.png">

<!-- ![02](images/02.png) -->
<img title="02" alt="Alt text" src="images/02.png">

- p-value (p): Probability of obtaining a result equal to or more extreme than was observed in the data.


- **Type I Error.** Reject the null hypothesis when there is in fact no significant effect (false positive). The p-value is optimistically small.

- **Type II Error.** Not reject the null hypothesis when there is a significant effect (false negative). The p-value is pessimistically large.

- Usual value for Statistical Power = 80%,being 20% of false negatives.

- **Low Statistical Power:** Large risk of committing Type II errors, e.g. a false negative.

- **High Statistical Power:** Small risk of committing Type II errors.


### Power Analysis (Student's t Test Power Analysis)

- **Effect Size.** The quantified magnitude of a result present in the population. *(using Pearson’s correlation coefficient for the relationship between variables or Cohen’s d of at least 0.80)* 

- **Sample Size.** The number of observations in the sample.

- **Significance (alpha).** Boundary for specifying a statistically significant finding when interpreting the p-value. (5%)

- **Statistical Power.**  The probability of accepting the alternative hypothesis if it is true. (80%)

<!-- ![03](images/03.png) -->
<img title="03" alt="Alt text" src="images/03.png">

> [Source](https://machinelearningmastery.com/statistical-power-and-power-analysis-in-python/)

 [PowerCalculator](https://bookingcom.github.io/powercalculator/)