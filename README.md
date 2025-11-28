# Ex01 Django ORM Web Application
## Date: 
28-11-2025
## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
ADMIN.PY: 

from django.contrib import admin 
from . models import cars,CarAdmin 
admin.site.register(cars,CarAdmin) 

MODELS.PY:

from django.db import models 
from django.contrib import admin 
class cars(models.Model): 
    brand = models.CharField(max_length=100) 
    model = models.CharField(max_length=100) 
    year = models.IntegerField() 
    price = models.DecimalField(max_digits=10, decimal_places=2) 
class CarAdmin(admin.ModelAdmin): 
    list_display=['brand','model','year','price'] 

```
## OUTPUT

<img width="1919" height="1079" alt="Screenshot 2025-11-28 133920" src="https://github.com/user-attachments/assets/958a1bfc-bbaf-4b97-a8cf-cce7970e4137" />


## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
