# capstone_project

Author : Fahmi Afri

### project overview

Finding the related features affecting the used car price .
The features :
Engine Capacity(cc) 
Engine Type - Petrol , Diesel , Hybrid , LPG , CNG
Year (1990-2021)
Mileage (kms)
Transmission type - automatic , manual 


### The Data

This data required me to do Regression analysis ,i.e : how much is this used car ?

As a Data Science lifecycle , i performed :

Business understanding - identifying the main concern of a buyer.

Data mining - collecting data suitable with the business problem.

Data resource :  https://www.kaggle.com/datasets/ebrahimhaquebhatti/75000-used-cars-dataset-with-specifications

Data cleaning - removing any inconsistencies in dataset i.e duplicate , missing values , outliers, standardization and normalization

Data exploration - building graph for better understanding of the data .

Feature engineer - manipulate features for better fit for our modeling .

Predictive model - performed Linear Regression to train , evaluate the performance and creating predictions .


## Conclusions

As a industry specialist, i have been working with cars for almost 6 years , i have reduced the range for Mileage(kms) and Years due to few reasons .

1990-2021 is still in acceptable range of year because of spare parts availability , workshop options , wear and tear of factory built , comfortability and newer technology .

Being a used car , having a 1km on the clock does not really indicate correctly and this may possibly error in dataset . Buying a brand new car from showroom must at least register 30km (car delivery, fuel filling , Road testing ).

Since last 60’s , car production stopped producing low engine capacities and the lowest they go since then is 660cc as we can see nowadays on the road . With this explanation , i have decided to scale my data within 660cc - 6600cc .

After modeling ,the best fit for linear regression with 0.795 of R squared value which mean 79.5% of the data fits the regression model .
As in the t-test columns , engine capacity and the year is very highly significant .
 
With the help of low p-values , we can reject the null hypothesis (no relationship between features)

Performed a validation with T-test, with a result of Mean Squared Error(MSE) : 0.11

Performed Cross validation test , resulted in 0.12 .

In conclusion . Engine capacity(cc) , age of the car and the engine type playing a big role in car prices .

