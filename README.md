# TrailPy

Proyecto personal para aprender:
- Git
- GitHub
- Java
- Linux
- desarrollo backend

## Comandos Git

### Inicializar repositorio

```bash
git init
```
Sirve para convertir una carpeta normal en un proyecto GIT 
y va aparecer una carpetita .git , donde se guardan historial, commits, ramas y cambios!

```bash
git add
```
Sirve para settear o preparar archivos para guardarlos, los coloca como en un carrito
cuando tenemos por ejemplo un 
Main.java 
y luego hacemos git add.
quiere decir que ese o esos archivos quiero incluir, 
el punto significa, todo lo que hay en la carpeta.


```bash
git commit 
```
esto guarda una version del proyecto, el " -m " significa mensaje 
por ejemplo 
git commit -m "cambio aplicado" ->>>> guarda esta version y describela asi
- un commit es una version guardada o checkpoint!

```bash
git remote add origin URL 
```
conecta tu proyecto local con github
origin = nombre del repositorio remoto


```bash
git push  
```
sube tus commits o avances a github
PC ->>>> github

```bash
git pull 
```
Esto trae cambios desde github a la PC 
github ->>>> PC 

```bash
git status 
```
Esto muestra archivos modificados, archivos nuevos y archivos listos para commit 
es tipo estado actual del proyecto

```bash
git branch -M main  
```
renombra la rama actual a main 
- una rama es una linea de desarrollo
- main es la rama principal 

```bash
git push -u origin main   
```
-git push es subir cambios 
-origin es al repositorio github
-main es a la rama main
- "-u" es recordar conexion futura

```bash
git pull --allow-unrelated-histories   
```
con esto forzamos la union de proyectos que parecen distintos!

### Flujo de trabajo tradicional
- git status
- git add .
- git commit -m "mensaje"
- git push










