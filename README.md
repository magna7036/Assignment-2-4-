salary = float(input("Enter Salary: "))

numDependents = int(input("Enter Number of Dependents: "))

 

stateTax = salary * (6.5/100)

print("State Tax: $" + str(stateTax))

 

federalTax = salary * (28/100)

print("Federal Tax: $" + str(federalTax))

 

dependentDeduction = (salary * (2.5/100)) * numDependents

print("Dependents: $" + str(dependentDeduction))

 

totalWithholding = (stateTax + federalTax) + dependentDeduction

takeHomePay = salary - totalWithholding

print("Salary: $" + str(salary))

print("Take Home Pay: $" + str(takeHomePay))
