# instalacionPrestashop
<br>
<br>

![Imagen portada](/img/1.png)
En este breve documento van los pasos para instalar una tienda virtual en Prestashop alojado en los servicios de Amazon Web Service

<br>

# [Creación de instancia]()
![Primer paso instancia](/img/2.png)
![Segundo paso instancia](/img/3.png)
Ponemos nombre de la instancia o servidor
<br><br>

![Tercer paso instancia](/img/4.png)
Elegimos la maquina de Ubuntu para que sea más fácil su administración
<br><br>

![Cuarto paso instancia](/img/5.png)
Y la imagen de la maquina la dejamos en la que nos da por defecto
<br><br>

![Quinto paso instancia](/img/6.png)
Elejimos una llave para poder conectarnos por ssh
<br><br>

![Sexto paso instancia](/img/7.png)
![Septimo paso instancia](/img/8.png)
Los otros datos los dejamos por defecto y lanzamos la instancia
<br><br>

![Octavo paso instancia](/img/9.png)
![Noveno paso instancia](/img/10.png)
![Decimo paso instancia](/img/11.png)



# [Creación y asignación de IP elástica]()
![paso 1 IP elástica](/img/12.png)
![paso 2 IP elástica](/img/13.png)
Creamos la ip elástica con la configración por defecto para que me asigne una dirección IP aleatoria
<br><br>

![paso 3 IP elástica](/img/14.png)
![paso 4 IP elástica](/img/15.png)
Ahora asociamos la dirección ip con la instancia creada al principio
<br><br>
Ahora pasamos a la creación de grupo de entrada para poder conectarnos por internet
<br><br>

# [Creación de grupo de seguridad]()
![paso 1 grupo de seguridad](/img/16.png)
Editamos este grupo de seguriadad que se le asigno a la instancia
<br><br>

![paso 2 grupo de seguridad](/img/17.png)
Agregamos una nueva regla de entrada, elegimos que el tipo sea HTTP para poder conectarnos por interneyt y en destino elegimos Anywhere ipv4 para que todos se puedan conectar 
<br><br>

![paso 3 grupo de seguridad](/img/18.png)


# [Conectarse por SSH]()
Para conectarnos por ssh y poder hacer toda la administración de nuestra maquina debemos hacer los siguientes paso desde consola, en este caso use gitbash
<br><br>

![paso 1 ssh](/img/19.png)
![paso 2 ssh](/img/20.png)
Una vez hayamos entrado por ssh debemos instalar apache que nos permitira crear un servidor web, tambien debemos instalar php y mysql para las bases de datos y por último la conección entre php y mysql
<br><br>

![paso 3 ssh](/img/21.png)
Y por el momento ya podemos ver que nuestro servidor web esta funcionando
<br><br>

![paso 4 ssh](/img/22.png)
![paso 5 ssh](/img/23.png)

verificamos el estado para rectificar que este corriendo los servidores, librerias y paquetes que instalamos
<br><br>

# [Configuración de la base de datos]()
![paso 1 base de datos](/img/24.png)
entramos a la base de datos
<br><br>

![paso 2 base de datos](/img/25.png)
Hacemos la creación de la base de datos
<br><br>

![paso 3 base de datos](/img/26.png)
Creamos usuario en la base de datos
<br><br>

![paso 4 base de datos](/img/27.png)
Y le damos todos los privilegios de la base de datosa nuestro usuario para que la pueda administrar
<br><br>

![paso 4 base de datos](/img/28.png)

![paso 4 base de datos](/img/29.png)
Instalamos las siguientes librerias y dependencias de php
<br><br>

# [Instalación y descarga de Prestashop]()

Entrar a la carpeta raiz del servidor web
<br><br>


![paso 1 instalación y descarga Prestashop](/img/30.png)



![paso 1 instalación y descarga Prestashop](/img/31.png)
Descomprimimos la carpeta de prestashop
<br><br>

![paso 1 instalación y descarga Prestashop](/img/32.png)
Crear la carpeta para descomprimir e instalar Prestashop
<br><br>

![paso 1 instalación y descarga Prestashop](/img/33.png)
Mover la carpeta comprimida(pestashop.zip) a a que se creo anteriormente(Prestashop)
<br><br>

![paso 1 instalación y descarga Prestashop](/img/34.png)
Ahora descomprimir la carpeta(Prestashop.zip)
<br><br>