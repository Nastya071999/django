# django
Microsoft Windows [Version 10.0.17763.1879]
(c) Корпорація Майкрософт (Microsoft Corporation), 2018. Усі права захищено.

C:\Users\Hewlett Packard>cd djangogirls

C:\Users\Hewlett Packard\djangogirls>python
Python 3.4.3 (v3.4.3:9b73f1c3e601, Feb 24 2015, 22:44:40) [MSC v.1600 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> quit
Use quit() or Ctrl-Z plus Return to exit
>>> quit()

C:\Users\Hewlett Packard\djangogirls>python -m venv myvenv

C:\Users\Hewlett Packard\djangogirls>myvenv\Scripts\activate
(myvenv) C:\Users\Hewlett Packard\djangogirls>pip install django==1.11
You are using pip version 6.0.8, however version 21.1.1 is available.
You should consider upgrading via the 'pip install --upgrade pip' command.
Collecting django==1.11
  Downloading https://files.pythonhosted.org/packages/47/a6/078ebcbd49b19e22fd560a2348cfc5cec9e5dcfe3c4fad8e64c9865135bb/Django-1.11-py2.py3-none-any.whl (6.9MB)
    100% |################################| 6.9MB 40kB/s
Collecting pytz (from django==1.11)
  Downloading https://files.pythonhosted.org/packages/70/94/784178ca5dd892a98f113cdd923372024dc04b8d40abe77ca76b5fb90ca6/pytz-2021.1-py2.py3-none-any.whl (510kB)
    100% |################################| 512kB 168kB/s
Installing collected packages: pytz, django


Successfully installed django-1.11 pytz-2021.1

(myvenv) C:\Users\Hewlett Packard\djangogirls>django-admin startproject mysite .

(myvenv) C:\Users\Hewlett Packard\djangogirls>python manage.py migrate
Operations to perform:
  Apply all migrations: admin, auth, contenttypes, sessions
Running migrations:
  Applying contenttypes.0001_initial... OK
  Applying auth.0001_initial... OK
  Applying admin.0001_initial... OK
  Applying admin.0002_logentry_remove_auto_add... OK
  Applying contenttypes.0002_remove_content_type_name... OK
  Applying auth.0002_alter_permission_name_max_length... OK
  Applying auth.0003_alter_user_email_max_length... OK
  Applying auth.0004_alter_user_username_opts... OK
  Applying auth.0005_alter_user_last_login_null... OK
  Applying auth.0006_require_contenttypes_0002... OK
  Applying auth.0007_alter_validators_add_error_messages... OK
  Applying auth.0008_alter_user_username_max_length... OK
  Applying sessions.0001_initial... OK

(myvenv) C:\Users\Hewlett Packard\djangogirls>python manage.py runserver
Performing system checks...

System check identified no issues (0 silenced).
May 07, 2021 - 11:58:44
Django version 1.11, using settings 'mysite.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.
[07/May/2021 12:04:31] "GET / HTTP/1.1" 200 1716
Not Found: /favicon.ico
[07/May/2021 12:04:31] "GET /favicon.ico HTTP/1.1" 404 1962
