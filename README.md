# Ex01 Django ORM Web Application
## Date: 

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

admin.py 
```
from django.contrib import admin
from .models import Car_Inventory, Car_InventoryAdmin
admin.site.register(Car_Inventory, Car_InventoryAdmin)
```
models.py
```
from django.db import models
from django.contrib import admin
class  Car_Inventory(models.Model):
    Plate_No = models.CharField(max_length=20, primary_key=True)
    Car_Manufacturer = models.CharField(max_length=15)
    Car_Model = models.CharField(max_length=100)
    Car_Color = models.CharField(max_length=20)
    Mileage = models.IntegerField( )

class Car_InventoryAdmin(admin.ModelAdmin):
    	list_display = ('Plate_No', 'Car_Manufacturer','Car_Model', 'Car_Color', 'Mileage')
```
## OUTPUT

<img width="1887" height="920" alt="image" src="https://github.com/user-attachments/assets/9ee9cff0-d94e-407d-805e-a7e9845d2542" />


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
