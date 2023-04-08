# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Fork and clone the repositary in to your IDE.

### STEP 2:
Create a django project and an app and a superuser account and run the server.

### STEP 3:
Modify changes in settings and write ur code on models and admin and run the server.

###STEP 4:
Login in to admin using your superuser account and populate the records.



## PROGRAM
```
from django.db import models
from django.contrib import admin
# Create your models here.
class Student(models.Model):
    studentname = models.CharField(max_length=100,primary_key= True)
    refno = models.CharField(max_length=100)
    lastname= models.CharField(max_length=80)
    emailid = models.EmailField()
    age=models.CharField(max_length=10)
    mobile=models.CharField(max_length=10)

    
class StudentAdmin(admin.ModelAdmin):
    list_display = ('studentname','refno','lastname','emailid','age','mobile')
````
## OUTPUT

![4a0fcd8c-7c20-45a3-a2b2-6b50450efa7a](https://user-images.githubusercontent.com/120550359/230556586-e4f77efe-a04f-4ee9-b968-d05e85fe8f3f.jpg)

![632d6262-169b-40b3-a880-97a40c2fbb33](https://user-images.githubusercontent.com/120550359/230556598-bf1e3421-2423-4a59-b800-8df31da06108.jpg)





## RESULT
Thus we developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
