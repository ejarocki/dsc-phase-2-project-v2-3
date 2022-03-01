Overview and Business Understanding
My stakeholder is Lynn Crane Real Estate. She wanted to identify trends within home sales in King County, Washington. There are many considerations when buying and selling a home that she must take into account. She wanted to know which attributes of a home are the most desirable (ie. yield the highest selling price). I used data from the King County House Sales dataset to create several models to determine which features affected price the most. 

Modeling and Regression Results
5 models were created. The first model used all numerical features in the data set to perform multiple linear regression. The R-squared value was quite high (.627) as well as the dimension.Some standard error values were quite high as well as a number of negative coefficients. This model was not optimized. Model 2 focused on the bedrooms, living space, and floors of the homes in the dataset. Although its R-squared was good (.507), the p-value of floors failed at an alpha level of .05. There was also a negative correlation between bedrooms and price. Model 3 took into account the condition value of the homes in the dataset. The conditions ranged from 0-Poor to 5-Very good. There was a small R-value of 0.007, which means that the condition of these homes accounted for less than 1% of price variation. Even though this value was small, I worked it into my fourth model to see if it could improve Model 2. Model 4 looked at the relationship between Price, Condition, and Living Space. The R-squared was slightly improved from Living Space v. Price alone, but several variables failed by having a p-value of greater than and alpha of .05. Therefore, this model was not acceptable. I found that the best model was just Living Space vs. Price. This model takes into account 49.3% of the variation in Price just from living space alone, with a coefficient of 280.8630. 

Conclusion
Find homes with lots of living space that are undervalued, even if their condition is not top quality
Prioritize living space over number of floors in a prospective hosue
If a house can be rennovated for resale, advise the homeowner to expand the living space.

Directory

> Project2-Elijah.Jarocki.ipynb: Jupyter Notebook with code used to perform analysis
> 
> Project2-Elijah.Jarocki.pdf: PDF version of slideshow presentation for the project
> 
> /Data: Folder with kc_house_data.csv, the working data for this project & column_names.md a further explanation of the meaning of the column features for the dataset. 
> 
> LICENSE.md: License from Flatiron School for use of this data
