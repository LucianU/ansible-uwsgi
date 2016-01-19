uwsgi
=====
Installs `uwsgi` and the config for the specified site.

Role Variables
==============
| Variable | Description | Default value |
|----------|-------------|---------------|
|`uwsgi_config_dest`| location of the uwsgi config file for the Django site | `/etc/uwsgi/apps-available/{{ site_repo_name }}.ini` |
|`uwsgi_django_settings`| settings module of the Django site | `{{ site_django_settings }}` |
|`uwsgi_module`| wsgi module of the Django site | `{{ site_repo_name }}.wsgi` |
|`uwsgi_socket`| domain socket where uwsgi will listen for requests | `/run/uwsgi/app/{{ site_repo_name }}/socket` |
|`uwsgi_venv`| Django site's virtual env | `{{ site_virtualenv }}` |


Dependencies
============
- [django-site](https://github.LucianU/ansible-django-site)
