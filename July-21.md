# July 2021

## 5th July 2021

* When ideatating during an OKR, don't ask the question directly related to the OKR.
* Think of a question that will help direct the discussion in the right direction.
* Don't think of surface level questions.

## 6th July 2021: What is Analytics?

* Analytics:
  * to figure out patterns
  * bulding blocks of data analytics ⟶ metrics (something you can measure)
  * use metrics to take a qualitative thing and give a quantitative answer to
* Types of metrics
  * Scale Neutral vs Unneutral:
    * The first doesn't change with an increases number of observations. e.g. Average height of individuals would be the almost the same for 1000 vs 100000 people
    * The second does. e.g. Revenue generated from 1000 vs 100000 customers
  * Comparing metrics - absolutely or relatively
  * Based on when the effect is visible. e.g. an acquistion project (long term) vs a retention project (readily observable)
* Proxy metrics - sometimes if you don't have time to measure long term metrics, you use a metric that will indicate something similar. e.g. what can you measure that'll tell you that you're lead towards retention?
* Benchmark your metrics against something to convey the scale of the change
* Relationship among variables:
  * How are 2 or more things related with each other?
  * Changing which thing influences the other
    * What is the causing factor and what is the effective factor?
  * Correlation: "expresses the extent to which two variables are linearly related (meaning they change together at a constant rate)."
  * Sometimes, you need to find whether it's a direct effect or an indirect effect. If it's indirect, you need to identify the links.
  * It's difficult to identify the causing factor and effecting factor. e.g. does unhealthiness lead to laziness or vice versa?
  * To find cause and effect in a controlled environment ⟶ experiment
* Distributions
  * How spread out your data is?
  * Measures of central tendency = mean, median, mode (mean ⟶ expected value)
* Experimentation
  * Why sample the population?
    * Sample will have errors
    * But it's expensive to take entire population - can't sample everyone (and simultaneously)
    * An Ideal sample should be representative of your population
  * Types of sampling bias [Source](https://www.scribbr.com/methodology/sampling-bias/), e.g.
    * Selection
    * Supervisorship
    * Self-selection
    * Undercoverage
    * Non-response

* Permutations: Fancy way of saying how things are arranged

## 10th July 2021: Quality check

* Data Analysis isn't just about writing code/queries, but also about what output you generated is correct.
* Always QC your data against a known source of truth.

## 17th July 2021

### [Random Sampling vs Random Assignment](https://www.statisticssolutions.com/random-sampling-vs-random-assignment)

* random sampling is used to ensure the representativeness of the sample (i.e., external validity)
  * a sample is only truly random if all individuals in the population have an equal probability of being selected to participate in the study
  * In practice, very few research studies use “true” random sampling because it is usually not feasible to ensure that all individuals in the population have an equal chance of being selected.
  * For this reason, it is especially important to avoid using the term “random sample” if your study uses a nonprobability sampling method (such as convenience sampling).
* Random assignment refers to the method you use to place participants into groups in an experimental study
  * Ideally, you would want to randomly assign the participants to be in the experimental group or the control group, meaning that each participant has an equal probability of being placed in the experimental or control group.
  * This helps ensure that there are no systematic differences between the groups before the treatment (e.g., the aspirin or placebo) is given to the participants.

### Collecting and summarizing data (Penn State: Stat500)

* Space is left between bars in a bar chart to emphasize their's no ordering between them. Bar chart ⟶ categorical variables; Histogram ⟶ quantitative variables.
* Sample = represenative of the population.
* Unless outlier data points are known mistakes, one should not remove them from the data set! One should keep the extreme points and use more resistant measures such as sample median to estimate the population median.
* For many applied statistical methods, a required assumption is that the data is normal, or very near bell-shaped. When the data is not normal, we will need to transform the data to normality using numerous transformation techniques e.g. logarithmic transformation.
* Skewness is the measure of the degree of asymmetry
* Measure of central tendency don't tell the whole story, for this we use:
  * measures of position (e.g. percentiles - where a certain percentage of data lies) and
  * measures of variability (e.g. range, IQR, SD, Variance - to describe the spread)
  * ... to help paint a more concise picture of what's going on with your data.
* IQR = resistant to outliers, since it's the middle 50% of the data
* When calculating sample variance, we divide by `n-1` instead of `n`, to give it a special property that we call an "unbiased estimator".
* standard deviation is approximately equal to the range of the data divided by 4.
  * considering a normal distribution, 95% of the data is within two standard deviations of the mean
  * For a relatively small sample, the range is likely to based on data from within this 95% range
* Adding constant to every value doesn't change any variability measures
* Multiplying a random variable by a constant:
  * increases the variance by the square of the constant.
  * increases SD, range, mean by SD * constant
