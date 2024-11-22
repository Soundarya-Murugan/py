---
title: Modifying-Nested-Values
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

# Define a class for Employee that supports attributes
class Employee:
    def __init__(self, name, role, contact):
        self.name = name
        self.role = role
        self.contact = contact

# Define a class for Company that holds a list of employees
class Company:
    def __init__(self, employees):
        self.employees = employees

# Creating instances of Employee
company = Company([
    Employee('John', 'Manager', {'email': 'john@example.com'}),
    Employee('Jane', 'Developer', {'email': 'jane@example.com'})
])

# Using magicattr to set the 'role' attribute of the first employee
magicattr.set(company, 'employees[0].role', 'Senior Manager')

# Directly modifying the nested 'email' value in the second employee's dictionary
company.employees[1].contact['email'] = 'jane.new@example.com'

# Using magicattr to get the updated role of the first employee
role = magicattr.get(company, 'employees[0].role')

# Output the modified values
print(role)  # Expected Output: 'Senior Manager'
print(company.employees[1].contact['email'])  # Expected Output: 'jane.new@example.com'


```

    Senior Manager
    jane.new@example.com



```python

```


---
**Score: 0**