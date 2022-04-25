# django+mysql template

## make project
Build image.
```
docker-compose build
```

make prooject
```
docker-compose run web --rm sh -c "django-admin startproject {projectname} ."
```

Open {project name}/settings.py and fix.
```python:settings.py
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'django-db',
        'USER': 'django',
        'PASSWORD': 'django',
        'HOST': 'db',
        'PORT': '3306'
    }
}
```
All services up
```
docker-compose up -d
```
[next](https://qiita.com/bakupen/items/f23ce3d2325b4491a2dd)
template
