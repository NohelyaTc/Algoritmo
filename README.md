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
Mosek: una vez instalado tiene que activarse la licencia. 


## Run algoritmo

1. AbriR XAMPP e inicialiar los servicios de MySQL y Apache.
2. Cargar el archivo odbcconfig.mat
3. Abrir Matlab y cargar la carpeta que contienen el algorimo (Matlab).
    
    Ir a la pestaña |APP| y buscar |data base explorer| seleccionar |conecct|
    
    En la ventana colocar el usuario: gah y password:123456 de la ase de datos y concetar.

4. Inicializar Ipl.m ubicado en la carpeta src. 
5. Abrir config.m ubicado en src y ejecutarlo, abrira una ventana donde se selccioanra add patch. 
6. Correr main_dsrm.m el archivo principal del algoritmo. 




                                 
