# Moodle_Docker
Desplegar un Sistema LMS Moodle usando Docker en una computadora Mac Pro 2019 

Antes de empezar la imstalaciom vamos a contestar las siguientes preguntas:

1.- ¿Qué modelo de Mac? <br>
    Es una Mac Pro 2019<br>
3.- ¿Qué procesador tiene?<br>
    Un intel Xeon W<br>
4.- ¿Cuántos núcleos tiene?<br>
     8 nucleos a 3.5Ghz<br>
5.- ¿Cuántos hilos de ejecución tiene?<br>
    56 hilos<br>
6.- ¿Qué tarjeta(s) de video tiene?<br>
    Tiene dos tarjetas AMD Radeon PRO W5500X de 8 GB<br>
    
![image](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/46a6ddf8-eea3-4d24-a4da-95ac7fe6bb89)


<h1> Despliege del sistema</h1>


Para empezar con la instalacion, debemos de habera ya instalado Git y Docker en nuestra Mac, una vez teniendo esto abriremos uns linea de comandos donde clonaremos este mismo repositorio que contiene el docker-compose.yml que es el que nos ayudara con la instalacion, para eso usaremos el siguiente comando: $ Git clone https://github.com/AaronSol28/Moodle_Docker.git


![2](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/a344a1c1-8bfd-413c-ba33-c6d35c3325a6)

Una vez tengamos el repositorio clonado, lo que haremos es ir a la ruta donde se guardo el contenido del repositorio, para esto usaremos el siguiente comando: $ Cd Moodle_docker


![3](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/7e1c1e14-13e3-4e1e-9d6c-cd619043c9dd)

Lo siguiente sera verificar el archivo Docker-compose.yml para ver que el contenido sea correcto con el siguiente comando: $ cat docker-compose.yml

![4](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/b31c9478-4259-4f3c-ae1d-08a2f5652196)

Ahora, para poder descargar y montar la imagen y el contenedor de moodle en nuestra Mac, debemos de correr el siguiente comando: $ docker-compose -f docker-compose.yml up -d, ahora esperaremos a que se descarguen e instale el contenedor con las imagenes necesarias.

![5](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/e2966aff-e165-4d2b-9feb-bd3a85933c2b)

Ya terminado el proceso de instalacion, usaremos el comando: $ docker ps, para ver lo que esta corriendo y los puertos en donde vamos a acceder a ellos.

![6](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/cc322382-0ef9-41c0-bc14-07b530d8e236)


En nuestro caso el servicio esta corriendo en el puerto 8080 de nuestra maquina, para visualizar moodle corriendo nos iremos a nuestro navegador safari y pondremos en el buscador lo siguiente:
http://localhost:8080

![7](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/a7ebc7e7-48a7-4eac-abfd-ec959daff3e7)

Con esto habremos acabado con la instalacion de un Sistema LMS Moodle usando Docker en una computadora Mac Pro 2019 satisfactoriamente.

Conclusiones:
En esta actividad pude experimentar un caso muy cercano a la realidad en cuanto al tipo de tareas que se me asignarian en un trabajo de DevOps, usando un equipo de alta gama y con la potencia necesaria para correr el sistema, asi como tambien los comandos y herramientas dentro del SO para implementar el mismo. Me deja una experiencia para las tareas que se me posrian asignar en un trabajo.
