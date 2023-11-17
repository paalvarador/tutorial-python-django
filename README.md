# Tutorial de Python Django

!(assets/images/python-django.png)

## Capítulos

1. Instalación y Configuracion de Django

- Guia paso a paso para instalar Django
- Configuración inicial del proyecto
- Actvar el entorno virtual del proyecto

2. Estructura del proyecto Django

- Explicación de la estructura de archivos y carpetas
- Descripción de cada componente importante

3. Creación de modelos

- Definición de modelos y relaciones
- Uso de migraciones para actualizar la base de datos

4. Vistas y templates

- Creación de vistas y su relación con las URLs
- Uso de templates para renderizar páginas

5. Formularios en Django

- Creación y manejo de formularios
- Validación y personalizaciones

6. Autenticación y autorización

- Implementación de sistemas de autenticación
- Control de acceso a vistas y recursos

7. APIs en Django

- Creación de una API simple
- Uso de serializadores y vistas basadas en clases

8. Despliegue

- Opciones para desplegar una aplicación Django
- Configuración básica de servidores web

## 1. Instalación y Configuración de Django

# Creando el primer proyecto ej Django

Para crear un proyecto en Django debemos realizar los siguientes pasos:

1. Crear una carpeta en cualquier lugar de nuestra computadora. Por ejemplo
   crearemos una carpeta llamada storefront en el escritorio y luego ejecutamos
   el comando:

| Comando               | Descripción                                       |
| --------------------- | ------------------------------------------------- |
| pipenv install django | Este comando instala Django en un entorno virtual |

```
~ cd Desktop
~ mkdir storefront
~ cd storefront
~ pipenv install django
```

Cuando se crear el proyecto con pipenv se crea todo lo necesario para poner el
proyecto en un entorno virtual.

# Activación del Entorno Virtual

Una vez creado el proyecto debemos activar el entorno virtual donde se encuentra
el proyecto. Esto lo podemos realzar con el siguiente comando

```
~ pipenv shell
```

Una vez activado el entorno virtual, se procede a crear el proyecto con el
siguiente comando

```
~ django-admin startproject storeproject .
```

El punto (.) es usado para que el proyecto se cree en la raiz del proyecto

## 2. Estructura del Proyecto

Una vez creado el proyecto se crea la siguiente estructura

[-] (root folder) STOREFRONT
[-] (app folder) storefront
[-] **init**.py
[-] asgi.py
[-] settings.py
[-] urls.py
[-] wsgi.py
[-] db.sqlite3
[-] manage.py
[-] Pipfile
[-] Pipfile.lock
[-] Readme.md

# Ejecutar el proyecto

Una vez que nuestro proyecto se encuentra creado podemos usar el siguiente
comando para iniciar nuestro servidor de pruebas y ver el funcionamiento

```
$ python manage.py runservrer
```
