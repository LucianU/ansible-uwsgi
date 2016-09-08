uwsgi
=====
Installs `uwsgi` and the config for the specified site.

Role Variables
==============
| Variable | Description | Default value |
|----------|-------------|---------------|
|`uwsgi_app_name`| Name of the uwsgi app | `none` |
|`uwsgi_module`| Import path to WSGI module | `{{ uwsgi_app_name }}.wsgi` |
|`uwsgi_socket`| Domain socket where uwsgi will listen for requests | `/run/uwsgi/app/{{ uwsgi_app_name }}/socket` |
|`uwsgi_venv` | Path to the site virtualenv | `{{ site_virtualenv }}` |

Dependencies
============
- [django-site](https://github.com/LucianU/ansible-django-site)

License
=======
BSD
