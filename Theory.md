# Statistics Background
## Measures of Center
### Arithmetic Mean
= Mean = Average  
= ∑x/N

#### Advantages
Most accurate measure of center in a dataset without outliers.

#### Disadvantages
Influenced by outliers.

### Outlier
A data value that is either much greater than or much less than the rest of the data and not representative of the rest of the data being considered.

### Median
- Middle value in the sorted list of data values.  
= (N+1)/2  
  - N = number of items in the list
  - If no single middle exists, find the mean between the two middle items.

#### Advantages
Not influenced by outliers.

#### Disadvantages
In a dataset without outliers, a less accurate measure of center.

### Mode
- The most frequently occurring value.
- Much less commonly used than mean and median.
*e.g. The mode of 1, 4, 4, 8, 8, 8, 9 is 8, because 8 appears more times than any other value.*

## Measures of Spread
### Minimum, Maximum, Range
- Measures of Center **does not** indicate the **spread** of data values.
- A simple measure of spread is to report the **minimum** and **maximum** values as well as the **range**.
### Mean Absolute Deviation (MAD)
- The mean of the absolute difference between each value and the value's mean.
- Absolute values (magnitudes) are used to avoid negative distances.
### Variance and Standard Deviation
- **Variance**: Squares the difference between each value and value's mean.
- **Standard deviation**: The square root of the variance.

## Histograms
### Histogram with evenly-sized bins
#### Frequency Distribution
A table that displays how often an outcome occurs for a sample.
- **Construction**: The data set is divided into mutally exclusive classes.
- **Class**: A value of a categorical variable OR an interval of a continuous variable.
- **Frequency**: The number of events or values that fall under each class.
#### Histogram
The most common graphical representation of a frequency distribution.
- **Bin** Splits a continuous variable into a number of class intervals.
  - Includes value equal to or greater than the lower boundary, but less than the upper boundary (**lower <= value < upper**).
### Histogram bin size
#### Goal of Histogram
Estimate the probability density function of the continuous variable on the x-axis, i.e. to be able to **fit a smooth curve over the most rectangles**, while **minimizing the white space under the curve**.
- Multiple bin sizes should be attempted to determine the best distribution of the data.
- Start with a bin size so that the number of bins = +- √N where N is the nubmer of values.
  - E.g. Officer Smith has 15 tickets -> √15 = 3.9 ≈ 4 bins. Since the maximum ticket speed is 28 mph over the limit, a good initial bin size would be 28/(4 bins) = 7 mph bins.
### Distribution Patterns
- **Unimodal**: standard bell curve; one prevalent peak (mode) in histogram.
- **Bimodal**: two prevalent modes.
- **Multimodal**: multiple prevalent mode.
- **Skewed Left**: contains a mode on the right with a tail of low-frequency bins to the left.
- **Skewed Right**: contains a mode on the left with a tail of low-frequency bins to the right.
### Histograms with unevenly-sized bins
- **Unit Area Histograms** should be used to compare likelihoods of two unequally-sized bins.
  - Rectable heights are equal to the bin/frequency/bin size.
## Experiments and Events
### Experiments, outcomes, and sample spaces
- **Experiment**: a procedure that results in one out of a number of possible outcomes.
- **Outcome**: the result of an experiment.
- **Sample Space**: the set of all possible outcomes (e.g for dice: 1, 2, 3, 4, 5, 6).
### Events
- **Events**: Subset of a sample space. E.g. for a dice roll, the event A is rolling an even number.  The event A occurs when a 2, 4, or 6 is rolled.
  - **Compound Event**: Subset of the sample space consisting of more than one outcome. E.g. The event A is compound event since rolling an even number consists of three otucomes.
  - **Simple Event**: Subset with a single outcome. E.g. The event C is rolling a 5 on the die. C is a simple event with a single outcome.
## Discrete Random Variable and their Distributions
### Random Variables
A rule that assigns a number to every outcome in the sample space of an experiment. E.g. in the experiment of a coin toss, a random variable may assign 1 to Heads or 0 to Tails. A random variable is typically defined using a capital letter, such as X = 1 (H) amd X = 0 (T).  
  
Random variables can be **discrete** or **continuous**.
- **Discrete random variable**: take on a countable number of distinct values like the integers between 0 and 100.
- **Continuous random variable**: take on any value within a range of values like the real numbers between 0 and 100.
### Discrete Probability Distributions: Probability Mass Functions
**Probability Mass Function (pmf)**: the probability that a discrete random variable is exactly equal to some value (typically depicted as a table, plot, or equation).
- The notation p(X=x) or p(x) us typically used or the pmf of X.
- The probabilities assigned in a pmf are between 0 and 1, and the total probability must sum 1.
### Probability Distribution: Cumulative Distribtution Function
**Cumulative Distribution Function (cdf)**: of a discrete random variable is the probability that x will fit in a **range** of values.
- Cdf sums each of the pmf values as you go along the table. The last entry should equal 1.
- Notation: F(x) where p(X ≤ x). 
## Properties of discrete probability distributions
### Mean or expected value of a discrete random variable
Mean (≡ Expected Value): the sum of the possible values of X multiplied by the probability of the value.
-	µ = E(X) = ∑▒〖x*p(x)〗
- center of the distribution
### Variance and Standard Deviation of a discrete random variable
- Mean of discrete random variable = center of the distribution.
- Variance of a discrete random variable = spread of the distribution.
  - 	σ^2=V(X)= ∑▒〖(x-μ^2 )*p(x).〗
  - Is a weighted average with probabilities as the weights.
  - units are in *unⅈts^2*.
- Standard deviation of a discrete random variable = measure of the spread in the units of the orginal random variable. It is the square root of the variance.
  - 	σ= √(σ^2 )
