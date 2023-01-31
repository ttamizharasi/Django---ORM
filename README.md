# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


![er](https://user-images.githubusercontent.com/119657317/215686891-52b639a2-b2c0-406e-a96a-12e72de2f2ba.png)








## DESIGN STEPS

### STEP 1:

clone the problem from github

### STEP 2:

create a new app

### STEP 3:

Enter the code for admin.py and models.py

### Step 4:

execute Django admin and create 10 employees

## PROGRAM
 
 ```
 Model.py

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

Admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

```

## OUTPUT

![out](https://user-images.githubusercontent.com/119657317/215686790-6c627d12-088a-4573-888b-cb96461a6e5b.png)


## RESULT

Program executed successfully
