# Moodle_Docker
Desplegar un Sistema LMS Moodle usando Docker en una computadora Mac Pro 2019 

Antes de empezar la imstalaciom vamos a contestar las siguientes preguntas:

1.- ¿Qué modelo de Mac?
    Es una Mac Pro 2019
2.-¿Cuánta memoria RAM tiene?
    Tiene instalados 96GB de memoria RAM
3.- ¿Qué procesador tiene?
    Un intel Xeon W
4.- ¿Cuántos núcleos tiene?
     8 nucleos a 3.5Ghz
5.- ¿Cuántos hilos de ejecución tiene?
    56 hilos
6.- ¿Qué tarjeta(s) de video tiene?
    Tiene dos tarjetas AMD Radeon PRO W5500X de 8 GB
    
![image](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/46a6ddf8-eea3-4d24-a4da-95ac7fe6bb89)


Para empezar con la instalacion, debemos de habera ya instalado Git y Docker en nuestra Mac, una vez teniendo esto abriremos uns linea de comandos donde clonaremos este mismo repositorio que contiene el docker-compose.yml que es el que nos ayudara con la instalacion, para eso usaremos el siguiente comando: $ Git clone https://github.com/AaronSol28/Moodle_Docker.git


![2](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/a344a1c1-8bfd-413c-ba33-c6d35c3325a6)

Una vez tengamos el repositorio clonado, lo que haremos es ir a la ruta donde se guardo el contenido del repositorio, para esto usaremos el siguiente comando: $ Cd Moodle_docker


![3](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/7e1c1e14-13e3-4e1e-9d6c-cd619043c9dd)

Lo siguiente sera verificar el archivo Docker-compose.yml para ver que el contenido sea correcto con el siguiente comando: $ cat docker-compose.yml

![4](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/b31c9478-4259-4f3c-ae1d-08a2f5652196)

Ahora, para poder descargar y montar la imagen y el contenedor de moodle en nuestra Mac, debemos de correr el siguiente comando: $ docker-compose -f docker-compose.yml up -d, ahora esperaremos a que se descarguen e instale el contenedor con las imagenes necesarias.

![5](https://github.com/AaronSol28/Moodle_Docker/assets/105986750/e2966aff-e165-4d2b-9feb-bd3a85933c2b)