## Continuous probability distributions and properties
### Population density function (pdf)
Describes the relative likelihood of all values for a continuous random variable.
*Ex. The amount of time for Casey to do his chores is a random variable, X, where all values between 1 hour and 2 hours are equally likely.*
- **Notation**: f(x)
- The area under portions of the curve given by the pdf provide the probabilities.
- Must be non-negative (+).
- Total area under curve must = 1
### Continuous distribution function (cdf) for continuous random variable
The probability that for any number x, the observed value of the random variable will be at most x or p(X ≤ x).
*Ex. When Casey does the housework, the cdf describes the probability of Casey finishing in time less than or equal to any value x, such as the probability X is less than or equal to 1.5.*
- The notation F(x) is typically used for the cdf.
### Mean, variance, and standard deviation for continuous random variables
-	The mean or expected value E(X), µ, of a continuous random variable X is a measure of the center of the distribution. The mean is a weighted average of the possible values of the random variable, with the pdf providing the weights. Graphically, the mean is where a pivot is placed so that the pdf balances.
-	The variance, σ^2, of a continuous random variable X is a measure of the spread of a distribution. The variance, like the mean, is a weighted average. The variance averages the squared distance of each possible value of X from the mean, with weights provided by the pdf. The units of the variance are the units of X squared. Ex: If X is money, in dollars, the variance of X is measured in dollars squared.
-	The standard deviation, σ, is a measure of the spread of the distribution in the units of the original random variable. The standard deviation is the square root of the variance, σ=√(σ^2 ).
## Specific Distributions
### Binomial Distribution
Models how many times an event occurs in a certain number of trials, with the important assumption that the probability of the event occurs is the same for each trial.
-	*Ex. A basketball player is fouled on a 3 point shot attempt and awarded 3 free throws. A binomial distribution models the number of free throws the player makes out of three. The probability the player is successful on each attempt, based on his season average, is 0.75.*
- **Models**: number of times an event occurs in a certain number of trials.
- **Notation**: X  ~ Bin(n,p)
  - **Bernoulli distribution**: binomial distribution with n=1
  - **Parameters**: 
    - n= number of trials
    - p= probability of the event occurring on each trial; the probability is assumed the same on each trial, and trials are independent.
- **Possible values**: x= 0, 1...n. 
- **Key quantities**
  - **Mean**: n * p
  - **Variance**: n * p(1-p)
### Discrete distributions
Used when binomial distribution is not a good choice. Includes Poisson, negative binomial, and hypergeometric distributions.
#### Poisson distribution
- **Models**: The number of events that occurs in an interval; counts. *Ex. The number of emails received each day*.
- **Notation**: X ~ Poisson(µ)
- **Parameters**:
  -**µ**: Mean(average) number of events per interval.
- **Assumptions**:
  - The average in each interval is the same.
  - The count in one interval is independent of the count in other intervals.
- **Possible values**: x = 0, 1, ...
- **Key quantities**:
  - **Mean**: E(X) = µ.
  - **Variance**: σ^2 = Var(X) = µ.
#### Negative binomial distribution
- **Models**: The number of failures in a sequence of trials before an even occurs a specified number of times. *Ex. The number of non-junk emails received before 10 junk emails are received.*
- **Notation**: X ~ NB(s,p)  
The NB distribution with s = 1 is also known as **geometric distribution**.
- **Parameters**:
  - s: The number of times the event must occur (the number of successes).
  - p: Probability of the event occurring (success) on each trial; assumed the same.
- **Possible values**: x = 0, 1, ...
- **Key quantities**:
  - **Mean**: µ = E(X) = s/p
  - **Variance**: σ^2 = Var(X) = s(1-p)/p^2
#### Hypergeometric distribution
- **Models**: The number of events in a certain number of trials (draws) when each trial is a new selection from a finite population. Once selected, an item is no longer available for selection (known as "draws without replacement"). *Ex. The number of players from the AFC (one of two conferences) randomly selected for a fantasy football team.*
- **Notation**: X ~ Hypergeo(k, n, N)
- **Parameters**:
  - k: Number of trials (draws)
  - n: Number of possible events in the population
  - N: Number in the population
- **Possible values**: x = max(0, n + k - N), ... min(k,n).
- **Key quantities**:
  - **Mean**: µ = E(X) = n.k/N
  - **Variance**: σ^2 = Var(X) = n.k.(N-k)(n-n)/N^2(N-1)
### Normal distribution ≡ Gaussian Distribution 
A continuous probability distribution characterized by a bell-shaped pdf and is symmetric around the mean, µ.
- 68% of the population is within 1 standard deviation of the mean of hte normal distribution.
- 95% of the population is within 2 standard deviations of the mean of the normal distribution.
### Continuous distributions
For situations when the normal distribution is not a good choice.
- Choosing the distribution requires assumpations and key quantities such as mean and variance, shape of pdf.
#### Exponential distributions
- **Models**: Time between events. *Ex. The time until the next bus arrives at a bus stop.*
- **Notation**: X ~ Exp(ʎ)
- **Parameter**: ʎ: Rate of arrivals. *Ex. Buses arrive at a rate of ʎ = 4 per hour.*
- **Possible values**: all values ≥ 0.
- **Mean and variance**: E(X) = 1/ʎ, Var(X) = 1/ʎ^2
#### Beta distribution
- **Models**: Probability for proportions; flexible model for situations where possible values are in a range (generally 0 to 1). *Ex. The percentage of the day that will be sunny.*
- **Notation**: X ~ Beta(α,β)
- **Parameters**: α, β are shape parameters, both must be greater than 0. Sometimes additional parameters a and b are included if the range of values modeled is from a to b rather than 0 to 1.
- **Possible values**: All values between 0 and 1 (or a and b if additiona parameters added).
- **Mean and variance**: E(X) = α/(α + β), Var(X) = α.β/(α + β)^2.(α + β + 1) 
#### Uniform distribution
- **Models**: Possible values fall in arange with equal probabilities; often used to produce a random number. *Ex: The calbe repair technician provides a time window from 9 to 11 am for arrival and all times in the interval are equally possible.*
- **Notation**: X ~ U(a,b)
- **Parameters**: a is the minimum possible value and b the maximum.
- **Possible values**: All values between a and b.
- **Mean and variance**: E(X) = (a+b)/2, Var(X) = (b-a)^2/12.
#### Triangular distribution
- **Models**: Possible values fall in arange and one value in the range is considered most likely. *Ex. The return on investment is thought to range from 0 to 10% with the most likely value 7%.*
- **Notation**: X ~ Triangle(a,c,b)
- **Parameters**: a is the minimum possible value and b the maximum. The value c (which must be in the range of a to b) is the most likely value.
- **Possible values**: All values between a and b.
- **Mean and variance**: E(X) = (a+b+c)/3, Var(X) = (a^2 + b^2 + c^2 + ab - ac - bc)/18 
## Hypothesis Testing
### Statistical significance: An informal introduction
Are the sample statistics extreme enough to infer a conclusion about the population?
- If p-value < 0.05 it is statistically significant at level alpha and two possibilities exist:
  - The null hypothesis is true and the observed data is relatively unusual with an extreme sample statistic that is simply due to chance.
  - The null hypothesis is false and the alternative hypothesis provides a more reasonable explanation for the population parameter.
