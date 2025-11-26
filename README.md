# Ex02 Django ORM Web Application
# Date:24/03/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![1dig](https://github.com/user-attachments/assets/47d51fd5-178b-4bc0-af2f-5f7b80f27a26)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM:
ADMINS.PY:
```
from django.contrib import admin
from.models import Loan,LoanAdmin
admin.site.register(Loan,loanAdmin)
```
MODELS.PY:
```
from django.db import models
from django.contrib import admin
class Loan(models.Model):
   lid=models.CharField(max_length=15,primary_key="lid")
   loantype=models.CharField(max_length=15)
   name=models.CharField(max_length=15)
   age=models.IntegerField()
   aadhar=models.IntegerField()
   documents=models.CharField(max_length=15)

class LoanAdmin(admin.ModelAdmin):
    list_display=('lid','loantype','name','age','aadhar','documents')
```
# OUTPUT
Include the screenshot of your admin page.
![web11](https://github.com/user-attachments/assets/b29dccb2-cd15-4977-8eb0-0c0ffc3d3b87)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
