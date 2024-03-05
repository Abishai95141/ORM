# Ex02 Django ORM Web Application
## Date: 02-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

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
Execute Django admin and create details for 10 books

## PROGRAM

```
models.py
from django.db import models
from django.contrib import admin 
class bookdb(models.Model):
    Bookid=models.IntegerField(primary_key=True)
    Bookname=models.CharField(max_length=20)
    Bookauthor=models.CharField(max_length=50)
    Bookprice=models.IntegerField()
    Bookgenre=models.CharField(max_length=20)
class BookAdmin(admin.ModelAdmin):
    list_display=("Bookid","Bookname","Bookauthor","Bookprice","Bookgenre")

admin.py
from django.contrib import admin
from .models import bookdb,BookAdmin
admin.site.register(bookdb,BookAdmin)
```

## OUTPUT

![image](https://github.com/Abishai95141/ORM/assets/139335314/3a39a794-bc8b-4299-98ed-81626fb057ce)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