### Hypothesis Test Errors
- **Type I error**: True null hypothesis is rejected.
- **Type II error**: False null hypothesis is accepted.
## Confidence Intervals
A range of values believed to include a population parameter at a stated level of confidence.
- **Construction**: sample statistic and margin of error (of population mean).
  - **Margin of error (MOE)**: range of values above and below the sample statistic.
    - MOE = z* σ/√n
      - z* = critical value that depends on the type of test (one-sided vs. two sided) and the significance level α.
      - α = probability of a type I error
      - larger sample sizes  = narrower confidence interval (because of smaller MOE).
## Comparing two population means
An analyst commonly seeks to determin whether two samples are from populations with the same population means.
- A **large difference** in two **sample means**, relative to the **sample standard deviations** suggest the population means may be different. The difference depends on:
  - Standard deviations of the two populations.
  - Sample sizes.
- The sample standard deviations estimate the population standard deviations:
  - Relatively large sample standard deviations require a relatively large difference between the sample means to infer a statistically significant difference in population means;
  - Relatively small sample standard deviations require a relatively small difference between the sample means to infer a statistically significant difference in population means.
# Parametric Analysis
## Parameterized population models 
### Parametric Analysis
**Normally distributed**
- **Parameter**: Characteristics of a population
  - Population parameters are almost always unknown ∴ sampling is performed to obtain a parameter’s estimator.
- **Statistic**: Characteristic of a sample
- **Common Statistics and Parameters**
  - **Statistic**
    - ̅x: sample mean
    - s: sample standard deviation
    - s^2: sample variance
    - ̂p: sample proportion
  - **Parameter**
    - µ: population mean
    - σ: population standard deviation
    - σ^2: population variance
    - p: population proportion
### Parametric tests
-	**One-way t-test** - determines whether the hypothesized mean is equal to the true population mean.
-	**Paired t-test** - used to compare two population means in the case where the two samples are dependent.
-	**Two-way t-test** - determines whether the population means are equal.
-	**Analysis of variance (ANOVA)** - determines whether the means of two or more populations are equal.
### Normal Distribution
A bell-shaped probability distribution with two parameters: the mean (µ) and standard deviation (σ).
p(x)=1/(σ√2 π) ⅇ^((-(x-μ)^2)/(2σ^2 ))

### Finding probabilities associated with a normal distribution 
Most situations involve random variables from distributions that are continuous.
  - **Continuous random variable**: a random variable that can take on any value within a range of infinitely many or uncountable values. 
    - Ex: Random variables that represent measurements with continuous values such as body mass index and radius of an O-ring joint are continuous.
The following notation is used when working with normally distributed random variables and other random variables following continuous distributions:
- P(X<a) is the probability that the random variable X takes on a value of at most a.
- P(X>a) is the probability that the random variable X takes on a value of at least a.
- P(a<X<b) is the probability that the random variable X takes on a value between a and b.
### Central limit theorem for means
As the sample size drawn from the population with distribution X becomes larger, the distribution of the sample means X̄ approaches that of a normal distribution, N~(μx,σx/√n), where σx/√n is the standard deviation.
- Calculate probabilities associated with non-normal distributions assuming the sample sizes are sufficiently large.
#### Assumptions
1. **Randomness**: samples must be randomly selected.
2. **Independence**: sample values must be independent of each other
3. **Size**: sample size must be large enough (<30)
4. **10% condition**: sample size must be at most 10% of the population size.
## Student's t-test
### Student's t-distribution (≡ t-distribution)
Obtaining a large enough sample may not be possible or the population standard deviation is unknown. In both cases, the sample standard deviation/sample size^2 can be used in place of the population standard deviation.
- **Student's t-distribution (≡ t-distribution)** used in place of normal distirbutions where the **sample size (n) is small** or the **population standard deviation (σ) is unknown**.
  - **Parameter**: Degrees of Freedom (df) = n-1
    - As df increases, the t-distribution approches the normal distribution with mean = 0 and standard deviation = 1
- **t-statistic**: obtained from a sample assumed to have a t-distribution.
The formula for t-statistic is t=  ( ̅x - μ )/(s/√n)   where s is the sample standard deviation, ̅x is the sample mean, µ is the population mean, and n is the sample size. 
### Student's t-test (≡ t-test)
- Method of hypothesis testing for the **mean of a sample** taken from a **normally distributed population** when the **population standard deviation is unknown**.
- **Purpose**: To determine if the difference between the sample mean and the hypothesized population mean is statistically significant.
  - **Null hypothesis**: hypothesis of no difference
  - **Alternative hypothesis**: the claim contrary to the hypothesis
    - The alternative hypothesis ultimately depends on what the study claims. If the study claims that:
      - The parameter > hypothesized value: the hypothesis test is **right-tailed** and H_a:μ>μ_0. 
      - The parameter < hypothesized value, the hypothesis test is **left-tailed** and H_a:μ<μ_0. 
      - The parameter has a different value, then the hypothesis test is **two-tailed** and H_a:μ≠μ_0. 
- The **significance level** (**α**), is the probability of rejecting the null hypothesis when the null hypothesis is actually true. Thus, if the p-value is less than the significance level, sufficient evidence exists to reject the null hypothesis. Common values for α are 0.05 and 0.01.
### Confidence interval for a t-distribution
The confidence interval for a population mean was defined as (x - ̅z* σ/√n, x + ̅z^ σ/√n)
  - In practice, however, the population standard deviation is rarely known. Thus, confidence intervals using the t-distribution are more useful because the sample standard deviation is used instead.
