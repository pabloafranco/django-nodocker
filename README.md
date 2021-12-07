# docker- nodjango

Para inicializar el proyecto necesito:

1. instalar python 3+
2. instalar paquetes necesarios que no se encuentran en "requeriments.txt"
 con el comando pip install -r requeriments.txt
3. instalar MySql e inicializar el servicio
4. Ejecutar el initial.sql para crear el schema de django


## Creamos el proyecto django

django-admin startproject [nombre del proyecto] .

## Confirguramos el proyecto con nuestra base de datos

Modificamos el archivo setting.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'django',
        'USER': 'userdjango',
        'PASSWORD': 'passworddjango',
        'HOST': 'localhost',
        'PORT': 3306,
    }
}

## Ahora ya podemos crear nuestra app con el siguiente comando

python manage.py startapp {reemplazar por nombre de aplicacion}

