[inicio](inicio.html) / [mi mundo](miMundo.html) / [programacion](programacion.html) / mongo 
#  Mongo
<!-- MarkdownTOC -->

- [Proposito](#proposito)
- [Consola de mongodb](#consola-de-mongodb)
- [mongoDB](#mongodb)

<!-- /MarkdownTOC -->

Se instala como parte de meteor.

* Sobre un curso de coursera 
* Es necesario un servidor para lanzar el programa que lo lleva el propio meteor
* recursos
    - [web de mongo ](https://www.mongodb.com)

# Proposito
Trastear con esta base de dato no sql parte de MEAN.
Importante recordar que no son tablas sino colecciones.



# Consola de mongodb
meteor mongo

# mongoDB
Instalo uMongo ligera y eficiente
http://edgytech.com/umongo/

desde el directorio donde se lanza meteor para que corra la aplicación
````
meteor mongo  
show databases 
````
 para ver las bases de datos que tenemos
````
meteor:PRIMARY> show collections
chats
meteor_accounts_loginServiceConfiguration
system.indexes
users
````

````
db 
````
dice la que estas usando
````
use <nombre base de datos> 
````

cambia de base de datos
````
db.users.find().pretty()  
````
muestra el contenido de esa colección formateado chulo.
````
db.users.find().count()   
````
el número de registros.
````
show collections   
````
muestra las colecciones 
````
db.<nombreCollection>remove()
````
o mejor drop()

