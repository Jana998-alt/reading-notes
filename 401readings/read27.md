#  Django Models

*Models* define the structure of stored data, including the field data types, their maximum size, default values, selection list options, allow for documentation, label text for forms, etc. The definition of the model is independent of the underlying database.

## Fields

Models are maped out through fields that it contains. each field represents a column of data that we want to store in one of our database tables.
examples of fields: 
- BinaryField
- BooleanField 
- CharField	
- DateField	
- DateTimeFeild	
- DecimalField	
- DurationField
- EmailField


## Meta

Metadata
You can declare model-level metadata for your Model by declaring class Meta.

One of the uses of metadata is to control the default ordering of records returned when you query the model type.

PS: do not forget to define a str method, it will make your testing life easier!
```
def __str__(self):
    return self.field_name
```

##  Django admin site

Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records
The admin application can also be useful for managing data in production, depending on the type of website

### Registering models
1- open admin.py

2- register model by admin.site.register(model_name)

3- to create a super admin/user type: ``` python manage.py createsuperuser``` in terminal

4- it will ask you to give a user name for the super user, an email, a password and to confirm the password
5- To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin)

you can display your wanted field by using list display attribute in a class that inherates from admin.modelAdmin:

```
class BookAdmin(admin.ModelAdmin):
    list_display = ('title', 'author', 'display_genre') 
```
