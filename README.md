# Proyecto - Java VideoStore con Pruebas para Autograding - Maven

**VideoStore** es una App Java desarrollada para gestionar el Punto de Venta de una tienda de renta de Videos.

La tienda ofrece a sus clientes tres tipos de películas:

* REGULAR
* NEW_RELEASE
* CHILDREN

Su equipo ha recibido la última versión de la App, la cual posee varios defectos. 

Se les ha encomendado la tarea de detectar y corregir los mismos y verificar su eliminación mediante un conjunto pruebas unitarias (incluidas). 
Utilice las herramientas y técnicas estudiadas para dar mantenimiento a esta aplicación

## Versión de Java

Verifica que tengas la versión adecuada de Java para trabajar con Maven. En caso de requerir una versión especial, usa los siguientes comandos.

### Verificar versión actual
```
java --version
```
### Verificar versiones disponibles para instalar
```
sdk list java
```
### Instalar la última versión
```
sdk install java
```
### Instalar una versión específica
```
sdk install java xxx-version
```
Ejemplo:
```
sdk install java 17.0.18-ms
```

## Uso del proyecto con Maven

### Compilar
```
mvn compile
```
### Probar N tests
```
mvn test
```
### Probar 1 test
```
mvn test -Dtest="AppTest#testSingleNewReleaseStatement"
mvn test -Dtest="AppTest#testDualNewReleaseStatement"
mvn test -Dtest="AppTest#testSingleChildrensStatement"
mvn test -Dtest="AppTest#testMultipleRegularStatement"
mvn test -Dtest="AppTest#testRentalStatementFormat"

```
### Ejecutar App
```
java -cp target/classes miPrincipal.App
```
### Ejecutar App con Maven
```
mvn -q exec:java
```
### Empacar App
```
mvn package
```
### Limpiar binarios
```
mvn clean
```
## Comandos Git-Cambios y envío a Autograding

### Por cada cambio importante que haga, actualice su historia usando los comandos:
```
git add .
git commit -m "Descripción del cambio"
```
### Envíe sus actualizaciones a GitHub para Autograding con el comando:
```
git push origin main
```
Los comandos anteriores están considerados para un ambiente Linux. [Referencia.](https://www.baeldung.com/junit-run-from-command-line)
