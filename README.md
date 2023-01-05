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

