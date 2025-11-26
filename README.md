# Ex02 Django ORM Web Application
# Date:25/11/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
admin.py

from django.contrib import admin 
from .models import Car_Inventory, Car_InventoryAdmin 
admin.site.register(Car_Inventory, Car_InventoryAdmin)

models.py

from django.db import models 
from django.contrib import admin 

class  Car_Inventory(models.Model): 
    Car_Model = models.CharField()
    Engine_Type = models.CharField() 
    Car_Type = models.CharField() 
    Date = models.DateField()
    Car_Mileage = models.IntegerField()  
    

class Car_InventoryAdmin(admin.ModelAdmin): 
    list_display = ('Car_Model', 'Engine_Type', 'Car_Type', 'Date', 'Car_Mileage')
```
# OUTPUT

<img width="1916" height="976" alt="deekshaorm" src="https://github.com/user-attachments/assets/d9109f97-4072-49da-81af-043b94717c53" />


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
