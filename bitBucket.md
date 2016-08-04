# BitBucket
uso [bitBucket](https://bitbucket.org/pelos6) porque me permite tener repositorios privados.
Necesito tener [git](git.html) instalado.
## primero creo el repositorio en la web de nombre mundo.
[repositorio mundo](https://bitbucket.org/pelos6/mundo)
## luego en el ordenador donde comienzo
```
cd C:\nube\MEGA\mundo
git init
git remote add origin https://pelos6@bitbucket.org/pelos6/mundo.git
```

## luego subo el contenido del directorio
```
git add -A
git commit -m "primer commit"
git push -u origin master
```

problemas con la cache .. se dieron al cambiar el nombre de los archivos
```
git rm -r --cached .
git add .
git commit -am "cache limpia"
git push
```


para recuperar los cambios en otro directorio de trabajo
```
git pull
```
## Para usarlo en el ordenador nuevo
cd c:/nube/mega
git clone https://pelos6@bitbucket.org/pelos6/mundo.git

##Sublime y Git BitBucket
###SublimeGit  
http://www.azulweb.net/integra-git-en-sublime-text-3/
con ctrl + mayus + p se pueden ver los comando de Git:status 
que sale información muy interesante.
pero no consigo que funcione bien con el repositorio de bitBucket 
Lo dejo instalado 
[Instrucciones del package control](SublimeGitPackageControlMessages.md)
el push lo hago a mano mientras investigo como solucionarlo.
###sublime-github
###GitLink
Te dice que enlace tiene tu archivo incluso a nivel de linea y te puede llevar a esa URL
