### Guidelines related to Django Syntax
## Be explicit
	- Use `ModelName.DoesNotExist` instead of `ObjectDoesNotExist`.
	- Use `PositiveIntegerField`, `SmallIntegerField` and so on if it makes more sense,
	instead of always using the standard IntegerField
	- Always provide a related_name for Foreign Keys and Many to Many Relations.
	- Use `request_data` to hold POST request data.
	- Use `response_data` to hold data that you want to send in the response
	- Use `status_code` to hold the status of the response

## Better Usage
	- Instead of `if queryset: do something` use `if queryset.exists(): do something`
	- Use `DecimalField` instead of `FloatField` to store monetary information.
	- 

## Preferred
	- Instead of `django.contrib.auth.models.User`, use `settings.AUTH_USER_MODEL`. To query the User model,
	use `get_user_model()`.

## Beware:
	- Never use signals for calling third-party APIs.
	- 


### Docstrings and Comments
## Docstrings
	 - Every function/method/class should have a docstring


### Guidelines related to Python syntax
	- Use "4" spaces for indentation.
	- Every class should have `__str__` and `__repr__`.
	- Two spaces between any two classes/functions
	
## Imports
	- Organizing Imports:
		- Python Standard Libraries
		- Third Party Libraries (except Django and Rest Framework)
		- Django Imports
		- Rest Framework Imports
		- Application Imports
	- Imports should be in alphabetical order

## Naming conventions
	- Modules: lower_case_with_underscores
	- Packages: lowercase
	- Classes: CamelCase
	- Functions/Views: mixedCase
	- Methods/Variables: lower_case_with_underscores
	- Constants: UPPERCASE
	- Private Methods/Variables: _leading_underscore


### Some useful Python functions
	- map
	- lambda
	- dir
	- 
