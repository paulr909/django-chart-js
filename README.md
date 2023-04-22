[![Python Version](https://img.shields.io/badge/python-3.10-brightgreen.svg)](https://python.org)
[![Django Version](https://img.shields.io/badge/django-4.2-brightgreen.svg)](https://djangoproject.com)

# Django with Chart JS

Run your app in a Virtual Environment: http://python-guide-ru.readthedocs.io/en/latest/dev/virtualenvs.html

```shell
python -m venv venv && source venv/bin/activate
```

Generate SECRET_KEY:
```shell
python -c 'from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())'
```

Install the requirements:
```shell
pip install -r requirements.txt
```

Apply the migrations:
```shell
python manage.py migrate
```

Populate the database with randomly generated data (amount = number of purchases):
```shell
python manage.py load_data --amount 2500
```

Create a superuser, and run the server:
```shell
python manage.py createsuperuser
python manage.py runserver
```

- [http://127.0.0.1:8000/shop/statistics/](http://127.0.0.1:8000/shop/statistics/) -
  Stats view
- [http://127.0.0.1:8000/admin/statistics/](http://127.0.0.1:8000/admin/statistics/) -
  Admin view
- [http://127.0.0.1:8000/admin/shop/](http://127.0.0.1:8000/admin/shop/) - Extended
  admin view
