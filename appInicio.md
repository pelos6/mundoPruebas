[mi mundo](miMundo.html) / [programacion](programacion.html) / [meteor](meteor.html) / appInicio 
#  app Inicio
<!-- MarkdownTOC -->

- [Proposito](#proposito)
- [crear una aplicacion con meteor](#crear-una-aplicacion-con-meteor)
- [cuentas de usuario](#cuentas-de-usuario)
- [bootstrap](#bootstrap)
- [mongodb](#mongodb)
- [session](#session)

<!-- /MarkdownTOC -->


# Proposito
Se crear una apliación sencilla propia desde el inicio usando lo que voy aprendiendo
# crear una aplicacion con meteor
````
meteor create tryMeteor
cd tryMeteor 
meteor
````
Asi se crea y se lanza en el puerto localhost:3000
C:\nube\MEGA\programacion\JavaScript\meteorJs\appInicio\tryMeteor>
el puerto se puede cambiar con 
```
meteor --port 3030
```

Quito el html del ejemplo que es un simple contador de click y pongo la barra de menu y el login.

# cuentas de usuario
para la autenticación con usuario se añade 
´´´
meteor add accounts-ui accounts-password
´´´ 
los paquetes nuevos se añaden en 
C:\nube\MEGA\programacion\JavaScript\meteorJs\appInicio\tryMeteor\.meteor\packages
Solo con esto ya tenemos implementado el login.
Incluido el  reenvio de contraseña al correo que se ha indicado.
En local ese correo se muestra por la consola del programa indicando el enlace que se usa para resetear la contraseña.
[más información](https://www.meteor.com/tutorials/blaze/adding-user-accounts)

# bootstrap
para usar bootstrap se tiene que añadir el paquete 
```
meteor add twbs:bootstrap
```
Se usa el repositorio de [meteor Atmosfere](https://atmospherejs.com/twbs/bootstrap)


# mongodb
para resetear la base de datos
```
meteor reset 
```

# session
```
meteor add session
```