# Creación de una aplicación en Django, y publicación en Heroku
Pasando por GitHub, para control de versiones.

Si todo va bien, este documento se podrá usar como guía para hacer un proyecto sencillo.

Para desarrollar este proyecto se ha instalado
* Python 3.8.10
* Django 3.2.6

Iremos dejando algunas configuraciones para la etapa de compilación, para que nos den errores, y conocer cómo podemos enfrentarlos.


1. [Puesta en marcha del server de Django (40 min)](https://github.com/gianfranco-s/tutorial-django/blob/main/1.%20Puesta%20en%20marcha%20del%20server%20de%20Django.ipynb)  
  1.1 Iniciar un entorno virtual (`venv`)  
  1.2 Instalar Django  
  1.3 Crear el proyecto  
  1.4 Configuración de **settings.py**  
  1.5 Configurar la base de datos  
  1.6 Iniciar el servidor  

2. [Ahora sí, programemos el backend en Django](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#2-ahora-s%C3%AD-programemos-el-backend-en-django)  
  2.1  [Flujo de información en Django](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#21-flujo-de-informaci%C3%B3n-en-django)  
  2.2  [Creación de una vista (view)](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#22-primera-vista)  
  2.3  [View en base a una plantilla (template)](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#23-primera-vista-ahora-con-un-template)  
  2.4  [Un buen momento para subir el proyecto a un hosting SaaS]()  
  2.5  [Creación de una segunda app](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#24-creaci%C3%B3n-de-una-segunda-app)  
  2.6  [Modelos en Django](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#25-modelos-en-django)  
  2.7  [Base de datos en Django](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#26-opcional-interacci%C3%B3n-con-la-base-de-datos)  
  2.8  [Django admin](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#27-django-admin)  
  2.9  [Presentación de contenido](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#28-presentaci%C3%B3n-de-lista-de-ejercicios)  
  2.10 [Página de inicio](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#29-p%C3%A1gina-de-inicio)  
  2.11 [Creación de aplicación **accounts**](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#211-creaci%C3%B3n-de-aplicaci%C3%B3n-accounts)  
    2.11.1 [Asociación de Signup](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#2111-asociaci%C3%B3n-de-signup-con-accounts)  
    2.11.2 [Crear formulario de Login](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#2112-crear-el-formulario-de-ingreso)  
    2.11.3 [Guardar cuentas de usuarios](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#2113-guardar-y-validar-cuentas-de-usuario)  
    2.11.4 [Configurar ingreso de usuarios](https://github.com/gianfranco-s/tutorial-django/blob/main/2.%20Ahora%20s%C3%AD,%20programemos%20el%20backend%20en%20Django.md#2114-ingreso-de-usuarios)  

3. Vamos con el frontend!  
  3.1 Configuración de archivos estáticos  
  3.2 Extender templates  
  3.3 Utilización de archivos css e imágenes  
  3.4 ¿Algo de Bootstrap?  
  3.5 Y una pizca de Vue  
  
4. Creación y manejo del repositorio en GitHub  

5. Publicar en Heroku  
  5.1 Crear la aplicación  
  5.2 Configurar **settings.py**  
  5.3 Subir el sitio  
  
  
