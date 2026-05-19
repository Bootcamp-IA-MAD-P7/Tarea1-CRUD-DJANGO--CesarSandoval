# Tarea1-CRUD-DJANGO--CesarSandoval
Este documento sirve como Readme - Respuesta a tarea 1

## CRUD

Es una nomenclatura que se usa para identificar los 4 procesos claves de la gestión y manipulación de datos  como son: Create Read Update Delete
El fin es que este organizado y automatizado este proceso ya que antiguamente esto se hacia a mano.

## PATRONES
Son formas de trabajo que nos permiten organizar de manera eficiente el mantenimiento y escalibilidad asi como la colaboración en el proceso de desarrollo

**MVC**

Es el patron de modelo vista controlador 
 - Modelo que maneja la lógica del negocio
 - Vista  que es la interfaz del usuario
 - Controlador que recibe la información del usuario y decide que vista va.

**MVT**

 Es la misma lógica solo que es usada por Django
 - Modelo  que maneja Datos y BD
 - Vista que contiene la lógica
 - Template que es la parte visual HTML

## DIFERENCIAS 
 Si bien tienen ciertas diferencias en como manejan las peticiones el enfoque es el mismo. Solo que la intefaz visual responde a una plantilla.
Django usa principalmente MVT

## ESTRUCTURA
Un proyecto en Django se estructura en dos bloques principales PROYECTO y APPS 
El Proyecto es el contenedor de los apps.
Dentro de proyecto esta la parte critica de configuración  y en las apps tenemos los modelos vistas y templates
Adicional en esta sección app tenemos uno llamado admin, que se autogenera.

## PARA QUE SE USA %%
Se usa para mostrar lógica o código en los templates, y cuando van sin %% u solo va {{}}es porque se muestran variables

## FLUJO DE DATOS ENTRE FORM HTML y BD DJANGO
    USUARIO LLENA FORM --> 
                FORM ENVIA DATOS CON POST -->
                                VIEW RECIBE DATOS  --> 
                                             DJANGO VALIDA --> 
                                                       MODELO GUARDA DATA EN BD --> 
                                                                 DJANGO DEVUIELVE RESPONSE O REDIRECT

Eso se puede resumir como 
HTML FORM --> VIEW --> BASE DE DATOS

## HERRAMIENTAS DE DJANGO PARA FACILITAR CRUD
* STARTUP  Crea una aplicacion
* MAKEMIGRATIONS  Genera files de migracion
* MIGRATE		Aplica los cambios a la DB
* RUNSERVER	Inicia servidor de desarrollo
* MODELFORM	Genera formularios basado en modelos
* ADMIN		Genera un panel de administrador
* CREATESUPERUSER	 Crea el Admin master del app o sistema.

## ADMIN DE DJANGO
Este se genera de manera automatica permitiendo hacer CRUD del objeto o clase usuario.
Para esto solo necesitamos registrar el modelo admin.py  crear el usuario y luego ingresar  a /admin

## DJANGO Y REST
Django no es REST de origen pero es posible hacer desarrollo a traves de API REST

REST Es un estilo de arquitectura para crear APIS usando HTTP
Tiene 4 metodos GET POST PUT DELETE

## DJANGO REST FRAMEWORK
Es una libreria que facilita la implementacion de API REST en Django.