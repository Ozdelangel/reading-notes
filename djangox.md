Django x

First we’re going to go to the djangox repository and use the template that is provided by 
Will vincent.
Then you are going to clone it down to your local computer
Go to your template repository that you just cloned down
Do some clean up and get rid of things that you are not going to need in your local repository
Then you have to do all the necessary things that have to do with poetry 
Poetry add django
Poetry add django-allauth
Poetry add django-crispy-forms django-debug-toolbar and white nose
Shell up and code up when you are done check that you got all your dependencies in your toml. 
Then migrate, create super user, then run server - what is django doing when running migrate? It is running our database and its building all the tables that are in the admin console
Go through the djangox homepage and explore all the settings make a user and look around
Note: when possible separate out your installe apps in settings.py
Next you are going to add an application python manage.py startapp <your-app>
Like always go to your setting.py and put it in your installed apps
Make your urls in you application - touch <app-name>/urls.py
In your urls.py you are going to want to put in all your views
