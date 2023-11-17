# Ex02 Django ORM Web Application
## Date: 10.10.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
Admin.py

from django.contrib import admin
from .models import footballplayers,playersAdmin
admin.site.register(footballplayers,playersAdmin)

Models.py

from django.db import models
from django.contrib import admin
class footballplayers (models.Model):
    name=models.CharField(max_length=100)
    address=models.CharField(max_length=100,default=00000)
    age=models.IntegerField()
    record=models.IntegerField()
    city=models.CharField(max_length=100,default=0000)

class playersAdmin(admin.ModelAdmin):
    list_display=('name','address','age','record','city')
```

## OUTPUT

![Alt text](<Screenshot 2023-10-31 093509.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
