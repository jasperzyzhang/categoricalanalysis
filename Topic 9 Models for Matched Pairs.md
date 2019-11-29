# Topic 9: Models for Matched Pairs

### Nov28

## Questions to be solved

1. Pp 20 interpretation from othose odds ratios

## Models for Matched Pairs

1. Responses in the two samples are statistically dependent.

   eg. sample from two different time points

2. **McNemar's Test: test of marginal homogeneity**

3. $\pi_{ab}$ the probability of outcome a for the D 2004 observation and b for D 2008

4. $n_{ab}$: the number of such paris in a sample of n matched pairs with $p_{ab} = n_{ab}/n$ the sample proportion

5. $p_{a+}$is the proportion in cate a for observagtion 1. and $p_{+a}$ is the corresponding proportion for observation 2, compare these two marginal proportions 

6. **Marginal Homogeneity**: $\pi_{1+} = \pi_{+1}$ then $\pi_{2+} = \pi_{+2}$ <=> $\pi_{12} = \pi_{21}$

7. $H_0: \pi_{12} = \pi_{21}$: **Hypothesis of Symmetry**

   1. Note the diagonal elements are not important since they correspond to the proportions of respondents whose approval/disapproval have stayed the same over time.

8. Total number of observations in the off-diagonal is fixed

   1. $n^{*} = n_{12} + n_{21}$.
   2. $n_{12}, n_{21}$ ~ Bin(n*, 0.5)
   3. $z = \frac{\frac{n_{12}}{n^{*}} - 0.5}{\sqrt{0.5(1-0.5)/n^{*}}} = \frac{n_{12} - n_{21}}{\sqrt{n_{12} + n_{21}}}$ 
   4. 0.5 n* is the expected count for n12 under H0
   5. estimated proportion n12/n* , and the variance of the proportion under H0 is  0.5(1-0.5)/n* .
   6. Under H0, n*>=10,z is approx N(0,1). p-value for a two-sided alternative is doubled. 2P(Z>=z)
   7. $z^2$ to $\chi_1^2$ This test is valid under geneal multinomial sampling when **n\* is not fixed but n is.**

9. **small** sample size example:

   Z^2 = (54-16)^2/ (54+ 16) = 20.63, Pvalue is  $P(\chi_1^2 \geq 20.63 ) = 0.000006$ : **Very strong evidence of a shift in the democraft direction**.

10. **Difference between the marginal proportions**: 

    1. $d = \pi_{1+} - \pi_{+1} = \pi_{12} - \pi_{21}$

    2. $\hat{d} = \frac{n_{12}}{n} - \frac{n_{21}}{n}$

    3. $V(\hat{d}) = n^{-2}V(n_{12}-n_{21}) = n^{-1}[\pi_{12}(1-\pi_{12}) + \pi_{21}(1-\pi_{21}) + 2\pi_{12}\pi_{21}]$

    ​           $ = n^{-1}[\frac{n_{12}}{n}(1 - \frac{n_{12}}{n}) + \frac{n_{21}}{n}(1 - \frac{n_{21}}{n}) + 2\frac{n_{12}n_{21}}{n^2}]$

    4. 95%CI is $\hat{d} \pm 1.96 \sqrt{\hat{V}(\hat{d})}$

11. Male and Female example
    1. Male:95CI for $\pi_{1+} - \pi_{+1}$ = 0.088 $\pm$ 1.96(0.0189) = (0.051, 0.125) We infer that the population percentage of males voting D increased by between 5% and 13%
    2. Female: (0.106, 0.171), shift toward D seems that it may be greater for females than males.
    3. 95CI for a difference of differences: (0.138 - 0.088) $\pm$ 1.96 $\sqrt{(0.0189)^2 + (0.0167)^2}$ = (0.001, 0.1) There is evidence of a greater shift for females than males, as much as 10%.
12. **Increased precision**
    1. Dependent samples can help improve the precision of statistical inferences for **Within-Subject Effects**
    2. **Substaintial **when samples are highly correlated
13. 









