Task: Analyse under which condition an employee absenteeism more than 3 hours

data _preprocessing:
	- data wrangling
	- dummy variables (feature engineering)
prediction:
	- model (regression)
	- prediction (absenteeism more than 3 hours = 1, absenteeism less than 3 hours = 0 )

   
result of analysis:

Transportation Expense and Children (we suspect that someone how has lower transportation expense lives closer to the workplace) :
	- Employees with no children live closer to the workplace then someone with children
	- There is a slight correlation between more transport expense (and children) and the probability to be absent for more than 3 hours
	--> more children and higher transport expense = higher probability to be absent for more than 3 hours
	
Reasons vs Probability:
	- Diseases: very high probability that employee will be absent for more than 3 hours
	- Light reason : very low probability that employee will be absent for more then 3 hours (medical appointment, physiotherapist, ...)
	- Poisoning: not enough data
	- Pregnancy: no known case in this dataset 
	
Age vs Probability:
	- employee age <= 40 : lower probability to be absent for more than 3 hours
	- employee age > 40 : higher probability to be absent for more then 3 hours
	 
screenshots:

dashboard

data _preprocessing

prediction