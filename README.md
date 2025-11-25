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
from.models import Loan
class LoanAdmin(admin.ModelAdmin):
    pass
admin.site.register(Loan,LoanAdmin)

models.py

from django.db import models
from django.contrib import admin
 
class Loan(models.Model):
 Name=models.CharField(max_length=10)
 Accountno=models.IntegerField(primary_key="Refno")
 Address=models.CharField(max_length=30)
 Aadharno=models.IntegerField()
 Email=models.EmailField()

 class LoanAdmin(admin.ModelAdmin):
  list_display=('Name','Accountno','Address','Aadharno','Email')
```
# OUTPUT
<img width="1908" height="967" alt="deekshaorm" src="https://github.com/user-attachments/assets/ce1d16ec-98c7-4f33-bb7f-7f7b0a7ff907" />


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
