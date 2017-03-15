# Practica 5: Sessions y Autenticación en ExpressJS

Ésta práctica consiste en realizar un servidor que utilice sesiones y autenticación para servir la website de un gitbook de ejemplo.
Para ello se han creado unas rutas básicas que administrarán los servicios.

* **/**
Ésta ruta inicial, nos mostrará las instrucciones de nuestro servidor, como también los enlaces a las diferentes rutas disponibles explicadas a continuación:

  * **/content**
  En esta ruta, se mostrará el gitbook solamente en el caso de que se haya logueado el usuario previamente, de otro modo saldrá un error.

  * **/login**
  En esta ruta nos saldrá un formulario en el que casa usuario introducirá su nombre de usuario y contraseña, dichos valores serán enviados en el cuerpo de la petición http (POST), los cuales se compararán con los datos de usuarios alojados en el fichero **users.json**, en el caso de que se encuentre entre ellos, se rellenará la sesión con el nombre y contraseña del usuario, de ésta forma se podrá acceder al gitbook tras pasar la barrera de autenticación de la función auth, que comprueba que el nombre y contraseña existan en la sesión.

  * **/register**
  En esta ruta, se servirá un formulario en el que se puede crear un nuevo usuario y añadirlo a nuestra base de datos **users.json**.

  * **/logout**
  Tras visitar esta ruta, se destruirá el objeto de session del cliente en el servidor, por lo que ya no tendría ninguna sesión activa para acceder a los recursos.








* [Enlace al repositorio Github](https://github.com/ULL-ESIT-DSI-1617/sessions-y-autenticacion-en-expressjs-alberto-diego-35l1)
* [Enlace a la publicación en máquina iaas Alberto](http://10.6.129.237:8088/)
* [Enlace a la publicación en máquina iaas Diego](http://10.6.128.78:8088/)
* [Enlace a la publicación en Heroku](https://fast-thicket-56276.herokuapp.com/)

* [Pagina web asignatura](https://campusvirtual.ull.es/1617/course/view.php?id=1136)
* [Enunciado de la practica](https://casianorodriguezleon.gitbooks.io/ull-esit-1617/content/practicas/practicasessions.html)

* [Página personal de Diego](https://alu0100761252.github.io)
* [Página personal de Alberto](https://alu0100825510.github.io)
