# Práctica del curso de DevOps

Cada alumno deberá desplegar en un servidor su desarrollo para la práctica del curso de Programación Backend con Node.

El alumno podrá elegir la plataforma de hosting donde desplegar dicha práctica (Azure, AWS, etc.).

La entrega de la práctica será a través del formulario de entrega de prácticas, en el que se deberá
indicar la URL del repositorio donde tienen el código de la solución de la práctica del curso de Programación Backend con Node. Dentro de este repositorio deberá existir un archivo README.md en el cual deberán indicar la URL donde está desplegada la práctica para que pueda ser evaluada.

---

**Quedaría montado de la siguiente manera:**

- Práctica React - MegaANUNCIOS:
    <br />
    [http://35.181.61.77/](http://35.181.61.77/)
    ```shell
	UserName: usu1
	Password: pas1
    ```
    <br />
- Práctica Node - NodePOP:
    <br />
    [http://ec2-35-181-61-77.eu-west-3.compute.amazonaws.com/](http://ec2-35-181-61-77.eu-west-3.compute.amazonaws.com/)
	
   
    ```shell
    Ejemplo con filtrado:

    http://ec2-35-181-61-77.eu-west-3.compute.amazonaws.com/?skip=0&limit=5&sort=name&price=1-5000&tags=lifestyle
    ```
	
	
---

<br />

## Ejercicio 1

La arquitectura deseada para la puesta en producción es la siguiente:

• Utilizar node como servidor de aplicación utilizando PM2 como gestor de procesos node para que siempre esté en ejecución. La aplicación node deberá reiniciarse automáticamente al arrancar el servidor (en el startup).

• Utilizar nginx como proxy inverso que se encargue de recibir las peticiones HTTP y derivárselas a node.

• Los archivos estáticos de la aplicación (imágenes, css, etc.) deberán ser servidos por nginx (no por node). Para poder diferenciar quién sirve estos estáticos, se deberá añadir una cabecera HTTP cuando se sirvan estáticos cuyo valor sea: X-Owner (la X- indica que es una cabecera personalizada) y el valor de la cabecera deberá ser el nombre de la cuenta de usuario en github o bitbucket del alumno. Si la solución de la práctica por parte del alumno no tuviera archivos estáticos, deberá proporcionar el acceso a un archivo estático que se sirva a través de nginx (por ejemplo a través de la URL <dominio>/public/logo.jpg). En este caso, el alumno deberá indicar la URL del archivo estático en el archivo README.md del repositorio.

Ejercicio 1:
<br />
[http://ec2-35-181-61-77.eu-west-3.compute.amazonaws.com/](http://ec2-35-181-61-77.eu-west-3.compute.amazonaws.com/)

<br />

## Ejercicio 2

Si se accede al servidor web indicando la dirección IP del servidor en lugar del nombre de dominio, se deberá carga la práctica realizada en el módulo de React o React Avanzado (a elección del almuno).

Ejercicio 2:
<br />
[http://35.181.61.77/](http://35.181.61.77/)

```shell
Login:

    UserName: usu1
    Password: pas1
```
