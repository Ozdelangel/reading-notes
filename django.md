If you need help with django go and dive into the docs at djangoproject.com
Terminal stuff
Create a folder or project to work with
Mkdir django-things 
Cd into it and then poetry init -n the reason we are using poetry is because django doesn’t come with python
Install django
We are next going to user django-admin startproject django_things
Do not use a underscore when you make a folder use underscore when you start your project
django-admin startproject django_things . remember to use the dot when making the project
Asgi a way to send messages and we are not using it
Whiskey.py for deployment but we are not using this but we may use it later
Settings.py we are going to use because we’re going to be playing around alot in there - the secret_key will be in there but don’t worry about it right now. It is potato you can make it anything you want
Debug set to true will help us when we need help but of course it won’t give us everything - when we convert it to false it won’t show to the user
Allowed hosts - intranet internal resources that people in you company will use
Sql lite database is built and it is a single file - good for making apps quickly - good for small things - size of the traffic
To run server python manage.py runserver
We have to set debug false
Allowed hosts and we can make allowed hosts to local host
Django gives us back end administration for free
Most of the time debug will be set to true
Python manage.py migrate
Django gives these things for free because our database is empty
CTRL C is how you shutdown the server
Adding an app to our project 
Python manage.py startapp things
It will make a folder
Admin folder will handle admin tasks
Apps.py - apps.config is the only thing we worry about
Models.py - user password and other things
Tests where we run tests
Views where we are gonna manage the views of our app
5. Telling our project that our app exists
Under installed apps add your app
Go into views to make template views - get rid of what they have
From django.views.generic import TemplateView - put this into views
Set up what your home page is going to look like
Create a class HomPageView(templateView)
Template_name = ‘home.html’ - its going to show what our html is going to look like
Modify your URL’s
Inside your app directory create a file called url.py - and it will handle routes within our application
Inside your application you need to build out the urls.py
Inside urls
Import paths from django.urls import path
Import views because the file needs to know about the home page view
Set an application pattern or url pattern is a route - we are going to handle the home route
Then there is going to be a variable called urlpatterns that is a list and its going to tell you where its going to urlpatterns=[ path(‘’, homepageview.as_view(), name=home’]
Its going to tell it where its going and its going to access the home route
Another path with same convention ‘’, include(things.urls’)

Four main                      
Add app
Adjust views
Adjust urls
Adjust templates
We need to do those things before anything else
Creating templates
Create a folder called templates 
Touch templates/home.html
Touch templates/base.html
Make an html file and inside the body (%block content%)
(%endblock content%)
Inside home.html (%extends.html%)
(%block content%)
(%endblock content%)
Add an h1^ 
One last piece to update inside project inside settings and inside or templates > dir> type BASE_DIR/’templates’
Testing
