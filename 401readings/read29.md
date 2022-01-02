# Django Custom User

You can customize the default user model provided by django using : *custom user model*

1- in settings.py, add this line: ``` AUTH_USER_MODEL = 'accounts.CustomUser' ```

2- add the custom user model in models.py (you can also use CustomUserCreationForm, CustomUserChangeForm models, they have different features) 

```
from django.contrib.auth.models import AbstractUser
from django.db import models

class CustomUser(AbstractUser):
    pass
    # add additional fields in here

    def __str__(self):
        return self.username
```

3- create a superuser to login to the admin page ```$ python manage.py createsuperuser```


## (Django X)[https://github.com/wsvincent/djangox]

this is a django starter code, with the following features:

- Django 3.1 & Python 3.8
- Install via Pip, Pipenv, or Docker
- User log in/out, sign up, password reset via django-allauth
- Static files configured with Whitenoise
- Styling with Bootstrap v4
- Debugging with django-debug-toolbar
- DRY forms with django-crispy-forms
