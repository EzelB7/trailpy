# TrailPy

Proyecto de práctica y aprendizaje sobre programación, Git y desarrollo de aplicaciones.

## Tecnologías utilizadas
- Java
- Git
- GitHub
- Arch Linux
- Hyprland

## Comandos Git

### Inicializar repositorio
```bash
1- git init
```
Sirve para convertir una carpeta normal en un proyecto GIT 
y va aparecer una carpetita .git , donde se guardan historial, commits, ramas y cambios!

```bash
2- git add
```
Sirve para settear o preparar archivos para guardarlos, los coloca como en un carrito
cuando tenemos por ejemplo un 
Main.java 
y luego hacemos git add.
quiere decir que ese o esos archivos quiero incluir, 
el punto significa, todo lo que hay en la carpeta.


```bash
3- git commit 
```
esto guarda una version del proyecto, el " -m " significa mensaje 
por ejemplo 
git commit -m "cambio aplicado" ->>>> guarda esta version y describela asi
- un commit es una version guardada o checkpoint!

```bash
4- git remote add origin URL 
```
conecta tu proyecto local con github
origin = nombre del repositorio remoto


```bash
5- git push  
```
sube tus commits o avances a github
PC ->>>> github

```bash
6- git pull 
```
Esto trae cambios desde github a la PC 
github ->>>> PC 

```bash
7- git status 
```
Esto muestra archivos modificados, archivos nuevos y archivos listos para commit 
es tipo estado actual del proyecto

```bash
8- git branch -M main  
```
renombra la rama actual a main 
- una rama es una linea de desarrollo
- main es la rama principal 

```bash
9- git push -u origin main   
```
-git push es subir cambios 
-origin es al repositorio github
-main es a la rama main
- "-u" es recordar conexion futura

```bash
10- git pull --allow-unrelated-histories   
```
con esto forzamos la union de proyectos que parecen distintos!

## Branches 
Una branch es una linea de desarrollo independiente
la rama principal normalmente se llama 
``` bash 
main 
```

## Clonar proyecto 
``` bash
git clone URL
```

### Flujo de trabajo tradicional
- git status
- git add .
- git commit -m "mensaje"
- git push










