# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
```
MODELS.PY:

from django.db import models
from django.contrib import admin
# Create your models here.
class Employee (models.Model):
    emp_id=models.CharField(primary_key=True,max_length=4,help_text='Employee ID')
    ename=models.CharField(max_length=50)
    post=models.CharField(max_length=20)
    salary=models.IntegerField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','salary')
    
    
ADMIN.PY:


from django.contrib import admin
from .models import Employee,EmployeeAdmin
# Register your models here.

admin.site.register(Employee,EmployeeAdmin)
```
## OUTPUT

![django](https://user-images.githubusercontent.com/118916413/230156828-7d0aebf3-ac52-4a87-8f7c-9a5d3de5f9ca.png)

## RESULT

Thus the program have been executed successfully.
