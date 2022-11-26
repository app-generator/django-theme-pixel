# [Django Theme Pixel](https://github.com/app-generator/django-theme-pixel)

Modern template for **Django** coded on top of **Pixel Lite**, an open-source `Boostrap 5` design from `Themesberg`. 

> Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.

<br>

**Links & Resources**

- [Django Theme Pixel](https://django-pixel-lite.appseed-srv1.com/) - LIVE Demo
- [Django Theme Pixel](https://github.com/app-generator/django-theme-pixel_p) - `playground project`
- UI Kit: [Pixel UI Kit](https://github.com/themesberg/pixel-bootstrap-ui-kit) `v4.1.0`

<br />

![Pixel Bootstrap Lite - Full-Stack Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/168753915-d61b2f97-57b2-4d14-a774-d217d120ff62.png)

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

**Pixel Lite** is a free and open-source [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) based user interface kit featuring over 80 fully coded UI elements and example pages that will help you prototype and build a website for your next project.

![Django Theme Pixel - About US page, product designed by Themesberg, coded by AppSeed.](https://user-images.githubusercontent.com/51070104/204097260-64e4db26-0096-46e5-90f7-24974ff40487.jpg)

<br />

> [Django Theme Pixel](https://github.com/app-generator/django-theme-pixel) - `Freelancer Page`

![Django Theme Pixel - Freelancer page, product designed by Themesberg, coded by AppSeed.](https://user-images.githubusercontent.com/51070104/204097202-00f62bf0-d32c-4249-a36e-3e929db369a8.jpg)

<br />

> [Django Theme Pixel](https://github.com/app-generator/django-theme-pixel) - `Contact US`

![Django Theme Pixel - Contact, product designed by Themesberg, coded by AppSeed.](https://user-images.githubusercontent.com/51070104/204097603-72a670aa-5ba2-4749-8b18-4655e6728d19.jpg)

<br />

---
**[Django Theme Pixel](https://github.com/app-generator/django-theme-pixel)** - Modern Theme provided by **[AppSeed](https://appseed.us/)**
