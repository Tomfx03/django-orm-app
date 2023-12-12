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
#From admin.py
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)


#From models.py
from django.db import models
from django.contrib import admin

# Create your models here.

class Student (models.Model):
    referenceno=models.CharField(primary_key=True,max_length=20,help_text="referenceno")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    mobileno=models.IntegerField()
class StudentAdmin (admin.ModelAdmin):
    list_display=('referenceno','name','age','email','mobileno')


## OUTPUT

![Screenshot from 2023-12-12 16-05-41](https://github.com/Tomfx03/django-orm-app/assets/101335832/3d3e96f6-b0db-4463-9253-cc188f3fbec9)



## RESULT
