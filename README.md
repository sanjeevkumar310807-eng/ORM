# Ex02 Django ORM Web Application
# Date:
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
'''
admin.py

from django.contrib import admin
from.models import cars,carsAdmin

admin.site.register(cars,carsAdmin)

models.py

from django.db import models
from django.contrib import admin

class cars(models.Model):
    car_model=models.CharField(max_length=20)
    car_name=models.CharField(max_length=20)
    manufactoring_date = models.DateField()
    colour=models.CharField(max_length=20)
    price=models.IntegerField()

class carsAdmin(admin.ModelAdmin):
    list_display=['car_model','car_name','manufactoring_date','colour','price']
    

# OUTPUT
<img width="830" height="531" alt="Screenshot 2025-11-26 092058" src="https://github.com/user-attachments/assets/2647d6ed-551a-4a33-bb8d-e911546132d5" />

<img width="1859" height="903" alt="Screenshot 2025-11-26 092600" src="https://github.com/user-attachments/assets/40eb3103-4ea2-477c-a0d2-d49ed073b6e7" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
