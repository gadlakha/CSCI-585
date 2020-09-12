Q1:
Linear Regression Model
class in the below equation represents Median Home Price(MEDV)

class/MEDV =

     -0.1084 * CRIM +
      0.0458 * ZN +
      2.7187 * CHAS=1 +
    -17.376  * NOX +
      3.8016 * RM +
     -1.4927 * DIS +
      0.2996 * RAD +
     -0.0118 * TAX +
     -0.9465 * PTRATIO +
      0.0093 * B +
     -0.5226 * LSTAT +
     36.3411

No of terms in the equation=12 terms (including constant term)

Attributes/terms not included are : 2
INDUS: Proportion of non-retail business acres per town 
AGE:Proportion of owner-occupied units built prior to 1940

Why?

Attribute selection is a method to improve the performance of the model by selecting subset of the variables that is a "better" estimator of the target 
variable.Since,by increasing the amount of attributes, we can always increase the R² value, but this may not be a good decision because it may lead to 
overfitting.INDUS and AGE variables do not provide contribution to explain the variance in the MEDV Variable, thus to the total R² as well 
i.e. coorelation between the MEDV and these two variables is not significant,and are among the lowest standardized regression coefficients, leading to their elimination in the linear 
regression equation.Method M5 selection algorithm has been used for the attribute selection which initally starts  with selection of full set of features and then,the feature
with the lowest standardized regression coefficient is marked for removal and retrieve significant variables for the equation.

Interpreting the equation:

-The sign of a regression coefficient tells us whether there is a positive or negative correlation between each independent variable and the dependent variable.

-A positive coefficient tells us that if the value of the independent variable increases, the  dependent variable also tends to increase. 

-A negative coefficient tells us that if the independent variable increases, the dependent variable tends to decrease.

-The coefficient value indicates that how much does the mean of the dependent variable changes with one-unit shift in the independent variable while not changing the other variables.
 Keeping other variables unchanged is required because it allows us to visualise the effect of each variable in isolation from the others.

Thus, 
1. On increasing 1 unit of CRIM(per capita crime rate by town) , MEDV(median value of owner-occupied homes in \$1000s) would decrease by 0.1084 unit. 

2. On increasing 1 unit of ZN(proportion of residential land zoned for lots over 25,000 sq.ft.), MEDV(median value of owner-occupied homes in \$1000s) would
   also increase by 0.0458  unit.

3. If Charles River dummy variable = 1 i.e.if tract bounds river, MEDV(median value of owner-occupied homes in \$1000s.) would also increase by 2.7187 units.

4. On increasing 1 unit of NOX-nitrogen oxides concentration (parts per 10 million), MEDV(median value of owner-occupied homes in \$1000s) would decrease by 17.376 units.

5. On increasing 1 unit of RM-average number of rooms per dwelling,MEDV(median value of owner-occupied homes in \$1000s) would also increase by 3.8016 unit.

6. On increasing 1 unit of DIS-weighted mean of distances to five Boston employment centres,MEDV(median value of owner-occupied homes in \$1000s) would decrease by 
   1.4927 units.

7. On increasing 1 unit of RAD -index of accessibility to radial highways, MEDV(median value of owner-occupied homes in \$1000s) would increase by 0.2996 units.

8. On increasing 1 unit of TAX -full-value property-tax rate per \$10,000, MEDV(median value of owner-occupied homes in \$1000s) would decrease by 0.0118 units.

9. On increasing 1 unit of PTRATIO i.e. pupil-teacher ratio by town, MEDV(median value of owner-occupied homes in \$1000s) would decrease by 0.9465 units.

10.On increasing 1 unit of B i.e.1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town,MEDV(median value of owner-occupied homes in \$1000s) would increase by  
   0.0093 units.

11. On increasing 1 unit of LSAT-% lower status of the population,MEDV(median value of owner-occupied homes in \$1000s) would decrease by 0.5226 units.

Intercept=36.3411 tells us what the MEDV value  would be if all attribute values are 0.

------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
Q2:
1. As per the instructions on Piazza @1030-The precision of the learning rate and momentum can be 1 decimal place.
RMSE (with learning rate=0.2 , momentum=0.1 and no other parameter changed)=   2.5856 (Screenshot attached of this one)

2. If 2 or more decimal places taken into account and only learning rate and momentum changed:
RMSE (with learning rate=0.221 , momentum=0.16 and no other parameter changed)=   2.5095

3. If other parameters updated
RMSE (with learning rate=0.1 , momentum=0.14 and Hidden Layers-14,2 and no of epoch=5600)=   1.4979

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
Q3:

Linear Regression Equation:
num_rings= -0.825* sex=I + 0.058*sex=M + (-0.458)*length+ 11.075 * diameter + 10.762 * height +8.975 * whole_weight + (-19.787)  * shucked_weight +(-10.582) * viscera_weight + 8.742 * shell_weight + 3.895 

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
Q5:

Cluster 0: 1388 items
Cluster 1: 499 items
Cluster 2: 448 items
Cluster 3: 22 items
Cluster 4: 172 items
Cluster 5: 1648 items
Total number of items: 4177
------------------------------------------------------------------------------------------------------------------------------------------------------------
Q6:

Linear Regression Equation:
num_rings= - 11.933 * length + 25.766 * diameter + 20.358 * height + 2.836