# FinalProjectLaboPythonB2

Bienvenue dans mon projet de fin de labo Python pour l'année scolaire 2021/2022. Le but de ce projet était de découvrir le framework de développement web Django dans le but de créer une application web de messagerie type Whatsapp.

Pour lancer le projet il suffit de : 

- cloner le projet,

- aller dans "PythonFinal/PythonFinal/settings.py" et remplacer cette partie par vos identifiants (début ligne 84),

```
DB_NAME = "whatsapp"
DB_USER = "django"
DB_PASSWORD = "0000"
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': DB_NAME,
        'USER': DB_USER,
        'PASSWORD': DB_PASSWORD,
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

- lancer le projet avec la commande  ``python manage.py runserver``.
PS : si jamais les tables ne se créent pas directement faites ``python manage.py makemigrations`` puis ``python manage.py migrate``.
