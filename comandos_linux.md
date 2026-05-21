# Comandos linux

## Navegacion 

### 1. pwd
``` bash
pwd
```
- muestra ubicacion actual / directorio actual 

### 2. ls 
``` bash
ls
```
- Lista archivos

### 2.1 ls -la 
```bash 
ls -la 
```
- lista archivos ocultos tambien

### 3. cd 
```bash
cd  
```
- Sirve para cambiar de carpeta o directorio

### 3.1 cd .. 
``` bash
cd ..
```
- Vuelve una carpeta atras


### 4. touch 
```bash 
touch 
```
- Touch sirve para crear un tipo de archivo con una extension definida
por el programador, touch archivo.txt

### 5. mkdir 
```bash
mkdir 
```
- Sirve para crear una carpeta/directorio, mkdir carpeta_nombre 

### 6. rm 
```bash 
rm 
```
- Sirve para eliminar un archivo, rm archivo.txt

### 6.1 rm -r 
```bash
rm -r 
```
- eliminacion recursiva, sirve para borrar carpetas

### 7. cp 
```bash
cp 
```
- sirve para copiar archivos, cp archivo.txt copia.txt 

### 8. mv 
``` bash
mv
```
- Sirve para mover o renombrar mv archivoamover.txt rutanueva

- mv archivo.txt nuevonombre.txt

### 9. cat 
``` bash
cat
```
- Sirve para mostrar el contenido de un archivo, ejemplo:
cat archivo.txt

### 10. less
``` bash
less 
```
- Sirve para leer archivos largos, ejemplo:
less archivo.txt

## Busqueda 
``` bash
find
```
### find [ruta] [opciones]

- ejemplo 
```bash
find . -name "archivo.txt"
```

### "find ." busca en el directorio o carpeta actual 
```bash
find .
```

### "find . -name "main.java" " con el "-name" busca por el nombre exacto 

```bash 
find . -name "archivo.txt" 
```
### find . -iname "README.md" ignora las mayusculas 

```bash 
find . -iname "README.md" 
```

### find con * comodin
```bash
find . -name "*.java" 
```
- busca todos los .java 

```bash
find . -name "*.md"
```
- busca todos los .md











