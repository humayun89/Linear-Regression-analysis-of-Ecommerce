# Linear-Regression-analysis-of-Ecommerce

                           Email  ... Yearly Amount Spent
0      mstephenson@fernandez.com  ...          587.951054
1              hduke@hotmail.com  ...          392.204933
2               pallen@yahoo.com  ...          487.547505
3        riverarebecca@gmail.com  ...          581.852344
4  mstephens@davidson-herman.com  ...          599.406092

[5 rows x 8 columns]
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 500 entries, 0 to 499
Data columns (total 8 columns):
 #   Column                Non-Null Count  Dtype  
---  ------                --------------  -----  
 0   Email                 500 non-null    object 
 1   Address               500 non-null    object 
 2   Avatar                500 non-null    object 
 3   Avg. Session Length   500 non-null    float64
 4   Time on App           500 non-null    float64
 5   Time on Website       500 non-null    float64
 6   Length of Membership  500 non-null    float64
 7   Yearly Amount Spent   500 non-null    float64
dtypes: float64(5), object(3)
memory usage: 31.4+ KB
       Avg. Session Length  ...  Yearly Amount Spent
count           500.000000  ...           500.000000
mean             33.053194  ...           499.314038
std               0.992563  ...            79.314782
min              29.532429  ...           256.670582
25%              32.341822  ...           445.038277
50%              33.082008  ...           498.887875
75%              33.711985  ...           549.313828
max              36.139662  ...           765.518462

[8 rows x 5 columns]
                           Coef
Avg. Session Length   25.724256
Time on App           38.597135
Time on Website        0.459148
Length of Membership  61.674732
                             OLS Regression Results                            
===============================================================================
Dep. Variable:     Yearly Amount Spent   R-squared:                       0.985
Model:                             OLS   Adj. R-squared:                  0.985
Method:                  Least Squares   F-statistic:                     5825.
Date:                 Sun, 27 Oct 2024   Prob (F-statistic):          3.46e-315
Time:                         05:03:00   Log-Likelihood:                -1296.2
No. Observations:                  350   AIC:                             2602.
Df Residuals:                      345   BIC:                             2622.
Df Model:                            4                                         
Covariance Type:             nonrobust                                         
========================================================================================
                           coef    std err          t      P>|t|      [0.025      0.975]
----------------------------------------------------------------------------------------
const                -1050.6537     26.458    -39.710      0.000   -1102.694    -998.614
Avg. Session Length     25.7243      0.534     48.137      0.000      24.673      26.775
Time on App             38.5971      0.528     73.045      0.000      37.558      39.636
Time on Website          0.4591      0.520      0.884      0.377      -0.563       1.481
Length of Membership    61.6747      0.516    119.540      0.000      60.660      62.690
==============================================================================
Omnibus:                        1.523   Durbin-Watson:                   2.024
Prob(Omnibus):                  0.467   Jarque-Bera (JB):                1.262
Skew:                          -0.108   Prob(JB):                        0.532
Kurtosis:                       3.199   Cond. No.                     2.56e+03
==============================================================================

Notes:
[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.
[2] The condition number is large, 2.56e+03. This might indicate that there are
strong multicollinearity or other numerical problems.
Mean Absolute Error: 8.426091641432116
Mean Squared Error: 103.91554136503333
Root Mean Squared Error: 10.193897260863155
