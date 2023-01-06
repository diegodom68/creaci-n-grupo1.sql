# Proyecto MySQL
### Indice
1. Instalación
2. Diseño
3. Conexión
4. Conclusiones

## 1.Instalación
Para comenzar con el proyecto debemos instalar MySQL y configurarlo con DataGrip. Para la 
instación iremos a la pagina de MySQL, donde descargaremos un archivo msi que es un instalador 
por pasos y nos lo instalará automaticamente. También configuraremos el usuario root al que 
tendremos que poner contraseña (123456). Una vez seguido los pasos de la instalación tendremos
una interfaz como esta:
![](../Capturas%20MD/1.png)
Y como podemos observar aparece una conexión de servidor que ya tendremos hecha. Una vez
creada esa conexión tendremos que crear un usuario para hacer la conexion y poder hacer las 
tablas con ese usuario. Tendremos una columna de opciones y tendremos que entrar en la que dice
users and privileges.

![](../Capturas%20MD/2.png)

![](../Capturas%20MD/3.png)

Como  vemos en las capturas seria añadir el usuario y poner el nombre y contraseña que queramos,
eso si nos pedira que sea una contraseña de minimo 8 caracteres y que sea de bastante dificultad.
(En nuestro caso Diego12345@).

Una vez finalizada la instalación de MySQL habra que conectarlo con DataGrip para poder trabajar
desde allí. Pero eso se explicará más adelante en el apartado **_Conexión_**.

## 2.DISEÑO
Nuestro base de datos a realizar es sobre la DIAMOND LEAGUE de atletismo. Hemos 
creido oprtuno hacer 7 tablas para optimizar y recoger los datos de esta liga. Adjunto foto:
![](../Capturas%20MD/Whats.jpg)
Como podemos ver hemos hecho una tabla paises para diferenciar tento el origen de los 
corredores tanto las sedes de las carreras. Tambien una tabla competiciones para saber los 
tipos de competiciones que hay y que se van a guardar.
La tablas paises y sexos estaran referenciadas en la tabla competiciones y la tabla corredores, y las tablas competiciones 
y corredores estaran referenciadas en las tablas del ranking, que habrá dos tablas de ranking 
una de hombres y otra de mujeres, ya que las competiciones no son mixtas.

## 3.CONEXIÓN
Nosotros para poder conectarnos nos a tocado iniciar sesion en git hub a todos y que uno crease el "grupo" y los demás
se uniesen allí de manera que todo el mundo viera lo que a subido todo el mundo, es decir, cada uno podia subir lo que quisiese
pero teniendo en cuenta que tambien lo iban a ver los demas participantes de ese grupo. Y esa parte es la conexion a traves de 
GitHub que es la mas sencilla. Ahora toca conectarse a DataGrip que a sido un poco mas complejo. Una vez dentro de  Datagrip debemos conectarnos con MariaDB o MySQL
en el cual debemos introducir un usuario y contraseña, que previamente hemos configurado en nuestro MySQL. 
![](../Capturas%20MD/4.png)
 Y antes de aplicar podemos hacer un test conection para asegurarnos de que tenemos conexión con la base de datos.

## 4.Conclusión.
La configuración de una base de datos MySQL es un proceso importante para establecer la estructura y organización de los datos almacenados en un sistema. 
Es necesario definir el esquema de la base de datos, incluyendo la creación de tablas y la definición de campos y tipos de datos. También es importante establecer 
los usuarios y sus permisos, para controlar quién puede acceder y realizar operaciones en la base de datos. Es esencial realizar pruebas y verificaciones para asegurarse de que
la configuración esté correcta y de que la base de datos funcione de manera eficiente y segura. En general, configurar una base de datos MySQL requiere una comprensión profunda de
cómo funcionan las bases de datos y cómo se utilizan en un sistema determinado. 

