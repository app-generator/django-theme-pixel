# [Django Theme Pixel](https://github.com/app-generator/django-theme-pixel)

Modern template for **Django** coded on top of **Pixel Lite**, an open-source `Boostrap 5` design from `Themesberg`. 

> Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.

<br>

**Links & Resources**

- [Django Theme Pixel](https://django-pixel-lite.appseed-srv1.com/) - LIVE Demo
- [Django Theme Pixel](#) - `playground project` (soon) 
- UI Kit: [Pixel UI Kit](https://github.com/themesberg/pixel-bootstrap-ui-kit) `v4.1.0`

<br />

![Pixel Bootstrap Lite - Full-Stack Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/168753915-d61b2f97-57b2-4d14-a774-d217d120ff62.png)

<br />

## `Video Presentation`

> This material provides `more information` about this library and the `playground project`.

@ToDo

<br />

## Why `Django Pixel Lite`

- Modern `Bootstrap 5` Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`
- ALL `UI KIT` pages available

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install django-theme-pixel
// OR
$ pip install git+https://github.com/app-generator/django-theme-pixel.git
```

<br />

> Add `theme_pixel` application to the `INSTALLED_APPS` setting of your Django project `settings.py`:

```python
INSTALLED_APPS = [
    "django.contrib.admin",
    "django.contrib.auth",
    "django.contrib.contenttypes",
    "django.contrib.sessions",
    "django.contrib.messages",
    "django.contrib.staticfiles",

    'theme_pixel',          # <-- NEW 
]
```

<br />

> Update project `settings.py` file to include (at the end of the file):

```python
LOGIN_REDIRECT_URL = '/'
EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `theme_pixel` urls in your Django Project `urls.py` file.

```python
from django.urls import path, include       # <-- UPD with 'include' directive

urlpatterns = [
    ...
    path('', include('theme_pixel.urls')),  #  <-- NEW
]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

<br />

## Screenshots

@ToDo

<br />

---
**[Django Theme Pixel](https://github.com/app-generator/django-theme-pixel)** - Modern Theme provided by **[AppSeed](https://appseed.us/)**
