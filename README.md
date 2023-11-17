# Ex02 Django ORM Web Application
## Date: 07.10.23

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
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)

Models.py

from django.db import models
from django.contrib import admin
class footballplayer (models.Model):
    numofmatch=models.IntegerField()
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    height=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('numofmatch','name','salary','age','height')
```

## OUTPUT

![Screenshot (57)](https://github.com/surothaaman/ORM/assets/133313653/aeb5813a-4506-46e3-bb2b-132a4e3da875)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