The t-confidence interval is given by  ( ̅x - t* s/√n, ̅x + t* s/√n)
  - where t* is the critical value that depends on the type of test, degrees of freedom, and significance level. The values for t* for common significance levels given selected degrees of freedom is shown in the table below.
## Comparing 2 samples: 2-sample t-test
### Two-sample t-test
The t-test discussed analyzes the **difference between the sample mean and the hypothesized value of the population mean**. A similar method exists to compare the means of two different populations. The two-sample t-test is used to determine if a statistically **significant difference exists between two population means**. Two types of two-sample t-test exist: paired and unpaired.
#### Paired t-test (≡ dependent t-test)
- A sample taken from **one population is exposed to two different treatments**. 
- The main idea is that measurements are recorded from the **same group**. 
  - *Ex: A group of professional cycling athletes is selected for a study on the effects of caffeine dosage on exhaustion times. The populations are the cyclists for each of two dosages. The samples are the measured exhaustion times for each dosage, which implies dependence because the measurements were taken from the same group.*
  - To obtain probabilities for a paired t-test, the paired R² is needed. The formula involves finding the mean and standard deviation of the differences between corresponding measurements:
t=( ̅d - μ_d)/(s_d/√n)
Where s_d  is the sample standard deviation of the differences, ̅d is the mean difference between the samples, and n is the sample size. 

#### Unpaired t-test (≡ independent t-test)
- A sample taken from **one population is not related to a different sample taken from another population**. 
- In contrast to the paired t-test, measurements from an unpaired t-test are recorded from **different groups** when exposed to the same treatment. 
  - *Ex: The effect of caffeine intake on exhaustion times is studied by measuring the exhaustion times of a randomly selected group of 9 professional cyclists taking caffeine pills and another group of 9 cyclists not taking caffeine pills. The two populations are all cyclists taking caffeine pills and those who are not taking the pills. The samples are the measured exhaustion times from the two groups, each with 9 cyclists, which implies independence because the times are for two different groups of cyclists.*
  - The t-test statistic for unpaired data is different from that of paired data. The formula involves subtracting the means of the two samples:
( ̅x_1 - ̅x_2-(μ_1 - μ_2))/√((s_1^2)/n_1 +(s_2^2)/n_2 )
where ̅x_1,  s_1, and n_1 are the mean, standard deviation, and sample size of the sample drawn from the first population respectively; and x_2, s_2, and n_2 are the mean, standard deviation, and sample size of the sample drawn from the second population. Since measurements are not subtracted, the sample sizes are not necessarily the same. The degrees of freedom are ⅆf = n_1 + n_2 - 2. Although μ_i - μ_2 can be any number based on the hypothesized means for the two populations, most of the time, the accepted difference between the means of the populations is 0. Finally, the formula for the t-statistic above assumes that the variances are unequal. In most practical instances, the homogeneity of variances should be verified using the Fisher's F-test before performing the unpaired t-test. 
## Comparing 3+ samples: ANOVA
### Comparing 3 or more populations
- *Ex: A researcher wants to classify iris species based on sepal length by using a method called k-means clustering. As a first step, the researcher checks whether the mean sepal length differs among three species of iris: setosa, virginica, and versicolor. A possible method to compare the means is to perform three unpaired t-tests: one between setosa and versicolor, another between setosa and virginica, and finally between versicolor and virginica.*
Analysis of variance (ANOVA) controls for the errors associated with comparing multiple population means. Analysis of variance (ANOVA) determines whether a statistically significant difference exists among the means of three or more populations. Equivalently, ANOVA tests for an association between a categorical predictor variable and a response variable. 
- *Ex: In the iris study, the predictor variable is the type of species and the response variable is sepal length. Data scientists and statisticians often refer to a categorical predictor variable as a factor and a possible value of a factor as a level. A factor can be a continuous variable partitioned into intervals commonly referred to as bins.*
#### The F-statistic
The ratio of between-group variance to within group variance.  
A number of quantities are involved when calculating the F-statistic:
- The **sum of squares between groups (SSB)**: measures the between-group variablility.
- The **mean of squares between groups (MSB)**: measure the between-group variance.
- The **sum of squares within groups (SSW)**: measures the within-group variability.
- The **mean squares within groups (MSW)**: measures the within-group variance.
Since MSB and MSW represent the between-group variance and within-group variance respectively, F = MSB/MSW
#### One-way ANOVA
Compares the means of three or more groups of one predictor variable.
- Null hypothesis = all of the group means are equal.
## Linear Regression
### Linear regression model
Is a linear function used to predict the value of one variable using the values of one or more variables.
- In a linear regression involving two variables:
  - **response variable** = the variable being modeled or predicted
  - **predictor variable** = the variable used to predict the response.
    - *Ex. A researcher wishes to construct a linear model that a student's grades given the number of hours spent studying. THe predictor variable is the number of hours spent studying and the response variable is student grade*.
- A scattor plot displays a set of predictor and response varaible pairs as data points.
  - The predictor variable X goes on the horizontal axis
  - The response variable Y goes on the vertical axis
  - Assuming the data represents a population, the population linear regression function is given by E(Y)=β_0+β_1 X, where E(Y) is the expected value of Y, and β_0  and β_1 are unknown population regression parameters. 
    - **Absoulte error ∈** = The difference between the true value Y and E(Y).
#### Method of least squares
Derives a linear regression model by minimizing the sum of squared errors.
#### Sample linear regression function
Are the predicted or fitted response values based on the simple linear regression model.
#### Linear regression fitted value
Is the predicted value of Y for the ith smaple value of X based on the linear regression line.
#### Linear regression residual
Is the estimated regression error based on the sample linear regression line.
### T-Test for linear regression
Check if β_1 ≠ 0 (alternative hypothesis).
## Parametric vs. nonparametric statistics
### What is the difference between parametric and nonparametric methods?
- **Student's t-test**: compares the means of two populations.
  - *Ex. The mean heights of men and women using the sample data.*
  - **Assumptions**: Normal distribution for each population (Parametric).
