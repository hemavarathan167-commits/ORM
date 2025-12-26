# Ex01 Django ORM Web Application
## Date: 24/12/25

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM
~~~
models.py

from django.db import models 
from django.contrib import admin
class Cars_DB (models.Model):
     Car_name=models.CharField(max_length=20)
     reg_no=models.IntegerField (primary_key=True)
     fuel_type=models.CharField(max_length=20)
     engine_model=models.CharField(max_length=20)
     insurance_no=models.IntegerField()
class Cars_DBAdmin(admin.ModelAdmin):
     list_display=["Car_name","reg_no","fuel_type","engine_model","insurance_no"]

admin.py

from django.contrib import admin
from .models import Cars_DB,Cars_DBAdmin
admin.site.register(Cars_DB,Cars_DBAdmin)
~~~

## OUTPUT
<img width="1014" height="429" alt="image" src="https://github.com/user-attachments/assets/1dba22a8-0e2d-4719-98b7-7bf3ace1648d" />



## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
