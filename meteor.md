[mi mundo](miMundo.html) / [programacion](programacion.html) / meteor 
#  Meteor
<!-- MarkdownTOC -->

- [Proposito](#proposito)
- [Inicio](#inicio)
- [instalar](#instalar)
- [instalar meteor de nuevo](#instalar-meteor-de-nuevo)
- [crear una aplicacion con meteor](#crear-una-aplicacion-con-meteor)
- [hosting con meteor](#hosting-con-meteor)
- [hosting en heroku](#hosting-en-heroku)
- [Consolas](#consolas)
    - [Consola de meteor.](#consola-de-meteor)
    - [consola del server](#consola-del-server)
- [port](#port)
- [usuarios](#usuarios)
- [Final](#final)
- [practicas coursera](#practicas-coursera)
- [Cursos de Coursera](#cursos-de-coursera)
    - [Introducción al Desarrollo con Meteror.js](#introducción-al-desarrollo-con-meterorjs)
- [Web Application Development with JavaScript and MongoDB](#web-application-development-with-javascript-and-mongodb)
- [ Responsive Website Tutorial and Examples](#-responsive-website-tutorial-and-examples)
- [blog](#blog)
- [graficos y meteor](#graficos-y-meteor)
    - [Textcircle](#textcircle)
    - [aplicacion desde cero](#aplicacion-desde-cero)

<!-- /MarkdownTOC -->

Instalo meteor.js un framework que parece interesante 
* Sobre un curso de coursera 
* Es necesario un servidor para lanzar el programa que lo lleva el propio meteor
* recursos
    - [web de meteor instalación](https://www.meteor.com/install)


# Proposito
Trastear con meteor un framework cliente servidor con javascript.

# Inicio
Instalo meteor.js un framework que parece interesante …
se instala en 
C:\Users\Javier\AppData\Local\.meteor\packages

login en meteor
javieriranzo 
pelos678
javieriranzomicroscope.meteor.com

sigo este manual que parece bastante bueno y en castellano
http://es.discovermeteor.com/chapters/deploying/
y este curso en ingles.
https://www.coursera.org/learn/web-application-development/home/week/1

tutorial básico 
https://www.meteor.com/tutorials/blaze
el código … no veo como actualizar una tarea.
https://github.com/meteor/simple-todos
# instalar 
[instalar meteor desde cero](instalarMeteor.html)
# instalar meteor de nuevo 
C:\nube\MEGA\cursos\coursera\minstantJavier>meteor
""C:\Users\Javier\AppData\Local\.meteor\\packages\meteor-tool\1.3.2_3\mt-os.windows.x86_32\meteor.bat"" no se reconoce como un comando interno o externo,
programa o archivo por lotes ejecutable.

# crear una aplicacion con meteor
````
meteor create <nombre aplicacion>
cd <nombre aplicación> 
meteor
````
Asi se crea y se lanza en el puerto localhost:3000
aplicación de ejemplo con 
meteor create try-meteor en 
C:\nube\MEGA\programacion\JavaScript\meteorJs\appInicio\tryMeteor>

en otra consola se puede ver la consola de mongodb con 
meteor momgo
y alli para ver las bases de datos 
```
show dbs
```  
para ver las collections
```
show collections 
```

# hosting con meteor
Al principio pongo la aplicación de ejemplo en meteor 
http://javieriranzomicroscope.meteor.com/
pero dejan de ofrecer hosting gratuito y ofrecen estar alternativas

If you’re only looking for free hosting, we recommend using a combination of free services from Heroku and MongoLa# Here are links to some community articles to help you get started:

How to run a MeteorJS application on Heroku in 10 steps
Deploy to production on Heroku
You can also consult the Meteor Guide for other DIY deployment options.

Que parecen interesantes

# hosting en heroku
Uno de los ejemplos que ofrecen los chicos de meteor es un blog mediun que esta muy de moda.
https://medium.com/@leonardykris/how-to-run-a-meteor-js-application-on-heroku-in-10-steps-7aceb12de234?mkt_tok=3RkMMJWWfF9wsRonu6rNZKXonjHpfsX56OsvXKe2lMI%2F0ER3fOvrPUfGjI4ATMBnI%2BSLDwEYGJlv6SgFTLLCMbJ20LgEXxA%3D#.k1f31n2hd

en c:/var/www
meteor create foobar
cd foobar
http://localhost:3000

git init
git add .
git commit -m "My first commit!

heroku login
heroku git:remote -a portfoliojavier
git push heroku master

javieriranzo@hotmail.com
pelos678
heroku apps:create foobar

heroku buildpacks:set https://github.com/jordansissel/heroku-buildpack-meteor.git

heroku addons:create mongolab:sandbox
tengo que meter la tarjeta de crédito de ing 
heroku config 

=== foobarjavier Config Vars
MONGOLAB_URI: mongodb://heroku_xcx1nx9h:bqc38q5m814p4a8n695glnrn78@ds021989.mlab.com:21989/heroku_xcx1nx9h

heroku config:add MONGO_URL=mongodb://heroku_xcx1nx9h:bqc38q5m814p4a8n695glnrn78@ds021989.mlab.com:21989/heroku_xcx1nx9h
heroku config:add ROOT_URL=https://foobarjavier.herokuapp.com

c:\var\www\foobar>git remote -v
heroku  https://git.heroku.com/foobarjavier.git (fetch)
heroku  https://git.heroku.com/foobarjavier.git (push)

c:\var\www\foobar>git push heroku master
Counting objects: 13, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (9/9), done.
Writing objects: 100% (13/13), 2.51 KiB | 0 bytes/s, done.
Total 13 (delta 0), reused 0 (delta 0)
remote: Compressing source files.# done.
remote: Building source:
remote:
remote: -----> Fetching set buildpack https://github.com/jordansissel/heroku-buildpack-meteor.git.# done
remote: -----> meteor app detected
remote:
remote: -----> Moving app source into a subdirectory
remote:
remote:        Node engine:         0.10.40
remote:        Npm engine:          unspecified
remote:        Start mechanism:     none
remote:        node_modules source: none
remote:        node_modules cached: false
remote:
remote:        NPM_CONFIG_PRODUCTION=true
remote:        NODE_MODULES_CACHE=true
remote:
remote:        PRO TIP: Use 'npm init' and 'npm install --save' to define dependencies
remote:        See https://devcenter.heroku.com/articles/nodejs-support
remote:
remote:        PRO TIP: Include a Procfile, package.json start script, or server.js file to start your app
remote:        See https://devcenter.heroku.com/articles/nodejs-support#runtime-behavior
remote:
remote: -----> Installing binaries
remote:        Downloading and installing node 0.10.40...
remote:
remote: -----> Building dependencies
remote:        Skipping dependencies (no source for node_modules)
remote:
remote: -----> Checking startup method
remote:
remote: -----> Finalizing build
remote:        Creating runtime environment
remote:        Exporting binary paths
remote:        Cleaning up build artifacts
remote:        Build successful!
remote:        /tmp/build_8aeb225247e3504e6d0cc8952903bb76
remote:        └── (empty)
remote:
remote:
remote: -----> Fetching Meteor 1.2.1
remote:   % Total    % Received % Xferd  Average Speed   Time    Time     Time
Current
remote:                                  Dload  Upload   Total   Spent    Left
Speed
remote:   0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--remote:  21  147M   21 31.7M    0     0  41.5M      0  0:00:03 --:--:--  0:00:03remote:  51  147M   51 75.5M    0     0  42.8M      0  0:00:03  0:00:01  0:00:02remote:  81  147M   81  120M    0     0  43.5M      0  0:00:03  0:00:02  0:00:01remote: 100  147M  100  147M    0     0  44.0M      0  0:00:03  0:00:03 --:--:-- 44.0M
remote:
remote: -----> Unpacking Meteor 1.2.1
remote:        Meteor 1.2.1 is installed
remote:
remote: -----> Building Meteor App Bundle
remote:
remote: -----> Installing App's NPM Dependencies
remote:        npm WARN package.json meteor-dev-bundle@0.0.0 No description
remote:        npm WARN package.json meteor-dev-bundle@0.0.0 No repository field.
remote:        npm WARN package.json meteor-dev-bundle@0.0.0 No README data
remote:
remote:        > fibers@1.0.5 install /tmp/build_8aeb225247e3504e6d0cc8952903bb76/build/bundle/programs/server/node_modules/fibers
remote:        > node ./build.js
remote:
remote:        `linux-x64-v8-3.14` exists; testing
remote:        Binary is fine; exiting
remote:        ansi-regex@0.2.1 node_modules/ansi-regex
remote:
remote:        ansi-styles@1.1.0 node_modules/ansi-styles
remote:
remote:        escape-string-regexp@1.0.3 node_modules/escape-string-regexp
remote:
remote:        chalk@0.5.1 node_modules/chalk
remote:
remote:        strip-ansi@0.3.0 node_modules/strip-ansi
remote:
remote:        supports-color@0.2.0 node_modules/supports-color
remote:
remote:        has-ansi@0.1.0 node_modules/has-ansi
remote:
remote:        eachline@2.3.3 node_modules/eachline
remote:
remote:        type-of@2.0.1 node_modules/type-of
remote:
remote:        amdefine@1.0.0 node_modules/amdefine
remote:
remote:        asap@2.0.3 node_modules/asap
remote:
remote:        underscore@1.5.2 node_modules/underscore
remote:
remote:        meteor-promise@0.5.0 node_modules/meteor-promise
remote:
remote:        promise@7.0.4 node_modules/promise
remote:
remote:        source-map-support@0.3.2 node_modules/source-map-support
remote:
remote:        semver@4.1.0 node_modules/semver
remote:
remote:        source-map@0.1.32 node_modules/source-map
remote:
remote:        fibers@1.0.5 node_modules/fibers
remote:
remote: -----> Discovering process types
remote:        Procfile declares types     -> (none)
remote:        Default types for buildpack -> web
remote:
remote: -----> Compressing...
remote:        Done: 161.7M
remote: -----> Launching...
remote:        Released v6
remote:        https://foobarjavier.herokuapp.com/ deployed to Heroku
remote:
remote: Verifying deploy.# done.
To https://git.heroku.com/foobarjavier.git
 * [new branch]      master -> master


le cuesta un rato pero al final se puede ver la aplicación en esta url .
Antes salia un mensaje de bienvenida con una documentación de como desplegar 

https://foobarjavier.herokuapp.com/


c:\var\www\foobar>heroku addons:create papertrail:choklad
Creating papertrail-slippery-43962.# done, (free)
Adding papertrail-slippery-43962 to foobarjavier.# done
Setting PAPERTRAIL_API_TOKEN and restarting foobarjavier.# done, v7
Welcome to Papertrai# Questions and ideas are welcome (support@papertrailapp.com# Happy logging!
Use `heroku addons:docs papertrail` to view documentation.

Para ver los logs

# Consolas
## Consola de meteor.
Cd C:var/www/foobar/
meteor     --- para arrancar el servidor que se ve en http://localhost:3000

meteor search <nombre paquete> ---para buscar paquetes disponibles 
meteor list --- muestra los paquetes instalados

## consola del server 
meteor shell

en la consola del server salen por este orden los mensajes de  
lib
shared
server
y en la del navegador la de
lib
shared
client

# port
Meteor 
````
-- port 3030
````
para lanzarlo en otro puerto y poder correr dos aplicaciones 

# usuarios
javieriranzo@hotmail.com
pelos678

pilarvelasanz@hotmail.com
pilarvela 

mariairanzo@hotmail.com
maria6 

# Final
Dejo el ejemplo bajado de github
c:\var\www\github_microscope
meteor
http://localhost:3000/

lo copio en foobar que es el que esta sincronizado con heroku
desplegado en heroku
https://foobarjavier.herokuapp.com
panel en 
https://dashboard.heroku.com/apps/foobarjavier/activity

# practicas coursera
https://github.com/templetonpr
parece la tarea final .

# Cursos de Coursera
## Introducción al Desarrollo con Meteror.js
Buen ejemplo con imagenes.
Validación de usuarios
# Web Application Development with JavaScript and MongoDB
#  Responsive Website Tutorial and Examples
Con meteor es la 5 parte de un curso de web responsiva
15.# Despliegue en heroku

meteor create foobar
cd foobar

.- ya he creado antes la aplicación que portfoliojavier con algún problema sobre permisos ….

git init
git add .
git commit -m "My first commit!

heroku login
heroku apps:create portfoliojavier

Creating portfoliojavier.# done
https://portfoliojavier.herokuapp.com/ | https://git.heroku.com/portfoliojavier.git

heroku buildpacks:set https://github.com/jordansissel/heroku-buildpack-meteor.git

git push heroku master
--- pero da un problema ….
heroku addons:create mongolab:sandbox
--- antes había creado otro mongolab en heroku directamente.
Heroku config 
=== portfoliojavier Config Vars
MONGODB_URI:        mongodb://heroku_q96503hh:p570u99a07q9k1rse59heov6f6@ds021761.mlab.com:21761/heroku_q96503hh
MONGOLAB_BROWN_URI: mongodb://heroku_shz4125m:d7huktiopq29fvs2fgdfr3q73n@ds015929.mlab.com:15929/heroku_shz4125m
tengo que meter la tarjeta de crédito de ing 
heroku config 

=== foobarjavier Config Vars
MONGOLAB_URI: mongodb://heroku_xcx1nx9h:bqc38q5m814p4a8n695glnrn78@ds021989.mlab.com:21989/heroku_xcx1nx9h

heroku config:add MONGO_URL=mongodb://heroku_xcx1nx9h:bqc38q5m814p4a8n695glnrn78@ds021989.mlab.com:21989/heroku_xcx1nx9h
heroku config:add ROOT_URL=https://portfoliojavier.herokuapp.com

>git remote -v
heroku  https://git.heroku.com/portfoliojavier.git (fetch)
heroku  https://git.heroku.com/portfoliojavier.git (push)

la aplicación deja de dar error
creo el primer usuario (que por defecto es el administrador )  javieriranzo@hotmail.com pelos678


15.# practica obligatoria meteor-portfolio-website Compañeros
El de panama
https://github.com/FoxPowerGH/Meteor-Portfolio-Website.git

el del futbolista
https://github.com/lazygalaxy/portfolio-meteorjs-example.git

el mio 
portafolio_website_example

stanislaw 
un fotografo buen trabajo.

Tim blog
noticias de canada con facebook y disqus … muy bueno 
jane
sobre una danzarina … muy bueno tambien.
15.# de compañeros
package.json si existe en el directorio
npm install  y se crea node_modules ….

15.# Entrega segunda mia
Primero clono lo que tengo en heroku .

C:\nube\MEGA\cursos\coursera\CursowebResponsivaEjemplos\deHeroku
heroku git:clone -a portfoliojavier
$ cd portfoliojavier
no quito nada del directorio local pues esta la base de datos con los posts

solo consigo 7 de 8 así que tengo que mejorar
.- mas fotos
.- que sea responsivo el menú.

# blog
Ejemplo de blog ryw:blog que es la extensión que se usa en ese curso para esa semana.
https://github.com/meteor-blog/example-blog-app.git
C:\nube\MEGA\cursos\coursera\CursowebResposivaEjemplos\blogejemplo\
javier@hotmail.com
javier 
tiene facebook twiter y disqus
# graficos y meteor
http://www.highcharts.com/blog/195-meteor-standalone

clono 
https://github.com/khriztianmoreno/meteor-charts.git
que en un comentario dice que tiene un ejemplo.....
a ver si no da problemas de permiso de lectura con mongodb .
No da esos problema# (eran por la ñ del directorios compañeros !!!!!)

## Textcircle
Funciona y esta bien …..

javieriranzo@hotmail.com
javier 

## aplicacion desde cero
[notas sobre una aplicación propia desde el inicio](appInicio.html) 