- **Parametric Method**: Makes inferences based on assuming some statistical distribution of a population or for a statistic. (Normal distribution).
- **Non-Parametric Method**: Makes inferences based on data requiring fewer assumptions about the statistical distribution of the population (skewed).
### Parametric
- **Advantages**: More powerful if the assumptions of the parametric test are true.
- **Disadvantages**: Require large samples. Samples must approximate a distribution.
### Nonparametric 
  **Use**: When data is small
- **Advantages**: Do not require large samples, or for the sample to be drawn from a specific distribution.
- **Disadvantages**: Less powerful when the assumptions for a parametric test are met. Also, more difficult to compute.
#### Using nonparametric analysis when the data is skewed
A normal distribution has a skewness of zero. If the right-tailed distribution has a skewness of 0.98 and a standard error of skewness of 0.39. Because the ratio 0.98 / 0.39 = 2.51 > 1.96, the right-tailed distribution is too skewed to be analyzed with parametric methods. 
#### Using nonparametric analysis when sample sizes are small
## Resampling: Randomization and bootstrapping
**Resampling**: nonparametric technique for determining statistical significance by comparing an outcome with a set of outcomes obtained by randomly assigning the data points among groups.
**Randomization test (≡ permutation test)**: A particular resampling technique that permutes the data points to obtain the comparison set of random outcomes, selecting each data point only once. 
- A randomization test is classified as random resampling without replacement, because the data point can no longer be drawn from the population.
### Significance for randomization tests
In the case of a null hypothesis, if the p-value is less than a significance level (such as 0.05), the difference is deemed significant. 
### Combinations for randomization tests
The number of ways to choose k items from a group of N data points is "N choose k", calculated as N!/k!(N−k)!
### Resampling: Bootstrapping
Randomly selects a set of data points, allowing the same data point to be selected more than once, to create an approximate sampling distribution.
- Data from different groups are not mixed. 
- **With replacement**: allowing selection more than once.
- **Assumptions**: Data is representative of the sample distribution.
## Wilcoxon rank-sum test
### Ranking
Orders the data such that for any two data points, one is greater than, less than, or equal to the other.
- *Ex: Given 3 data points 80, 75, and 99, a possible ranking is 1: 75, 2: 80, 3: 99. Ranking data can provide new insights into a sample population. Ranking data from two different randomly selected populations is the basis for some nonparametric statistical tests.*
- Statistical tests based on rank remove the necessity of assumptions of a normal distribution from the analysis of data. These methods: 
  - Are less powerful than the other nonparametric methods. 
  - Are useful in cases where assumptions about the distribution are clearly not possible. 
    - Distribution not normal (e.g. skewed or large outliers) 
    - Already ranked 
  - Remove information, such as the exact values of the data points. 
  - Simplify the remaining analysis. 
### Wilcoxon rank-sum test
- Can be performed using ranked data.
- Ignores the values of the original data and compares the sum of the two groups' ranks. 
- The test statistic for the Wilcoxon rank-sum test, W, is the minimum of the sum of the ranks for each group. 
  - *Ex: The sum of the ranks for the placebo group is 18.5, while the sum of the ranks for the painkiller group is 36.5. The test statistic is given by the smaller sum, so W = 18.5.*
- **Assumptions**:
  1. The two groups come from similar distributions.
  2. The two sets of data are independent.
### Kruskal-Wallis Test
#### Kruskal-Wallis Test
- Similar to Wilcoxon rank-sum test.
- Nonparametric equivalent to a one-way analysis of variance, and is an extention of the Wilcoxon rank-sum test to three or more groups of data.
- H0: All groups of data are drawn from the same distribution.
- H1: At least one group is drawn from a different distribution.
### Multiple Tests
#### Incorrect Rejection
In cases of multiple tests, the probability that at least one incorrect result is reported can be expressed based on the confidence level of the individual results. The family-wise error rate is the overall confidence level of multiple statistical tests due to type I errors. The significance of the k independent statistical tests is given by ̅α = 1 - (1-α_comparison )^k
- If the tests are not independent, the significance is given by:  
 ̅α ≤ kα_comparison
#### Techniques
The Bonferroni method sets a minimum critical value to reject each statistical test to assure a minimum significance level for a group of tests. *Ex: If the desired significance level is 0.05 for 5 independent tests, an individual test is rejected if the p-value for that test is less than 0.05/5 = 0.*
- Helps restrict type I errors
- More type II errors.
# Categorical Analysis
## Comparing samples having categorical data
- **Categorical data (≡ qualitative data)**: data that can only take on the value (usually a label) of one of several categories.
  - *Ex. A person's gender, seasons, and U.S. comparies are categorical varaibles. 
  - Two types of categorical data:
    - **Nominal**: No ordering, existing in name only, like apples, oranges, and grapes.
    - **Ordinal**: Have ordering, like disagree, neutral, and agree.
- Tables are often used to provide numerical summaries of categorical data.
  - **Contingency Table**: displays the number of observations in each category.
## Graphical displays of categorical data
- **Stacked bar chart**: a bar chart that depicts two or more groups on a single bar chart, with the proportion in each group having a different color in the bar.
## 2 samples, 2 categories: Fisher's exact test
### More on contingency tests
- **Fischer's exact test**: a method of calculating the exact p-value for contingency tables. 
  - **Assumptions**:
    - Row and column totals are fixed
    - If at least three of the totals are known, the 2x2 contingency table can be completed knowing only one of the four observations.
    - Calculated using hypergeometric distribution.
