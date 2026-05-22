#Comandos linux

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
- lista archivos ocultos

### 2.2 ls -l 

``` bash
ls -l 
```
- ver permisos 

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

### 11. history
```bash
history
```
- muestra los comandos anteriores 


### 12. !!
``` bash
!!
```
- repite el ultimo comando utilizado 

### 13. which 
```bash
which 
```
- te indica donde esta instalado un programa 
- por ejemplo
``` bash
which nvim 
```

## compresion 
- zip 
``` bash 
zip archivo.zip archivo.txt 
``` 

- unzip
``` bash 
unzip archivo.zip
```





## Busqueda 
``` bash
find
```
### find [ruta] [opciones]

- ejemplo 
```bash
find . -name "archivo.txt"
```

### "find ." 
- busca en el directorio o carpeta actual 
```bash
find .
```

### 1. "find . -name "main.java" " :
- con el "-name" busca por el nombre exacto 

```bash 
find . -name "archivo.txt" 
```
### 2. find . -iname "README.md" 
- el -iname ignora las mayusculas 

```bash 
find . -iname "README.md" 
```

### 3. find con * comodin
```bash
find . -name "*.java" 
```
- busca todos los .java 

```bash
find . -name "*.md"
```
- busca todos los .md

### 4. find con filtrado por tipo
```bash 
find . -type f 
```
- f= file/archivo , d = directory/directorio
- ejemplo con -type y -name 

``` bash 
find . -type f -name "*.txt"
```
- Esto busca todo los archivos .txt 

### 5. find con limite de profundidad 

``` bash
find . -maxdepth 1 
```
- Solo busca en la carpeta actual "1" 

### 6. find por tamano 
``` bash
find . -size +100M 
```
- mas de 100 MB

### 7. find para directorios vacios 
```bash
find . -type d -empty
```

### 8. find para eliminar 
``` bash
find [directorio] -name "*.txt" -delete
```
- esto elimina todos los .txt del directorio que coloques

## Redirecciones y pipes
``` bash
| 
``` 
- esto es un "pipe" 
- sirve para conectar comandos 
- ejemplo:

``` bash
ls | less 
```

### >
``` bash 
ls > archivo.txt
```
- Guardar la salida en un archivo con el " > "

### >> 
``` bash
echo "hola ">> notas.txt
```
- Agregar sin borrar 

## grep
- Sirve para buscar texto dentro de un texto y para combinar con | y filtrar  

## sintaxis basica

``` bash
grep [opciones] "text" archivo 
```

- Ejemplo 
``` bash
grep "hola" archivo.txt
```


## grep con ls 
- Ejemplo
```bash
ls | grep "md"
```
- Esto muestra solo archivos con .md 

## grep y numero de linea
- El "-n" indica en que numero de linea se encuentra lo que estamos  buscando
``` bash 
grep -n "main" Main.java 
```
## grep ignorando mayusculas
``` bash
grep -i "linux" archivo.txt 
```
- Esto te daria LINUX, linux, Linux y demas

## grep contar coincidencias
``` bash 
grep -c "error" logs.txt 
```
- Cuenta las coincidencias de error 

## grep busqueda recursiva
``` bash
grep -r "todo" 
```
- Va buscar "todo" en carpetas, archivos y demas!

## grep invertido 
```bash 
grep -v "java" archivo.txt
```
- Va mostrar todo quitando "java"

## grep solo nombres de archivos
``` bash
grep -l "java" 
```
- Muestra solo los nombres de archivos 

## grep recursivo y nombres de archivos
``` bash
grep -rl "todo"
```
- Va buscar recursivamente el nombre de archivo "todo" 

## grep con palabra exacta
``` bash 
grep -w "cat" archivo.txt
```
- va encontrar "cat" pero otra cosa como "categoria" no.

## grep linea exacta
``` bash 
grep -x "hola" archivo.txt 
```
- Debe salir exactamente hola 

## mostrar solo coincidencias
``` bash 
grep -o "linux" archivo.txt 
```
- Solo va mostrar las coincidencias sin enumerar. 

## grep regex 
``` bash
grep -E "java|python" archivo.txt 
```
- Busca java o python

## grep con color
``` bash 
grep --color "error" logs.txt 
```
- Colorea donde encuentre "error"
- se usan dos -- 

## grep mostrar n lineas despues de "busqueda"
``` bash 
grep -A 3 "error" logs.txt
```
- Encuentra "error" y va 3 lineas despues de eso 

## grep mostrar n lineas antes de "busqueda"
``` bash
grep -B 2 "error" logs.txt 
```
- Encuentra el "error" y muestra 2 lineas antes 

## grep con n lineas delante y atras de "busqueda"
``` bash
grep -C 2 "error" logs.txt 
```
- Muestra 2 lineas antes y despues de encontrar "error"

## grep con multiples patrones 
```bash 
grep -e "java" -e "python" archivo.txt 
```
- busca "java" y "python" y n cosas mas a medida que agregamos el " -e "

## grep con regex inicio  
``` bash
grep "^import" Main.java
```
- Las lineas que comienzan con import va mostrar, se utiliza el " ^ "

## grep con regex final
```bash 
grep "txt$" archivo.txt 
```
- todo lo que termine con txt 

## grep con comodin
``` bash
grep "h.la" archivo.txt
```
- El " . " punto se usa como comodin para autocompletar cualquier cosa
- hola, h0la, hila, etc.


## grep con comodin
``` bash
grep "h.la" archivo.txt
```
- El " . " punto se usa como comodin para autocompletar cualquier cosa
- hola, h0la, hila, etc.

## grep con conjunto de caracteres
``` bash 
grep "[aeiou]" archivo.txt 
```
- Cualquiera de estos caracteres quiere decir el " [] "
- Tambien sirve para numeros grep "[0-9]", establece un rango o de letras "[a-z]"

## grep para repeticiones
```bash 
grep "lo*" archivo.txt
```
- l + muchas "o", ejemplo l, lo, loo, looo, loooo, etc.

## Nota regex
- " . " = cualquier caracteres
- " * " = repetir lo anterior 








