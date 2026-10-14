# Bill Splitter

A Python program designed to calculate and split a restaurant bill evenly among a group of friends, including tax or tip calculations. This project was completed as part of the freeCodeCamp Python certification.

## Features

* *Running Totals*: Calculates the combined cost of appetizers, main courses, desserts, and drinks using augmented assignment operators.
* *Tip Calculation*: Automatically computes a 25% tip based on the running total.
* *Per-Person Breakdown*: Divides the final total among a specified number of friends and rounds the result to two decimal places for currency formatting.

## Code Overview

Here is the Python code used for this project:

```python
running_total = 0 #Storing an integer in variable 

num_of_friends = 4 # Storing the amount of people as integer in variable 

appetizers = 37.89 #Storing the price of items as a float in variable 
main_courses = 57.34 #Storing the price of items as a float in variable 
desserts = 39.39 #Storing the price of items as a float in variable 
drinks = 64.21 #Storing the price of items as a float in variable 

running_total += appetizers + main_courses + desserts + drinks # Storing the result of augmented assignment  of all meal items combined in variable 
print('Total bill so far:', running_total) #Output: Total of bill so far 

tip = running_total * 0.25 #Storing the result of multiplication add tip to running total in variable 
print('Tip amount:', tip) #Output: Total tip amount  

running_total += tip # Storing the result of augmented assignment in variable 
print('Total with tip:', running_total) #output: Total bill including the tip amount 

final_bill = running_total / num_of_friends # Storing the result of dividing the running total by number of people in variable 
print('Bill per person:', final_bill) #Output: Bill amount per person 

each_pays = round(final_bill, 2) #Storing the result of rounding the final bill per person by 2 decimal places in variable 
print(f'Each person pays: {each_pays}')# output:The total per person rounded to 2 decimal places 

## 💻 How to run
1. Ensure you have python installed on your system
2. Clone this repository or download the Bill_Splitter.py file 
3 Run the script using your terminal or command prompt
```bash
python Bill_Splitter.py
