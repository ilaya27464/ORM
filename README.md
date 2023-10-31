# Ex02 Django ORM Web Application
## Date: 31-10-2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

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

## admin.py:
```
from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)
```

## models.py:
```
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')
```

## OUTPUT
![Screenshot (405)](https://github.com/ashmistalin/ORM/assets/103128410/75ebb2fb-4f9b-4c8e-b961-973368382f85)
![Screenshot (409)](https://github.com/ashmistalin/ORM/assets/103128410/ebece0e7-7105-4a83-9b1d-0fd04ceed27c)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
