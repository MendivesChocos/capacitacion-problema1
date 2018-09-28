# Ejercicio 1
Capacitación: Git, bash y docker
Integrantes:
- christiam mendives    
- Walter Rafael
- El sol de aptitus

# PREGUNTAS

1. ¿Qué es y para qué sirve GIT?
Es un sistema para el control de cambios, y sirve para poder trabjar de forma mas ordenada en equipo
2. ¿Que es Github o bitbucket?
son almacenadores de repositorios
3. ¿Qué es y para qué sirve el SSH?
Es un protocolo que sirve para adminstrar de manera remota, sirve para trabajar de manera segura, para la autenticacion de usuarios de manera remota
4. ¿Que pasa si cambio de PC? ¿Tendré que generar el SSH nuevamente?¿Por qué?
Tendria que instalar todo desde cero, si porque tendria autenticarme en mi nueva pc
5. ¿Qué es markdown? ¿Para qué sirve?
Es un lenguaje de marcacion ligera, es para crear archivos guia
6. ¿Cómo inicializo y configuro un proyecto de git?
git init
git clone 
git config 

# Preguntas Docker

1. ¿Qué importancia tiene los tags en un proyecto?
Es importante taggear un poryecto, primero para tener un buen historial de versiones, segundo 
para que podamos detectar de manera rapida una version especifica de esta manera corregir algun error espeficico de esa version 
o volver a una version estable
2. ¿Cuál es la diferencia entre un tag normal y un tag anotado en git?
El tag anotado nos permite especificar un mensaje personalizado, y el ligero no me permite un mensajes y es mas usado en desarrollo
3. ¿Cómo se sube todos los tags de git que hay en mi local?
Se sube utilizando el git push origin --tags

4. ¿Es necesario loguearse cada vez que subo una imagen a dockerhub?
Si es necesario, sino no nos permitiria subir nuestra imagen

5. ¿Qué es y para qué sirve docker?
Docker es una plataforma opensource para desarrolladores y administradores de sistemas que nos permite crear, enviar y correr aplicaciones distribuidas dentro de laptops, VM's o cloud.

6. ¿Cuál es la diferencia entre docker y VirtualBox?
El virtualBox me permite virtualizacion a nivel de hardware y docker a nivel de sistema operativo

7. ¿Es necesario depender de una imagen de docker base al crear una imagen nueva?
si es necesario ya que la vitualizacion es a nivel de sistema operativo

8. ¿Porqué debo anteponer el nombre de usuario en una imagen docker nueva?
Para indicar que tu eres el autor, el usuario de la imagen y quien da mantenimiento a esta

9. ¿Que pasa si creo una imagen sin especificar una versión o tag, con qué versión se crea?
En este caso se agrega la version por default el tag latest.

10. ¿Porqué es necesario crear un contenedor con esta bandera -it ? ¿Qué pasa si no le pongo -it?
Ya que con esta forma el proceso bash esta activo, al ser mostardo de forma grafica. El contenedor ejecuta el proceso bash y al no detectar un error sobre el proceso, el contenedor termina su ejecucion.

11. ¿Para qué sirve ejecutar el comando bash al eejcutar una imagen?
Para interpretar las ordenes que voy ejecutar a mi container

12. ¿Cuál es la diferencia entre docker ps y docker ps -a?
El docker ps lista todos los contenedores que se estan ejecutando, y el docker ps -a lista todos los contenedores

# Paso 5

1. ¿Cuál es la diferencia entre una imagen y un contenedor?
la imagen es un archivo comprimido de multiples capas, y el contenedor es una instancia de una imagen

2. ¿Cómo listo las imágenes que hay en mi computadora?
se listan con el comando docker ps -a

3. ¿Cómo salgo de un contenedor de docker?
salimos con el comando exit, que nos permite detener el contenedor

4. ¿Se elimina el contenedor al salir de ella?
No se elimina, termina su ejecucion, pero permanece en un esatado exit.

5. ¿Cómo elimino un contenedor?
Se elimina con docker rm "id_container"

6. ¿Para qué es necesario el flag `-i`, `-t`, `--rm`?
El comando -i el para el modo interactivo, el -t permite la visualizacion de texto en el terminal, --rm sirve para eliminar un contenedor
luego de que este alla ejecutado sus procesos

7. ¿Cómo verifico que el archivo creado se encuentra en la imagen?
Ingresando al contendor a traves del bash

8. ¿Cómo se comenta una linea de código en Dockerfile?
Se comenta con el #