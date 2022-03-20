# Permissions

- This is basically a part of your code that determines if a permission is granted or denied access

- Permissions uses the `request.user`and `request.auth` properties to determine if the incoming request should be permitted

- This corresponds to the `IsAuthenticated` class in the DRF

- you can choose what kind of permission a user has another one that we are familiar with is `IsAuthenticatedOrReadOnly` basically means they can see it bu they can't add or delete any items from the database

# Object level Permissions
 - Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance

 # Setting the permission policy 

 - this is what we put in our settings.py in your project level of the django project 

 `REST_FRAMEWORK = {`
    `'DEFAULT_PERMISSION_CLASSES': [`
        `'rest_framework.permissions.IsAuthenticated',`
    `]`
`}`

at the end of the list is where you will set the default, we also used `AllowAny`

## Allowany
- this permission class will allow unrestricted access to all CRUD functions.

## IsAuthenticated
- this permission class will deny permission to any unauthenticated user, and allow permission otherwise

## IsAdminUser

- this permission class will deny permission to any user, unless `user.is_staff` is `True`

## IsAuthenticatedOrReadOnly
- this permission will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the safe methods like get, head, or options.
