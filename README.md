# Ex02 Django ORM Web Application
## Date: 18/10/2023
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
```
models.py
from django.db import models
from django.contrib import admin
class football_players (models.Model):
    playersid=models.CharField(max_length=20)
    players_name=models.CharField(max_length=100)
    players_position=models.CharField(max_length=100)
    players_age=models.IntegerField()
    players_jersey_no=models.IntegerField()
    players_email=models.EmailField()
class football_playersAdmin (admin.ModelAdmin):
    list_display=('playersid','players_name','players_position','players_age','players_jersey_no','players_email')
admin.py
from django.contrib import admin
from .models import football_players,football_playersAdmin
admin.site.register(football_players,football_playersAdmin)

```


## OUTPUT
![Screenshot 2023-10-18 090657](https://github.com/Gokkul-M/ORM/assets/144870543/a27f7c29-f03a-41c8-b438-2fce89185803)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
