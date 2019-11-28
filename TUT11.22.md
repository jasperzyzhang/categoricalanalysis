## TUT11.22

a

| Analysis of Maximum Likelihood Estimates |      |      |          |                |                 |            |
| :--------------------------------------- | :--- | ---: | -------: | -------------: | --------------: | ---------: |
| Parameter                                |      |   DF | Estimate | Standard Error | Wald Chi-Square | Pr > ChiSq |
| Intercept                                |      |    1 |   1.4246 |         0.8287 |          2.9554 |     0.0856 |
| control                                  |      |    1 |  -0.9594 |         0.2047 |         21.9760 |     <.0001 |
| problems                                 |      |    1 |   0.2956 |         0.0505 |         34.3081 |     <.0001 |
| sevent                                   |      |    1 |   0.3557 |         0.0804 |         19.5912 |     <.0001 |
| cohes                                    |      |    1 |  -0.1782 |         0.0373 |         22.8583 |     <.0001 |
| time                                     | 1    |    1 |   0.3566 |         0.2055 |          3.0116 |     0.0827 |
| time                                     | 2    |    1 |   0.2499 |         0.2041 |          1.4993 |     0.2208 |
| time                                     | 3    |    0 |        0 |              . |               . |          . |

bint = 142 pval = 0.08

bcontrol = -0,95 p = 10^-4

bproblems = 0.28 pval = 10^-4

bsevent = 0.35 pal <10^-4



becohes = -0,17 pval <10^04

bTime = 1VS3 = 0.35 pval = 0.08

bTime = 2VS3 - 0.25 pval = 0.22



b describe effects of predictors in a , effect of time on ptsd

ORsevent = 1.48 95CI = 1.22 1.67

ORcohes= 0.84 95ci = 0.78 0.90



Control: the odds ratio of ptsd for each additional control is 

e^-0.95 = 0.38(95%CI = (0.25, 0.32))

Problem the odds ratio of ptsd for each additional problem is 

e^0.29 = 1.34 ( 95CI = 1.22 1.48))



Time is not significant predict on ptsd, p val > 0.05



Solution c d 

| Solutions for Fixed Effects |      | $$\beta'$$ |                |      |         |            |
| :-------------------------- | :--- | ---------: | -------------: | ---: | ------: | ---------: |
| Effect                      | time |   Estimate | Standard Error |   DF | t Value | Pr > \|t\| |
| Intercept                   |      |     2.3588 |         1.1838 |  314 |    1.99 |     0.0472 |
| control                     |      |    -1.3239 |         0.2969 |  627 |   -4.46 |     <.0001 |
| problems                    |      |     0.3545 |        0.07049 |  627 |    5.03 |     <.0001 |
| sevent                      |      |     0.4016 |         0.1086 |  627 |    3.70 |     0.0002 |
| cohes                       |      |    -0.2476 |        0.06249 |  627 |   -3.96 |     <.0001 |
| time                        | 1    |     0.5258 |         0.2518 |  627 |    2.09 |     0.0371 |
| time                        | 2    |     0.3513 |         0.2394 |  627 |    1.47 |     0.1428 |
| time                        | 3    |          0 |              . |    . |       . |          . |



coefficents Inflated

The B-values in the model with cluster effect are larger than those in the null naive cluster less effects.

Hence, ignoring the clustering structure data yields to under estimation of the true effect size.