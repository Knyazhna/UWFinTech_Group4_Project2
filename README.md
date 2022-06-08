# UWFinTech_Group4_Project2

## Project Description

We will use machine learning for predicting the premium of health insurance and to identify factors that lead to higher healthcare costs.


## Outline

1. Exploratory Analysis and Visualization
	1. Age
	2. BMI
	3. Charges
2. Visualization of the distribution of medical charges in connection with other factors like "sex" and "region"
	1. Sex
	2. Region
	3. Smoker
3. Visualization of the distributions of the "sex", "region" and "children" columns
	1. Children
	2. Age & charges
	3. BMI & charges
4. Visualizing how the "charges" column is related to other columns ("children", "sex", "region" and "smoker").
	1. Visualizations
	2. Correlation
	3. Loss/cost
	4. Linear regression for NonSmokers (skikit-learn)
5. Model creation for Smokers in the dataset
	1. Workflow of Machine Learning Problem:
		1.  Explore the data and find correlations between inputs and targets
		2.  Pick the right model, loss functions and optimizer for the problem at hand
		3.  Scale numeric variables and one-hot encode categorical data
		4.  Set aside a test set (using a fraction of the training set)
		5.  Train the model
		6.  Make predictions on the test set and compute the loss
​
### Ideas for work division:
* Each section, as seen above, can be broken into individual modules - each contained within their own notebook
	* Then, within our main notebook we can import and call each module
​
* This allows us to split up the project without depending on the previous section to be compete
	* However, each section will need to create it's own test data so that we can test and run the code independently
​
### Other things to consider: 
While I like the layout of this project, I feel it best if we use data other than that contained in the Kaggle project
​
What we will need:
*  Features 
	* e.g. BMI, age, smoker (y/n))
* At least 10x features in row data
	* Age, BMI, smoker, chagers = 4 
		* 4 x 100 = 400 row data
​
​
## Notes on Data
* BMI every other year


### Variables
| Variable | Description | 
|-------------| ----------------| 
| PID | Person Number | 
| AGE18X | Age as of 12/31/18 (Edited/Imputed) |
| ENDRFY18 | 2018 Reference Period End Date: Year |
| TTLP18X | Person’s Total Income | 
| TOTEXP18 | Total Expenditures | 
| REGION18 | Census Region as of 12/31/18| 
| ADBMI42 | SAQ: Adult Body Mass Index (>17)-RD 4/2| 
| ADTBAC42 | Asked if smoke or use tobacco by health professional, last 12 months | 
[MEPS Docs](https://meps.ahrq.gov/data_stats/download_data/pufs/h209/h209doc.shtml#Health2510)
[MEPS Files](https://meps.ahrq.gov/mepsweb/data_stats/download_data_files_results.jsp?cboDataYear=All&cboDataTypeY=101%2CConsolidated+Data&buttonYearandDataType=Search) 
[MEPS Conversion](https://meps.ahrq.gov/about_meps/Price_Index.shtml)



## Contributors

* Maureen Kaaria

Email: maureenkaaria@gmail.com
* Khaing Thwe

Email: khaingzt88@gmail.com
* Olga Koryachek

Email: olgakoryachek@live.com

[LinkedIn](https://www.linkedin.com/in/olga-koryachek-a74b1877/?msgOverlay=true "LinkedIn")
* Arthur Lovett

Email: arthur@arthurlovett.com


---

## License

Licensed under the [MIT License](https://choosealicense.com/licenses/mit/)