## 2 samples, 2 categories, large sample: Chi-squared test
### Chi-square tests and expected cell counts
- Approximation that is used when a sample size is large.
- For larger contingency tables.
- An alternative to the Fischer's excact test: Fischer's exact tests provides exact p-values b ut requires a great deal of computation
- **Use**: Calculates how unusual the oberved contingency table is under the null hypothesis. Compares the observed values in each cell of a contingecy table to the expected values.
- **Calculation**: row total * column total / overall total
## 3+ samples and/or 3+ categories: Chi-square test
### Why use chi-square test for 3+ populations, and/or 3+ categories?
- While Fisher's exact test can be used for variables with more than two categories, calculating all possible contingency tables quickly becomes infeasible.
- **Assumptions**: Expected cell counts are > 5 (if <5 use Fisher's exact test).
#### Chi-square test of independence
- Determines if there is a significant relationship between two nominal (categorical) categories.
  - H0: The two variables are independent.
  - Ha: The two variables are not independent.
#### Chi-square test of homogeneity
- Determines whether different samples come from the same population.
  - i.e. Determines if the distribution of one variable is the same across all cetgories of the other variables.
## 2 samples, 2 categories: relative risk and odds ratio
- Measures of the practical or clinical effect based on sample data.
- *e.g. Ex: A study concludes that a statistically significant difference exists in deaths from the SARS virus for a group receiving the anti-viral drug Ribavirin compared to those not receiving the drug. However, drugs have side effects and may be expensive. Thus, if the risk of death from SARS is not sufficiently reduced using Ribavirin, a patient might choose not to use the drug despite the statistical result.*
### Exposure vs. Outcome
- **Exposure variable**: predictor variable
  - *e.g. In a SARS study, researchers were intereted in whether the likelihood of death is different for those taking Ribavirin. The variable identifying whether the person takes the drug or not is the exposure variable*.
- **Outcome variable**: response variable or the variable the study attemps to predict
- E1 and E2 (refer to risk measures table): the categories for the exposure variable; risk for the E1 group is compared to the risk for the E2 group.
  - E1 = exposed group.
  - *Ex. If gender is the exposure variable and E1 is defined as males, the risk of the outcome in males is compared to the risk in females.
- D1 and D2 are categories for the outcome variable.
### Risk Ratio (≡ relative risk)
- **Risk**: probability of the outcome occurring.
  - RE1 = a/a+b
  - RE2 = c/c+d
- **Risk ratio (or relative risk):** ratio of the risks of an outfome for two groups. The estimated risk ratio (RR) of outcome D1 occurring is:
  - RR = RE1/RE2 = (a/a=b)/(c/c+d)
  - An RR of 1 = estimated risk of the outcome is the same in the two groups.
    - RR of 2 = estimated risk in the exposed group is twice that of the unexposed
    - RR of 1/2 = estimated risk of the exposed group is half that of the unexposed.
### Odds Ratio (OR)
- **Odds**: the ratio of the probability that the event occurs to the probability that the event does not occur.
  - Odds = p/(1-p), where *p* is the probability of the even occuring. 
    - *Ex. The probability that a cornea transplant is successful (no rejection) is 0.8. The odds of success are **odds** = 0.8/(1-0.8) = 0.8/0.2 = 4/1 = 4.
    - The probability of the otucome, D1, for the first exposure group E1, is the risk previously estimated as RE1= a/a=b. 
    - The probaility D1 does not occure in the E1 group is 1-RE1 or b/a+b. The odds are shown below, which is similarly computed for the second exposure group E2.
      - OE1 = (a/a+b)/(b/a+b) = a/b
      - OE2 = (c/c+d)/(d/c+d) = c/d
    - **Odds ratio (OR): ratio of the odds of an outcome for two groups. The estimated odds ratio outcome D1 occurring is:
      - OR = OE1/OE2 = (a/b)/(c/d) = a.d/b.c 
      - OR of 1 = estimated odds of the outcome are the same in both groups.
      - OR of 2 = estimated odds in the exposed group are twice that of the unexposed.
      - OR of 1/2 = estimated odds in the exposed group are half that of the unexposed.
###  Using risk and odds ratios
Risk ratio is generally perferred over the odds ratio, because people usually understand risks or probabilities better tahn odds.
- When to choose odds ratio:
  - **Case-control studies**: A case-control study compares subjects who have an outcome of interest, referred to as cases, with a pre-selected number of subjects who do not have the outcome, referred to as controls.
    -	The risk ratio is not appropriate in case-control studies because the prevalence of the disease is not the same as the prevalence of the disease among people in the study. Thus, the risk estimates are not correct.
    - *Ex: 50 patients with pancreatic cancer are identified as cases at a cancer center. 50 patients without pancreatic cancer are randomly selected from other hospital patients to act as controls. Pancreatic cancer cases are 50% of the study subjects, which is much higher than the true risk of pancreatic cancer.*
  - **More complicated data analysis**: Estimates of the risk ratio are often not available or appropriate in studies with more than 2 categories for the predictor, or more than one predictor variable. Logistic regression, covered in another chapter, is useful in such settings and produces estimates of the odds ratio.
#### Useful facts about the risk ratio and odds ratio
- Odds ratio makes the difference in the groups appear greater than risk ratio.
- When the rate of occurrence of the outcome is high in either group, the odds ratio is much further from 1 than the risk ratio.
- Odds ratio is a reasonable approximation of the risk ratio when the prevalence of the outcome is low.
# Principal Component Analysis
## Introduction to PCA
### Components
PCA combines interdependent variables into new variables to simplify subsequent analysis.
- *Ex: A university may wish to predict which freshman applicants will succeed academically based on predictor variables of grade point average (GPA), standardized exam scores, amount of volunteer service, number of club memberships, and rating of the applicant's essay. Intuitively, noting that GPA and exam scores are highly correlated, one might just merge those variables into a new variable, perhaps called "academic score." Principal component analysis doesn't combine variables, but does something similar via use of "components."*.
- A table showing correlations between every variable pair can help in reducing predictor variables into components. \
  - Correlation values are used to calculate components. 
  - Components are not simple groupings of correlated data, but are weighted combinations of predictor variables. The weights of the predictor variables in the components is determined by all of the correlations between the predictor variables.
### Matrix plots
A matrix plot illustrates, via a scatter plot, every pairing of the original variables in a data set. In a matrix plot, each row has the same variable along the y-axis, and each column has the same variable along the x-axis. Thus, a matrix plot shows interdependence of every possible pair of variables. 
### Principal component analysis
Transforms variables into possibly fewer components to simplify subsequent analyses.
- **Goal of PCA**: is to maximize the data variability along as few components as possible.
### Eigenvector
Non-zero vector v that, when multiplied with the matrix, results in a vector that is a scalar multiple of v.
### Finding Eigenvalues
An eigenvalue is the change in the vector length after an eigenvector is multiplied by a matrix. 
- In PCA, the eigenvector with the largest eigenvalue becomes the first principal component, the second largest becomes the second, etc. 
- Each component's eigenvalue is that component's variability. 
- A = λ[I]
  - A = matrix
  - λ = eigenvalue
  - I = identity matrix
- det|A - λI| = 0  
- The number of eigenvalues = the number of equations 
  - *e.g. A matrix with 2x2 elements must have 2 eigenvalues, a 3x3 matrix has 3 eigenvalues.*
### Finding eigenvectors
 [1.0 0.9][v1,1] = λ[v1,1]  
 [0.9 1.0][v1,2]....[v1,2]  
First eigenvalue is λ = 1.9  
1.0(v1,1) + 0.9(v1,2) = 1.9(v1,1)  
0.9(v1,1) + 1.0(v1,2) = 1.9(v1,2)  
0.9(v1,2) = 0.9(v1,1)  
v1,1 = v1,2
### Creating principal components in two dimensions
The first principal component is created from the eigenvector that comes from the largest eigenvalue. The second principal component can be found using the next largest eigenvalue and eigenvector. Ex: The principal components for the example above are given by the two equations below.
- *Assume that one of the input variables had a value X1 = 0.5 and X2 = 0.3. What are hte principal component values for a data point created using the principal components.
  - The first principal component is Z1 = X1 + X2 = 0.5 + 0.3 = 0.8
  - The second principal component is Z2 = -X1 + X2 = -0.5 + 0.3 = -0.2
## Extending PCA to more variables
### Three variables
Principal component analysis works best in problems with large numbers of variables. A three variable example of principal component analysis is not significantly different from a two variable example.  

A best practice is to **standardize variables** when conducting a principal component analysis. 
  - **Standardized variable**: is a variable that has been adjusted to have a mean of zero and a standard deviation of one.  
    - Standardizing variables is accomplished by finding the mean and standard deviation of the input variables. The mean is then subtracted from each of the original input variable values. These new values are divided by the standard deviation of the sample to rescale the distribution. Standardizing all variables in the data set keeps the same correlation matrix and forces the input variables to be on similar scales. 
### Principal component analysis for many variables
Principal component analysis is best used with data with many input variables with unclear relations. The method of calculating principal components does not change with increasing numbers of input variables. First, the eigenvalues and the corresponding eigenvectors should be calculated. Then, the principal components are calculated, and the data is transformed into the principal components.
## Determining the number of components
### Selecting components
- **Advantage of PCA**: Reducing the number of variables in a large data set.
- Using a correlation matrix and standardized variables means that any eigenvalue > 1 = more variability in the data than a single variable. 
- An eigenvalue < 1 = less variability than a single variable. 
- Keeping eigenvalues greater than 1 is a good practice.
### Scree plot
A scree plot is a scatterplot of eigenvalues for each principal component, commonly used to visually select how many principal components to keep, by keeping components before the bend of the curve where eigenvalues level off.
## Interpreting principal components
### Covariance matrix
**Use**: If several variables' ranges don't vary much but one variable constantly gets the same value, standardization will over-emphasize small changes in those several variables.
### Understanding principal components
The individual weighting of each input variable in the principal components aids in the interpretation of each principal component. The weighting of each variable in the principal components shows the strength of the effect that the original variable has on the principal component. 
  - *Ex: A college admissions committee identified four criteria that determine whether a student will be offered admissions.*
  - **Calculating the weight of input variable**: if we are calculating the first principle component, Eigenvalue 1/ Sum(eigenvalues 2-5).
- A **principal component loading plot** displays the weight of each input variable between a pair of principal components.
The loading plot is created from two principal components. The weight of an input variable for each principal component is used as the coordinates in the scatter plot. 
  - *Ex: The weight of student GPA is 0.5083537 for the first principal component and 0.4683627 for the second principal component. The loading plot draws a line from the origin to each coordinate representing an input variable. The figure below provides a way to visualize the importance of each variable to a principal component and can provide some insight into the meaning of each principal component.*
### Factor loadings
The correlation between the original data and the new principal component. The factor loadings can be obtained by calculating the correlation coefficients between the principal component and each of the input variables.
# Multiple Regression
## The multiple linear regression model
### Elements of the multiple regression model
A multiple linear regression is a way to model the linear relationship between one quantitative response variable and one or more predictor variables.
- **Response variable**: variable being modeled or predicted (Y)
- **Predictor variable**: variables used to predict the response (X1, X2, X3... Xn)
- **Regression error term (ϵ)**: actual value of *Y* - expected value of *Y*.
  - ϵ is positive: actual Y > expected Y
  - ϵ is negative: actual Y < expected Y
  - ϵ is zero: actual Y = expected Y
## Regression diagnostics
A multiple linear regression model should generally only be used if a reasonable chance exists that the assumptions hold in the population:
  - Linear relationship between independent and dependent variables.
  - Errors between observed and predictced values should be normally distributed (using the Kolmogorov Smirnov test).
  - No multicollinearity in the data (independent variables should not be highly correlated to each other).
    - Multicollinarity may be checked using the following methods:
      1. Correlation matrix: magnitude of the correlation coefficients should be < 0.80
      2. Variance Inflation Factor (VIF): should be < 10
  - Homoscedasticity (no clear pattern in the distribution; should not be cone shaped = heteroscedastic)
### Assessing the regression assumption with residual plots
1. The **"mean of zero" assumption**: Mean of residuals should ≈ 0 for all predictor variables.
2. The **"constant variance" assumption (homoscedasticity)**: The variance of residuals for each fixed value of the horizontal quantity should remain ≈ constant all the way across the plot.
3. The **"normality" assumption**: A normal probability plot of the residuals has the ordered residuals plotted on the vertical axis and theoretical normal quantiles plotted on the horizontal axis. If the plotted points lie reasonably close to the diagonal line on the plot then one can conclude that the normality assumption holds.
4. **Assessing the "independence" assumption**: The most common form of dependence that can affect regression models is time dependence. Such time dependence can be assessed if the data was collected in time order and that information is available. Otherwise, assessing the independence assumption is difficult. However, if a variable that tracks time is available, a scatterplot with the residuals on the vertical axis and time order on the horizontal axis enables assessment of the independence assumption. If one scans the plot from left to right and the residuals tend to track one another more than would be expected by chance, then time dependence in the errors may exist and the independence assumption may not hold. If time dependence exists in the errors, the errors are said to be autocorrelated. If the residuals seem random, then one can conclude that the independence assumption holds.
5. Sample size > 30
### Influential observations
- **Outliers**: Observation's Y value is much larger than predicated by the model, or much smaller than predicted by the model.
- **High leverage**: Extreme combination of values that might be particularly high or low values for all the predictors or a combination of predictor values that is relatively unusual.
- **Multicollinearity**
### Residual standard error, R-squared and adjusted R-squared
#### Residual standard error
- Square root of the residual mean square s = √MSE
- Estimates the standard deviation of the residuals.
- Smaller residual errors are closer to the actual future value of Y.
#### R-squared
- Proportion of the total variation in the response variable, Y that is accounted for by the linear regression model.
#### Adjusted R-squared
- Allows alternatie models for the same response variable to be compared.
- Tends to only increase when a worthwhile predictor term is added to the model.
- A model with a higher value of adjusted R-squared would be preferred to a model with a lower value.
## Categorical predictors
### Categorical predictor variables
A categorical predictor variable has qualitative values representing one of a finite number of categories. 
- *Ex: A variable X1 representing species, whose possible values are human or dolphin.*
### Log-transformed response variable
A **logarithmic response variable transformation** is used when higher values tend to be more spread out than lower values.
### Model with an interaction term
An **interaction term** is two predictor variables multiplied together and used as an additional predictor term in a multiple linear regression model.
# Logistic Regression
## Introduction to the logistic regression model
### Binary Responses
A binary response variable is a response variable that has only two possible outcomes. Ex: Researchers wish to develop a model to predict whether a patient rejects a kidney transplant. The outcome is binary, because the patient either rejects the kidney or not. A binary response variable typically uses 0 and 1 to represent the two possible outcomes. Ex: Y = 1 if the patient rejects the kidney and 0 if the patient does not reject the kidney.
- *Ex.As in linear regression, interest is in modeling or predicting the binary response variable using one (or more) predictor variables. Ex: The binary response is whether a retired baseball player was inducted into the baseball Hall of Fame, and the predictor variables are career performance statistics such as hits, home runs, and runs scored. The binary response is a 1 if the player is in the Hall of Fame and a 0 if not. The plot below shows the Hall of Fame status for the predictor variable Hits (number of hits in the player's career).*
### The expected value of a binary response
The **population simple linear regression function** is E(Y) = β0 + β1X, where β0 and β1 are regression parameters. 
### The population logistic regression model
- S-curve
  - Multiple functions could model this "S" shape. The logistic regression model is a popular choice.
## Wald Tests
### Wald Tests of logistic regression parameters
### Likelihood Ratio (LR) test
Compares two nested models, which means that all predictors in the smaller model are contained in the second, larger, model.
- *Ex: A model to predict heart disease includes two predictors: age and sex. The LR test is used to compare the two predictor model to a second model, which includes age and sex plus two additional predictors: heart rate and blood pressure. The null hypothesis is that all the additional parameters are zero, and the alternative hypothesis is at least one parameter is not zero. Failing to reject the null hypothesis using the LR test suggests that none of the additional variables in the second model are useful in predicting the response.*
### Overall model LR test
The LR test can replace the F test for a linear regression model. The overall model LR test compares the model with predictor variables to a model with only the intercept. Thus, the overall model test is a special case of the general LR test. Two models that can be compared are a smaller model with only the intercept parameter β0 and a larger model with both intercept and slope parameters β0 and β1. In this case, the LR test and Wald test have the same hypotheses because only one predictor is added to the model. However, unlike the F and t tests for linear regression, the LR and Wald tests do not provide the exact same results. In general, the two tests produce very similar results. In rare cases where the conclusions differ, the LR test is preferred. 
### Hosmer-Lemeshow goodness of fit (GOF) test
Residual plots provide information about poor predictions. If a large number of observations are poorly fit, the model would not be very useful. The Hosmer-Lemeshow goodness of fit (GOF) test assesses whether the model predictions are close to the observed values of Y, which are either 0 or 1. The test considers groups of observations based on predicted probabilities. For a given group, the expected number of values with Y=1 is compared to the observed number. The null hypothesis of the test is that the model fits the data well. The test statistic adds up quantities based on the differences in observed and expected values, which makes the GOF test similar to a standard chi-square test. Thus, a poorly fit model gives rise to a large test statistic, which leads to the rejection of the null hypothesis.
### Influential observations
- Outlier
- High leverage observation
### Classification using logistic regression
In some applications, the goal of the logistic regression model is to predict whether the binary response Y takes on a value of 0 or 1. Predicting the category of a categorical response is known as classification. When classification is the goal of the analysis, a cut point is chosen to determine which category to predict. Ex: A player with predicted probability at or above the cut point of 0.5 can be classified as a Hall of Fame player, Y=1. Players with predicted probabilities below 0.5 can be classified as not in the Hall of Fame, Y=0. The choice of cut point impacts how well the model classifies, but the types of algorithms for choosing the cut point are beyond the scope of this material. A 2x2 classification table is useful for assessing how well the model classifies. The rows of the table are the classification categories based on the model, and the columns are the observed categories. Measures commonly used to help evaluate the classification results include sensitivity, specificity, and the area under the ROC curve. A summary of each measure is given below.
-	**Sensitivity** is the percentage of correctly classified observations with the desired outcome, Y=1. Ex: Percentage of players at or above the probability cut point, and thus classified as Hall of Famers, who are actually in the Hall of Fame.
-	**Specificity** is the percentage of correctly classified observations without the desired outcome, Y=0. Ex: Percentage of players below the cut point, and thus classified by the model as not Hall of Famers, who are actually not in the Hall of Fame.
-	The **ROC (Receiver Operating Characteristic) curve** plots the sensitivity vs. 1 minus the specificity for all possible cut points. The area under the ROC curve, referred to as AUC, is an indicator of how well the model distinguishes between a Y=0 and Y=1. An AUC of 0.5 means that the model performs better than chance. As a general rule, AUC > 0.7 is acceptable, AUC > 0.8 is excellent, and AUC > 0.9 is outstanding.
