> [!IMPORTANT]
> Acordaros de hacer PULL cada vez que vayáis a editar vuestro código.

>[!NOTE]
>En está guía vais a encontrar:
>
>[Guía de ejecución de java en consola para dummies 😁](#guía-de-ejecución-de-java-en-consola-para-dummies-)
>
>[Como usar GIT en consola para dummies 🦥](#como-usar-git-en-consola-para-dummies-) 


## Guía de ejecución de java en consola para dummies 😁

### Antes de empezar a trabajar:

Copia el archivo `rutalaboratorio.bat` al directorio en el que vayas a realizar la práctica. 

Supongamos para el ejemplo que la ruta es `C:\Users\alg\Desktop\practicas\practica0`

<img width="1150" height="147" alt="imagen" src="https://github.com/user-attachments/assets/9854b42c-ef84-4717-911b-b99a54cbee61" />

#### Edita el archivo rutalaboratorio.bat

En el **set path** pondremos la ubicación del /bin del jdk de java.

>[!TIP]
> Podemos usar el comando `java -XshowSettings:properties -version` para identificar la ubicación de esta carpeta.
> 
> El directorio aparece referenciado en java.home (y al comienzo del java.library.path):
> 
> <img width="535" height="64" alt="imagen" src="https://github.com/user-attachments/assets/0669d314-2d5b-4149-973d-940cb4f41f77" />

En el **set classpath** pondremos la ruta de la práctica que contiene el fichero .java
<p align="center">
  <img width="450" height="49" alt="imagen" src="https://github.com/user-attachments/assets/31be971e-b44b-4dde-a18f-e6cb606aff77" />
</p>

### Ruta de Java y Compilación:

Muevete a la carpeta de la práctica dentro de la consola de comandos:
- Abriendo la propia carpeta desde el explorador y escribiendo cmd en la barra de búsqueda.
  
    <img width="562" height="86" alt="imagen" src="https://github.com/user-attachments/assets/3ac94dda-cf2f-4690-9f29-9d4a7f153557" />
    
- Escribiendo cmd en la barra del menú de inicio y navegando hasta la carpeta.
  
  <img width="248" height="65" alt="imagen" src="https://github.com/user-attachments/assets/ad8d6eac-8e9b-4659-98cc-d5620823bbb7" />
  
Ejecuto `rutadelaboratorio.bat` en el directorio de trabajo de la práctica **y no cierro la consola**.

<p align="center">
<img width="610" height="168" alt="Captura de pantalla 2026-01-29 121323" src="https://github.com/user-attachments/assets/aa17f6ac-02e9-4b8b-ad1f-611133fdb6dc" />
</p>

Acto seguido, vamos a compilar los .java con el comando `javac -d . *.java`
- `javac` es el comando para realizar la compilación de clases java, nos permite crear archivos .class
- la opción `-d .` nos crea el/los directorios que necesiten las clases. Si estas se encuentran todas en el paquete _algoritmia_ nos creará una carpeta con ese nombre. El `.` especifica que lo generará en el repositorio actual.
- `*.java` especifica que el comando afectará a todos los archivos con extensión .java de la carpeta.

Una vez ejecutado el comando y corregidos los posibles errores de compilación, en nuestro directorio de trabajo deberían haber aparecido las carpetas correspondientes a los paquetes definidos en las clases compiladas.

<p align="center">
<img width="477" height="79" alt="imagen" src="https://github.com/user-attachments/assets/07e8a68e-66d3-481b-b664-8beeb5e791e3" />
</p>
Dentro de la/s carpeta/s generada/s se encuentra el .class de las clases compiladas

### Ejecutar el código

> [!IMPORTANT]
> Desde la consola de comandos, debemos asegurarnos de estar en la carpeta del directorio de trabajo.
> En nuestro ejemplo **C:\Users\alg\Desktop\practicas\practica0**

>[!CAUTION]
>No cerréis la consola para parar la ejecución del programa.
>
>En su lugar emplead el comando `Ctrl + C`
>
>Si no lo hacéis así, tendréis que volver a ejecutar `rutalaboratorio.bat` para ejecutar en una consola nueva

>**JAVA CON OPTIMIZACIÓN**
>
>Ejecutamos el comando `java paquete.clase`
>
><img width="1259" height="215" alt="ejec1" src="https://github.com/user-attachments/assets/c64069af-8746-4026-af26-5783e60705fe" />

>**JAVA SIN OPTIMIZACIÓN**
>
>Ejecutamos el comando `java -Xint paquete.clase`
>
><img width="1259" height="215" alt="ejec" src="https://github.com/user-attachments/assets/c38a4bea-fa4f-4f5d-a7ca-f7331a0286eb" />

## Como usar GIT en consola para dummies 🦥

### Obtener el repositorio en el ordenador
Primero debéis acceder a vuestro repositorio en GitHub y localizar el botón `<> CODE`
<p align="center">
<img width="704" height="150" alt="Ubicacion del boton code en Github" src="https://github.com/user-attachments/assets/11d6241a-95e8-4581-92f2-d00d683a1bc4" />
</p>
A continuación, copiáis la URL del directorio. Basta con presionar el botón <img width="22" height="22" alt="icono del botón de copiar" src="https://github.com/user-attachments/assets/afc81ad0-cb1f-4e1f-ae19-b75441c45b48" />
 ubicado al lado del cuadro de texto.

<p align="center">
  <img width="374" height="101" alt="Co" src="https://github.com/user-attachments/assets/26d48f14-5e03-46af-a2aa-671853f01dca" />
</p>

Ahora debéis abrir una consola de comandos en el directorio donde querais almacenar el repositorio (puede ser el escritorio si es lo que más cómodo os resulta).
Para clonar el repositorio en vuestro ordenador debeis utilizar la instrucción `git clone URL`

<p align="center">
  <img width="782" height="47" alt="clonar un repositorio de git en local" src="https://github.com/user-attachments/assets/5661490f-1b0b-41d2-b0e1-375394663a8a" />
</p>

> [!IMPORTANT]
> Si ya teníais el repositorio descargado, debeis actualizarlo por si ha habido cambios.
> 
> Para ello debéis emplear el comando `git pull` desde el repositorio local.
> 
> <img width="782" height="101" alt="como hacer pull" src="https://github.com/user-attachments/assets/1c899702-dd63-466e-96c1-1dffff07ed0d" />

Ahora trabajáis normalmente, creáis los ficheros .java que haya que crear y hacéis las prácticas.
Una vez tengais los ficheros terminados, comprobais el estado del repositorio con `git status`:

<p align="center">
<img width="610" height="267" alt="3" src="https://github.com/user-attachments/assets/babb9949-ce57-401e-8f7c-7ffd04c343e4" />
</p>

### Añadir archivos al repositorio local
Para añadir los archivos al repositorio local tenemos dos opciones:

> **Añadir todos los archivos**
>
> Empleando el comando `git add *`
> 
> <img width="453" height="37" alt="imagen" src="https://github.com/user-attachments/assets/69feb285-9dab-4385-aff1-6cea7cf322b8" />


> **Añadir archivos de manera individual**
>
> Empleando el comando `git add archivo1, archivo2`
> 
> <img width="600" height="37" alt="imagen" src="https://github.com/user-attachments/assets/123eb6b1-32d4-4d8d-97a4-b39da786b2d1" />

Una vez añadidos, empleando el comando `git status` aparecerán en color verde
<p align="center">
<img width="574" height="242" alt="imagen" src="https://github.com/user-attachments/assets/136a003f-ec24-4eac-ac34-02ae4fb6104e" />
</p>

### Hacer COMMIT: Persistir los cambios en el repositorio local

Una vez hayáis añadido todos los cambios a vuestro repositorio local, debéis emplear la instrucción `git commit -m "_Mensaje del commit_"` para confirmar y registrar de forma permanente estas modificaciones en el historial de vuestro repositorio local.

<p align="center">
  <img width="717" height="151" alt="imagen" src="https://github.com/user-attachments/assets/70f47f0d-db80-4bf2-a010-6b5f3480ec0b" />
</p>

Podemos ver lo que hemos commiteado empleando el comando `git show`

<p align="center">
  <img width="496" height="266" alt="imagen" src="https://github.com/user-attachments/assets/10483609-12e5-4353-a800-7b62cecb9993"/>
</p>

> [!CAUTION]
>
> **Si queremos deshacer un commit porque hemos cometido un error** 
>
>| Comando  | Consecuencias |
>| ------------- | ------------- |
>| `git reset HEAD~1` | **No pierdes nada:** pero tendrás que hacer git add de nuevo para añadir los archivos  |
>| `git reset --soft HEAD~1` | **No pierdes nada:** pero tendrás que hacer git commit de nuevo, con un nuevo mensaje |
>| `git reset --hard HEAD~1`  | **Pierdes el commit y todos sus cambios**  |

### Subir los cambios a GitHub

Una vez tengamos commiteado todo lo que queremos subir, empleamos la instrucción `git push`

> [!WARNING]
>
> **Sobre el uso de `git push`:**
> 
> La instrucción push es muy compleja de revertir, sobretodo cuando se trabaja con más personas.
>
> Aseguraos siempre de pushear unicamente cuando el código realmente esté listo.

