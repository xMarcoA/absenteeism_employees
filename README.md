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
![Bildschirmfoto 2021-05-23 um 19 30 01](https://user-images.githubusercontent.com/76050281/119494059-2d096580-bd61-11eb-856d-0ca4f3f59986.png)

data _preprocessing
![Bildschirmfoto 2021-05-25 um 12 49 30](https://user-images.githubusercontent.com/76050281/119494096-3561a080-bd61-11eb-900e-ddd65c5cab77.png)

prediction
![Bildschirmfoto 2021-05-25 um 13 03 26](https://user-images.githubusercontent.com/76050281/119494116-3abeeb00-bd61-11eb-88a3-075a48914d71.png)
