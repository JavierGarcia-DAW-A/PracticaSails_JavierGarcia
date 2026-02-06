# PracticaSails_JavierGarcia

## 1. Configuraciones Previas de la Máquina.

Creamos el repositorio de Github y lo clonamos mediante **git clone**.

Una vez hemos clonado el repositorio, entramos dentro de lo que sería el proyecto y hacemos un **vagrant init debian/bullseye64**, con esto se nos creará de manera automática el **Vagrantfile**, a mi me dieron muchísmos errores por el vagrantfile y no sabía como arreglarlos, así que recurrí a la IA y me dijo que el error era de los recursos de la máquina y me dejo el Vagrantfile tal que así:

![Vagrantfile](/capturas/1.png)

Con esa edición ya si podemos hacer el vagrant up y el vagrant ssh correspondientes.

![vagrantSsh](/capturas/2.png)

## 2. Instalar los paquetes necesarios

Una vez dentro de la máquina pasamos a instalar las dependencias necesarias para realizar este proyecto.

![paquetes](/capturas/3.png)

![composer](/capturas/4.png)

## 3. Creación y configuración del proyecto Laravel

Primeramente con composer creamos el proyecto con el nombre que nosotros queramos.

![install](/capturas/5.png)

Ahora editamos el proyecto, de primeras tendremos que copiar el .env.example a .env normal, para que coja la configuración de la base de datos.

![.env](/capturas/6.png)

## 4. Editar la base de datos

Ahora tendremos que crear la base de datos respectiva al proyecto y también vamos a crear un usuario específico para esta práctica.

![db](/capturas/7.png)

Ya creada la base de datos y todo lo respectivo a mysql, lanzamos las migraciones en nuestro proyecto.

![migracion](/capturas/8.png)

## 5. Comprobación

Una vez echo todo esto, nos tendría que salir en nuestro navegador de la máquina local la página principal de Laravel.

![comprobación](/capturas/9.png)




