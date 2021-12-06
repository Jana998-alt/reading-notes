# Django Forms

An HTML Form is a group of one or more fields, which allows us to collect information from the users. Forms are somewhat secure becasue they allow to send the data using POST requests. 

Django forms are a simpler ways to use forms. they provide ready-to-use templates and data validation for the form fields. Django forms are very similar to Django Models, and the code is also very similar. which makes sense because they kind of perform the same task.

Django forms handels the data through this algorithm: 

![django forms algorithms](form_handling.png)


basically including: Displaying the default form on first time it is requested by the user, validate the data, performing required actions if the data is valid and redirecting the user to another page.

### declaring a form:

inside the forms.py file in your app, type: 

``` 
from django import forms

class FormClassName(forms.Form):
    date_created = forms.DateField(help_text="Today's date")
```

### Validation 

this is how to validate a field:

```
from django.core.exceptions import ValidationError

class FormClassName(forms.Form):
    date_created = forms.DateField(help_text="Today's date")

    def clean_date_created(self):
        data = self.cleaned_data['date_created']

        if data != datetime.date.today():
            raise ValidationError(_('Invalid date - not today's date'))

        return data
```

We defined a method for the class, that utilizes the *cleaned_data* to validate the data.