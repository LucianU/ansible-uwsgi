uwsgi
=====
Installs `uwsgi` and the config for the specified site.

Role Variables
==============
| Variable | Description | Default value |
|----------|-------------|---------------|
|`uwsgi_app_name`| Name of the uwsgi app | `none` |
|`uwsgi_socket`| Domain socket where uwsgi will listen for requests | `/run/uwsgi/app/{{ uwsgi_app_name }}/socket` |

Dependencies
============
none

License
=======
BSD
