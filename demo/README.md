# Running the Deme

Create a virtual environment (running virtualenv) and point to python version 3.6:

```
virtualenv --python=python3.6 ~/swingenv
source ~/swingenv/bin/activate
```

Install the dependent libraries:

```
pip install -r requirements/demo.txt
```

This includes the django-modeltranslation, installing from the active development branch (pip install git+https://github.com/deschler/django-modeltranslation.git).

Build the database, load sample data, and run the application:

```
cd demo
python manage.py migrate
python manage.py loaddemo
python manage.py runserver
```

You can see the extra "translation" fields on the admin screens (admin/password).
