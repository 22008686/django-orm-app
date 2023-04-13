# Django ORM Web Application

## AIM:

To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:

Include your ER diagram here

## DESIGN STEPS:

## STEP 1:

Create a Django app Go to the app directory In models.py create two classes And save the models.py

## STEP 2:

Go to admins.py And put the two class in admins.py from the models.py And save the file

## STEP 3:

Start the Django server Then move to admin page

## PROGRAM:

MODELS.PY:
```
from django.db import models
from django.contrib import admin


# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```
    
ADMIN.PY:
```
from django.contrib import admin
from .models import Student,StudentAdmin


# Register your models here.
admin.site.register(Student,StudentAdmin)

```
## OUTPUT:

![orm](https://user-images.githubusercontent.com/118916413/231650246-682173ac-1c6a-41da-8e5b-056568202413.png)



## RESULT:

Thus the program have been executed successfully.
