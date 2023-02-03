# Calculating Coffee Servings from String Data

Methods used to calculate Total Servings: 

Considering the complexity of the 'Title' column data and that it is not standardized (different terms used to descibe servings and boxes), I decided to proceed with using Python to parse through unique 'Title' values using regular expressions to retrieve keywords associated with servings and its numeric values.  

I've organized keywords associated with servings into three groups: 
1. Count - number of servings per box
2. Box - number of boxes
3. Total - total number of servings per SKU

Number of servings associated with 'total' keyword group provides total number of servings per SKU. However it is barely used in the 'Title' column so we get servings count and multiply it by the number of boxes to get total. 

Total (if not explicitly stated) = count * boxes

If there is no informaiton on boxes or counts we assume the value is 1. 



DISCLOSURE:  The formulas and code need more fine-tuning to accomodate for all boundary casees. 
