# capstone_project

Author : Fahmi Afri

# project overview

Finding the related features affecting the used car price .

### The features :

Engine Capacity(cc) 

Engine Type - Petrol , Diesel , Hybrid , LPG , CNG

Year (1990-2021)

Mileage (kms)

Transmission type - automatic , manual 


### The Data

This data required me to do Regression analysis ,i.e : how much is this used car ?

As a Data Science lifecycle , i performed :

### Data mining - collecting data suitable with the business problem.

Data resource :  https://www.kaggle.com/datasets/ebrahimhaquebhatti/75000-used-cars-dataset-with-specifications

![Screenshot 2022-11-07 155105](https://user-images.githubusercontent.com/112393492/200230906-c5b72b6e-ce2c-4870-b3b7-58db0b60e5a3.png)

![Screenshot 2022-11-07 155259](https://user-images.githubusercontent.com/112393492/200230957-4ae0d18b-6d38-4c77-a218-6fbbff48d4e3.png)

### Data cleaning - removing any inconsistencies in dataset i.e duplicate , missing values , outliers, standardization and normalization

![Screenshot 2022-11-07 161135](https://user-images.githubusercontent.com/112393492/200231439-48831aca-7ac5-451b-bba0-0fadfe1e5c83.png)

![Screenshot 2022-11-07 161241](https://user-images.githubusercontent.com/112393492/200231458-49aa51f2-480b-4c81-809a-324e2f5e91a6.png)

![Screenshot 2022-11-07 155332](https://user-images.githubusercontent.com/112393492/200231472-1b40ab69-73df-40e5-9944-6812c9ccefb2.png)

![Screenshot 2022-11-07 162949](https://user-images.githubusercontent.com/112393492/200233212-f43d1436-1025-4a62-87ab-deb814f531b6.png)


As a industry specialist, i have been working with cars for almost 6 years , i have reduced the range for Mileage(kms) and Years due to few reasons .

1990-2021 is still in acceptable range of year because of spare parts availability , workshop options , wear and tear of factory built , comfortability ,newer technology and more safety features .

Being a used car , having a 1km on the clock does not really indicate correctly and this may possibly error in dataset . Buying a brand new car from showroom must at least register 30km (car delivery, fuel filling , Road testing ).

Since last 60’s , car production stopped producing low engine capacities and the lowest they go since then is 660cc as we can see nowadays on the road . With this explanation , i have decided to scale my data within 660cc - 6600cc .

Dropping 3 missing values ,which is 0.004 of the data wont affect much so i decided to drop it and carry on.

### Data exploration - building graph for better understanding of the data .

### Feature engineer - manipulate features for better fit for our modeling .

![Screenshot 2022-11-07 155537](https://user-images.githubusercontent.com/112393492/200231602-bafe345d-e644-4c96-856e-b0b8058424cc.png)

![Screenshot 2022-11-07 155604](https://user-images.githubusercontent.com/112393492/200231614-c73ebe3f-f2a4-48bd-97e1-34ee51f79b1d.png)

Performing standardization on the baseline model .

![Screenshot 2022-11-07 155858](https://user-images.githubusercontent.com/112393492/200231787-c38bf747-9c4e-4c9a-8d56-0c3e6be095bf.png)

Performing normalization for 2nd model .

![Screenshot 2022-11-07 160002](https://user-images.githubusercontent.com/112393492/200231628-fe50b032-9a31-4582-b512-3033a9666499.png)

### Predictive model - performed Linear Regression to train , evaluate the performance and creating predictions .

# Baseline model 

![Screenshot 2022-11-07 155811](https://user-images.githubusercontent.com/112393492/200231719-9e9872d9-e74d-4b7d-af8c-5ea8c2f5bf0f.png)

after standardized , the R-squared value :

![Screenshot 2022-11-07 162024](https://user-images.githubusercontent.com/112393492/200232111-a247b4a1-2d44-4807-a078-06145473367d.png)

# Model 2

![Screenshot 2022-11-07 160021](https://user-images.githubusercontent.com/112393492/200232205-fbe5bba9-193f-46a0-972e-1e651cfd562b.png)

![Screenshot 2022-11-07 160139](https://user-images.githubusercontent.com/112393492/200232226-1f7f6801-2ad6-4b9e-8a81-17fb3d76d6cd.png)

## Conclusions

After modeling ,the best fit for linear regression with 0.795 of R squared value which mean 79.5% of the data fits the regression model .
As in the t-test columns , engine capacity and the year is very highly significant .
 
With the help of low p-values , we can reject the null hypothesis (no relationship between features)

Performed a validation with T-test, with a result of Mean Squared Error(MSE) : 0.11

Performed Cross validation test , resulted in 0.12 .

In conclusion . Engine capacity(cc) , age of the car and the engine type playing a big role in car prices .

