# Ex02 Django ORM Web Application
# Date:25.03.2024
# Name:Malligesh
# register number:212223230119
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2025-04-08 102616](https://github.com/user-attachments/assets/8eb61d8c-6d76-4c89-b846-190343f8a2f2)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
Admin.py :

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)


Models.py :

from django.db import models
from django.contrib import admin
class Employee (models.Model): 
   eid=models.CharField(max_length=20,help_text="Employee ID")
   name=models.CharField(max_length=100)
   salary=models.IntegerField()
   age=models.IntegerField()
   email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```
# OUTPUT

![alt text](screenshot.png)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
