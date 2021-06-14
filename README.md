
Hello,

Welcome to the README file for my Zillow Project.

Here, you will find expanded information on this project including goals, how I will be working through the pipeline and a data dictionary to help offer more insight to the variables that are being used.

## Goal
My goal is to identify and key driver(s) of the home value in the Zillow database and develop a regression model to accurately predict the key driver(s) of the value of the home prices.

______________________



## Planning process

Below you will see the TRELLO pipleline I used which can also be found in this link: [TrelloBoard]https://trello.com/b/wSKsBvKG/zillow-project-board





###  Data Dictionary
- The dictionary below is a reference for the variables used within the dataset



|   Feature      |  Data Type   | Description    |
| :------------- | :----------: | -----------: |
|  parcelid | int64   | Unique parcel identifier    |
| bed    | float64 | count of bedrooms |
| bath   | float64 | count of bathrooms |
|  sqrft  | float64   | Total livable square footage    |
| county  # 6037| float64 | Los Angeles |
| county # 6059 | float64   | Orange    |
| county # 6111  | float64| Ventura |
| year_built    | float64 | year home was built|
| taxval  | float64 | total value of home established by taxing authority|
| taxamt    | float64 | The most recent year property taxes were assessed|
| propertylandusetypeid # 260  | float64 | property type - Residential General |
| propertylandusetypeid # 261  | float64 | property type - Single Family Residential |
| propertylandusetypeid  # 263 | float64 | property type - Mobile Home |
| propertylandusetypeid # 264  | float64 | property type - Townhouse |
| tax_rate    | float64 | This is property tax / tax_assessed_value|



-------------------
 
 
#### Initial Hypotheses

> - **Hypothesis 1 -** I rejected the Null Hypothesis; there is a difference.
> - alpha = .05
> - $H_o$: There is no association between number of bedrooms and tax value.  
> - $H_a$: There is an association between number of bedrooms and tax value. 

> - **Hypothesis 2 -** I rejected the Null Hypothesis; there is a difference.
> - alpha = .05
> - $H_o$: There is no association between square foot of home and tax value.
> - $H_a$: There is an association between square foot of home and tax value.


<hr style="border-top: 10px groove blueviolet; margin-top: 1px; margin-bottom: 1px"></hr>

### Executive Summary - Conclusions & Next Steps
<hr style="border-top: 10px groove blueviolet; margin-top: 1px; margin-bottom: 1px"></hr>

> - Recommendations & next steps:

I would recommend 







<hr style="border-top: 10px groove blueviolet; margin-top: 1px; margin-bottom: 1px"></hr>

### Pipeline Stages Breakdown

<hr style="border-top: 10px groove blueviolet; margin-top: 1px; margin-bottom: 1px"></hr>

##### **Plan ->** Acquire -> Prepare -> Explore -> Model -> Deliver
- [x] Create README.md with data dictionary, project and business goals, come up with initial hypotheses.
- [x] Acquire data from the SQL Database and create a function to automate this process. Save the function in an acquire.py file to import into the Final Report Notebook.
- [x] Clean and prepare data for the first iteration through the pipeline, MVP preparation. Create a function to automate the process, store the function in a prepare.py module, and prepare data in Final Report Notebook by importing and using the funtion.
- [x]  Clearly define two hypotheses, set an alpha, run the statistical tests needed, reject or fail to reject the Null Hypothesis, and document findings and takeaways.
- [x] Establish a baseline accuracy and document well.
- [x] Train three different regression models.
- [x] Evaluate models on train and validate datasets.
- [x] Choose the model with that performs the best and evaluate that single model on the test dataset.
- [x] Create csv file with the customer id, the probability of churn, and the model's predictions.
- [x] Document conclusions, takeaways, and next steps in the Final Report Notebook.

___

#### Acquire
> - Store functions that are needed to acquire data  that will be used for the Zillow Regression Project
> - The final function will return a pandas DataFrame


#### Prepare
> - Store functions needed to prepare the Zillow data
> - Import the prepare functions created by using .prepare.py


#### Explore
> - Answer key questions, my hypotheseses, and figure out the features that can be used in a regression model to best predict driver for churn


#### Model
> - Establish a baseline accuracy to determine if having a model is better than no model and train for at least 3 different models

#### Deliver
> - Deliver my findings in the presention.



<hr style="border-top: 10px groove blueviolet; margin-top: 1px; margin-bottom: 1px"></hr>

### Reproduce My Project

<hr style="border-top: 10px groove blueviolet; margin-top: 1px; margin-bottom: 1px"></hr>

You will need your own env file with database credentials along with all the necessary files listed below to run my final project notebook. 
- [X] Read this README.md
- [ ] Download the aquire.py, prepare.py, and final_report.ipynb files into your working directory
- [ ] Add your own env file to your directory. (user, password, host)
- [ ] Run the final_report.ipynb notebook