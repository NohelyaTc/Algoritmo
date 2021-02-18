# Algoritmo
DSM, rDSM, mDSM

# Requerimiento de software

MATLAB version R2017a

MATLAB es un sistema de cómputo numérico que ofrece un entorno de desarrollo integrado con un lenguaje de programación propio. Está disponible para las plataformas Unix, Windows, macOS y GNU/Linux. 

XAMPP version 3.2.4

XAMPP es un paquete de software libre, que consiste principalmente en el sistema de gestión de bases de datos MySQL, el servidor web Apache y los intérpretes para lenguajes de script PHP y Perl.

MOSEK version 9.2

MOSEK es un paquete de software para la solución de problemas de optimización matemática no lineal lineal, de entero mixto lineal, cuadrática, de entero mixto cuadrática, de restricción cuadrática, cónica y convexa no lineal.

# Instalación de software

Mosek: dispoble en www.monsek.com una vez instalado tiene que activarse la licencia. 



# Configuración de la base de datos 

Nos podemos encontrar el problema que el tamaño máximo a importar en phpmyadmin es inferior al tamaño de nuestra copia de la base de datos que queremos importar.

Para solucionar este problema tenemos que hacer lo siguiente:

Abrir el panel de control de Xampp. 

En el botón #config# muestra un menu de opciones seleccionar PHP(php.ini). 

Ir al archivo php.ini de nuestro Apache y buscar la línea donde tenemos: 

-upload_max_filesize

-post_max_size=4Mb

Normalmente el límite por defecto son 2 Mb, quedando de esta forma: 

-upload_max_filesize = 2M

-post_max_size= 2M

Poner en esa línea el tamaño máximo del archivo que importemos. Si queremos tener un máximo de 1000 Mb, por ejemplo, quedaría así: 

-upload_max_filesize = 1000M

-post_max_size= 1000Mb

Grabamos el archivo y reiniciamos apache.

Cuando volvamos a intentar importar un archivo en una base de datos en phpmyadmin tendremos un tamaño máximo de 1000 Mb.


## Run algoritmo

1. AbriR XAMPP e inicialiar los servicios de MySQL y Apache.
2. Cargar el archivo odbcconfig.mat
3. Abrir Matlab y cargar la carpeta que contienen el algorimo (Matlab).
    
    Ir a la pestaña |APP| y buscar |data base explorer| seleccionar |conecct|
    
    En la ventana colocar el usuario: gah y password:123456 de la ase de datos y concetar.

4. Inicializar Ipl.m ubicado en la carpeta src. 
5. Abrir config.m ubicado en src y ejecutarlo, abrira una ventana donde se selccioanra add patch. 
6. Correr main_dsrm.m el archivo principal del algoritmo. 




                                 
