# Python Cheat Sheet

## GIT HUB

0. git clone 
1. git add .
2. git commit -m "message stating what it is that has been changed"
3. git push (origin main)


## Conditionals 
for x in list_name:
    if x > 0:
        print("this return is positive and is" + x)
    elif x <= 0:
        print("this return is negative and is " + x)
        
## Loops

for number in num_list:
    if number > 50:
        print(number)

 * for initiates loop, 'number' is the name given to variable
 * 'in' specified which list the variables exist      

print("Index of first occurrence of the number 11:")
index = 0
for number in num_list:
    if number == 11:
        print(index)
    index += 1


## Iterating Lists 

* iterating means working through a list and applying calculations or printing sums. Essentially, working through a list and using its information to generate summary statistics.

once passed through a dataframe, iterating with pandas is very easy. 

for example

print("FINANCIAL ANALYSIS IS BELOW")
print("----------------------------")
print("TOTAL MONTHS ARE EQUAL TO:")
print(number_of_rows)
print("----------------------------")
print("TOTAL OF PROFIT AND LOSS IS EQUAL TO: ")
print(df["Profit/Losses"].sum())
print("----------------------------")
print("AVERAGE CHANGE WAS EQUAL TO: ")
print(df["Profit/Losses"].mean())
print("----------------------------")
print("GREATEST INCREASE WAS: ")
print(df[df['Profit/Losses'] == df['Profit/Losses'].max()])
print("----------------------------")
print("GREATEST DECREASE WAS ")
print(df[df['Profit/Losses'] == df['Profit/Losses'].min()])


## Functions 
def calculate_compound_growth_rate(beginning_balance, ending_balance, years):
    growth_rate = (ending_balance / beginning_balance)**(1/years) - 1
    return growth_rate

# Inputs
welcome_name = input(Hello, welcome to the website, what do I call you?)
print(f"Hello {welcome_name}")

don't forget to format!!!

inputs will automatically be recognised as strings. Must specify if it is an integer. 

sd = int(input("What is the standard deviation?"))

variance = sd**2

print(variance)

## Time Value of Money
A dollar today is worth more than a dollar tomorrow. 

fv = (CV * i/n)** t * n

pv = (FV / i/n)** t * n

essentially moving money through time. Must accomodate for compounding. 

i could equal the cost of equity capital, the market return alternative or any other percentage based returns. 

## CSV Reader

Essential for all calculations involving csv files.
csv == comma-separated values

from pathlib import Path
csv_path = (../Resources/filename.csv)

data = pd.csv_read(csv_path)

dataframe = pd.DataFrame(data)





## Cleaning Data


