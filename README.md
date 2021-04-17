# Tweety Django Backend
This is a repository for video series "About Monolith vs. Microframeworks 
Journey".

# Setup
Follow these steps for each Tutorial:
1. Clone Repository
```
git clone git@github.com:FullTweety/django-backend.git
```

2. Install Python packages (virtual environment is required)
```
pip install -r requirements.txt
```

3. Init & Update Submodule
```
git submodule init
git submodule update
```

## Setup Part 1 - Django Basics
For being able to setup the very first part checkout tag `initial_setup`
```
git checkout tags/initial_startpoint -b master
```

# Django Commands
1. Start the django server for being able to access your homepage.
```
python manage.py runserver
```

2. Create a superuser. Please note: This is just possible on an already 
    migrated database.
```
python manage.py createsuperuser
```

3. Create migrationfiles for giving the database the possibility to understand
    your models. _That command won't have any effect on your database yet._
    _It's just a required preparation._

```
python manage.py makemigrations
```

4. Migrate your models into your database. This will makes direct changes at
    your database. I recommend you to be very careful with it.
```
python manage.py migrate
```

5. Access the Django Shell. It might be useful at some points to work directly
    at your server without writing any files. It's recommended for some quick
    changes or insights.
```
python manage.py shell
```
