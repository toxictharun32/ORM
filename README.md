# Ex02 Django ORM Web Application
## Date: 20/09/2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
admin.py
from django.contrib import admin
from . models import Car
# Register your models here.

admin.site.register(Car)

class CarAdmin(admin.ModelAdmin):
    list_display = ('id','brand','model','year','price','type')

models.py
from unittest.util import _MAX_LENGTH
from django.db import models
from django.forms import IntegerField

# Create your models here.
class Car(models.Model):
    id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=15)
    model = models.CharField(max_length=40)
    year = models.DateField()
    price = models.IntegerField()
    type = models.CharField(max_length=10)

```


<img width="1920" height="1200" alt="Screenshot (1)" src="https://github.com/user-attachments/assets/597d9754-e3b4-4a16-afb1-acf77e251265" />
<img width="1920" height="1200" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/db176c58-91f6-432e-864e-312e4f25aab2" />



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
