django-custom-user
==================

A custom user model integrated with the default Django authentication backend. This is based on the feature added in Django 1.5, which allows you to create a custom user model to replace contrib.auth.models.User. The only pre-requisite for this is Django 1.5; if you have an older version and want to upgrade, look <a href="https://docs.djangoproject.com/en/dev/intro/install/">here</a>.

The CustomUser model isn't made to be too different from the default User. The biggest change is the absence of a 'username' field, and the 'email' being used as the unique identifier. The rest ofthe code demonstrates how to use the custom model with existing authentication resources:

<code>django.contrib.auth.forms.AuthenticationForm</code> - basic login form provided by Django

<code>django.contrib.auth.login,authenticate</code> - pre-defined methods to login and authenticate a user

See the Django <a href="https://docs.djangoproject.com/en/1.5/topics/auth/customizing/">docs</a>
for more info on customizing <code>contrib.auth</code>
