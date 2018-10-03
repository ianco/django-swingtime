# Running the Demo

Create a virtual environment (running virtualenv) and point to python version 3.6:

```
cd django-swingtime
virtualenv --python=python3.6 venv
source venv/bin/activate
```

Install the dependent libraries:

```
pip install -r requirements/demo.txt
```

This includes the django-modeltranslation, installing from the active development branch (pip install git+https://github.com/deschler/django-modeltranslation.git).

Load sample data (also builds the database) and run the application:

```
cd demo
./manage.py loaddemo
./manage.py runserver
```

You can see the extra "translation" fields on the admin screens (admin/password).
