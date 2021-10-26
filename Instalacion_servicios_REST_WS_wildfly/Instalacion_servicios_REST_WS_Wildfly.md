# Instalación de servicios REST/WS Wildfly

## 1. Introducción.
En esta practica vamos a desplegar dos aplicaciones en WildFly. La primera es una aplicación con simple Hello World usando JAX-RS (Java API for RESTful Web Service) y la segunda una demostración de Hello World usando JAX-WS Web Service.

Para poder realizar la siguiente practica se entiende que tendremos que tener instalado Java (JDK pertinente) + MAVEN ademas de WildFly instalado y configurado como consola de administración.



## 2. Servicio helloworld-rs.
Primero vamos a desplegar la aplicaciones RESTful, para ello vamos a descargarnos el proyecto en la siguiente página: WildFly quickstart.
Una vez descargado vamos a acceder al proyecto y lanzar “mvn clean install” para limpiar y generar el WAR de nuestra app.

![03-mvn-clean-install-rs](capturas/03-mvn-clean-install-rs.png)


Ahora que tenemos el WAR vamos a acceder a la consola de administración de WildFly con “ip_servidor:puerto/console” y ponemos el usuario y contraseña con permisos de administración de WildFly.

Ya dentro seleccionamos “start” en Deployments.

![04-deployments](capturas/04-deployments.png)


Ya en deployment apretamos en el +.

![05-add](capturas/05-add.png)


Ya aquí añadimos el .war .

![06-add](capturas/06-add.png)

![07-add](capturas/07-add.png)


Le damos a continuar y vemos como podemos cambiar el nombre o el nombre de ejecución. Al terminar de cambiarlos o dejarlos como están le damos a “Finish”

![09-specify-names](capturas/09-specify-names.png)


Y veremos algo como lo siguiente.

![08-terminado](capturas/08-terminado.png)


Cerramos y podremos ver los atributos del proyecto que hemos delegado.

![10-atributos](capturas/10-atributos.png)


Y si accedemos al root del proyecto lo veremos desplegado.

![11-pagina](capturas/11-pagina.png)



## 3. Servicio helloworld-ws.
Segundo vamos a desplegar la aplicaciones JAX-WS , para ello vamos a descargarnos el proyecto en la página pagina: WildFly quickstart.
Una vez descargado vamos a acceder al proyecto y lanzar “mvn clean install” para limpiar y generar el WAR de nuestra app.

![02-mvn-clean-install-ws](capturas/02-mvn-clean-install-ws.png)


Ahora que tenemos el WAR vamos a acceder a la consola de administración de WildFly con “ip_servidor:puerto/console” como hemos echo ya  Y en deployment apretamos en el + y lo añadimos.

![12-subida-war-ws](capturas/12-subida-war-ws.png)


Ventana donde podemos especificar los nombres de la aplicación.

![13-name-ws](capturas/13-name-ws.png)


Veremos algo como lo siguiente.

![14-terminado-ws](capturas/14-terminado-ws.png)


Cerramos y podremos ver los atributos del proyecto que hemos delegado.

![15-atributter-ws](capturas/15-atributter-ws.png)


Y si accedemos al root del proyecto lo veremos desplegado.

![16-pagina](capturas/16-pagina.png)
