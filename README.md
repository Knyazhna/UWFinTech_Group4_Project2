# UWFinTech_Group4_Project2

## Project Description

We will use machine learning for predicting the cost of healthcare given a list of personal characteristics. Our aim is to understand with greater clarity the correlation of cost with each of these features and in doing so, evaluate cost-effectiveness of personal health. 


## Data

### Overview
Our data is sourced from the Medical Expenditure Panel Survey (MEPS), a set of large-scale surveys of families and individuals, the medical providers, and employers accross the United States. More specifically, this project uses data from the Household Compoent (HC) that collects data from samples of families and individuals in selected communities to create a nationally representative sample population.

[MEPS File List](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_results.jsp?cboDataYear=All&cboDataTypeY=101%2CConsolidated+Data&buttonYearandDataType=Search) 
[MEPS 2018 Documentation](https://meps.ahrq.gov/data_stats/download_data/pufs/h209/h209doc.shtml#Health2510)

### Variables used in analysis: 
| Variable Name | Description |
--------------| ----------------|
| `ID` | Panel # + Encrypted DU Identifier |
| `Family_Size` | Number of persons associated with a single family unit after students are linked to their associated parent |
| `Region` | Geopgraphic Census Region | 
| `Age` | Age of respondent as of 12/31 |
| `Sex` | Sex (1=M/2=F) | 
| `Race` | Race | 
| `Education_Level` | Total Years of Education |
| `Highest_Degree` | Highest degree earned | 
| `BMI` | Body Mass Index | 
| `Tobacco_Use` | Frequency of Tobacco Use in last 12 months | 
| `Total_Personal_Income` | Person’s Total Income | 
| `Uninsured_2018` | Uninsured all of 2018 | 
| `Total_Expenditure` | Total expenditure (sum of all sources) on health services | 
| `Exp_Pocket` | Out of Pocket Expenditure |
| `Exp_Medicare` | Medicare Expenditure | 
| `Total_Medicaid` | Medicaid Expenditure | 
| `Exp_VA` | Veteran’s Administration/CHAMPVA Expenditure |
| `Total_Priv_Tri` | Total Private and TRICARE Expenditures | 
| `Total_Other` | Other Federal, Other State and Local, Other Private, Other Public, and Other Unclassified Sources | 

### Variable Encoding Key
Region:
| Value | Label | States |
| ----- | ----- | ------ |
| 1 | Northeast | Connecticut, Maine, Massachusetts, New Hampshire, New Jersey, New York, Pennsylvania, Rhode Island, and Vermont |
| 2 | Midwest | Indiana, Illinois, Iowa, Kansas, Michigan, Minnesota, Missouri, Nebraska, North Dakota, Ohio, South Dakota, and Wisconsin |
| 3 | South | Alabama, Arkansas, Delaware, District of Columbia, Florida, Georgia, Kentucky, Louisiana, Maryland, Mississippi, North Carolina, Oklahoma, South Carolina, Tennessee, Texas, Virginia, and West Virginia |
| 4 | West | Alaska, Arizona, California, Colorado, Hawaii, Idaho, Montana, Nevada, New Mexico, Oregon, Utah, Washington, and Wyoming | 

Race:
| Value | Label | 
| ----- | ----- |
| 1 | White – No other race reported |
| 2 | Black – No other race reported |
| 3 | American Indian/Alaska Native – No other race reported |
| 4 | Asian Indian – No other race reported |
| 5 | Chinese – No other race reported |
| 6 | Filipino – No other race reported |
| 10 | Oth Asian/Natv Hawaiian/Pacfc Isl- No Other race reported |
| 12 | Multiple races reported | 


## Analysis

1. Exploratory Analysis and Visualization
	1. Age
	2. BMI
	3. Expenditure
2. Visualization of the distribution of medical charges in connection with other factors like "sex" and "region"
	1. Sex
	2. Region
	3. Tobacco-use
3. Visualization of the distributions of the "sex", "region" and "children" columns
	1. Family size
	2. Age & Expenditure
	3. BMI & Expenditure
4. Visualizing how the "Expenditure" column is related to other columns ("children", "sex", "region" and "Tobacco-use").
	1. Visualizations
	2. Correlation
	3. Loss/cost
	4. Linear regression for NonSmokers (scikit-learn)
5. Create three different Machine Learning model:
	1. Workflow of Machine Learning :
		1.  Explore the data and train and test on three Regression Models (Linear, Ridge, Lasso)
		2.  Fit into the model and test the R-Squared score
		3.  Using Mean Squared Error (MSE) metric to evaluate predictions accuracy
		4.  Evaluate cross-valatdation
		5.  Make predictions on the test
		6.  Train the model, compared three models and pick the most accurate Regression model
		7.  Build an automated RobotAdvisor to estimate the annual Healthcare expenditure for new/existing customers (AWS Lex).


## Contributors

* Maureen Kaaria
    * Email: maureenkaaria@gmail.com
 
* Khaing Thwe
    * Email: khaingzt88@gmail.com

* Olga Koryachek
    * Email: olgakoryachek@live.com
    * [LinkedIn](https://www.linkedin.com/in/olga-koryachek-a74b1877/?msgOverlay=true "LinkedIn")

* Arthur Lovett
    * Email: repo@arthurlovett.com


## License

Licensed under the [MIT License](https://choosealicense.com/licenses/mit/)


