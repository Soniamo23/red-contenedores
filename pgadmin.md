# Practica servidor web
## 1. Titulo
Implementación de un Servidor Web con Docker utilizando Nginx y PostgreSQL
## 2. Tiempo de duración
Esta practica se realizo en un aproximado de 40 minutos 
## 3. Fundamentos:

La práctica de configurar un servidor de bases de datos utilizando Docker con PostgreSQL y pgAdmin es importante ya que se puede aprender la gestion de base de datos. 
- Docker es una herramienta que permite empaquetar aplicaciones en contenedores, facilitando su implementación, portabilidad y escalabilidad en diferentes entornos de desarrollo.
- PostgreSQL es un sistema de gestión de bases de datos relacional y objeto, conocido por su robustez, extensibilidad y cumplimiento de estándares SQL. 
- pgAdmin es una herramienta de administración y desarrollo para PostgreSQL que proporciona una interfaz gráfica para gestionar bases de datos. 


## 4. Conocimientos previos.
   
Para realizar esta practica el estudiante necesita tener claro los siguientes temas:
- Comandos basicos de docker
- Manejo de comandos
- Manejo de base de datos

## 5. Objetivos a alcanzar
   
- Implementar contenedores con PostgreSQL y pgAdmin.
- Configurar la comunicación entre contenedores utilizando una red Docker personalizada.
- Aprender a gestionar bases de datos mediante la interfaz gráfica de pgAdmin.
## 6. Equipo necesario:
  
- Computador con sistema operativo Windows/Linux/Mac.
- Instalación local de Docker.
- Acceso a internet.

## 7. Material de apoyo.
   
- Guia de asignatura asignada por docente.
- Video tutorial de docente
- Documento oficial sobre docker.
  
## 8. Procedimiento

Primer paso: Aqui entramos a la aplicacion de docker, en la terminal creamos y ejecutamos un contenedor de docker:docker run -d --name dbpsql -e POSTGRES_PASSWORD=admin  -p 5432:5432 postgres


Figura 1-1. Contener de docker
<img src="./image/Crear contenedor .png" alt="contenedor" width="800px">

Segundo paso: Le damos un correo y una contraseña, el correo puede ser el que sea puse el intitucional y la contraseña es admin, esto es para poder entrar en la pagina de pgAdmin

Figura 1-2. Creacion de usuario
<img src="./image/Creacion de usuario.png" alt="usuario" width="800px">

Tercer paso: Creamos para poder abrir ya en el localhost y se va a llamar redinterna, y conectar el dbpsql y pgadmin

Figura 1-3. Coneccion de red
<img src="./image/Crear red.png" alt="red" width="800px">

Cuarto paso: Tnemos que poner en el navegador el localhost:8090, que ese es el puerto que colocamos y asi poder abrir nuestro pgadmin donde se podra colocar el correo y contraseña que ya cremao anteriormente

Figura 1-4. Login
<img src="./image/Login a pgAdmin.png" alt="login" width="800px">

Quinto paso: Una vez entrado vamos a creacr un servidor qe se va a llamar servidor-db

Figura 1-5. Servidor
<img src="./image/Nombre al servidor.png" alt="servidor" width="800px">

Sexto paso: Dentro del servidor que cfreamos se va a crear una base de datos la cual llamaremos app web 

Figura 1-6. Creacion de usuario
<img src="./image/Creacion de app web.png" alt="usuario" width="800px">

Septimo paso: Por ultimo para hacer la verificación vamos a crear una tabla en app web y dentro de el archivo de Schemas y dentro de tablas podemos crear y asi verificamos que la coneccion fue exitosa.

Figura 1-7. Creacion de tabla
<img src="./image/Verificacion de coneccion.png" alt="tabla" width="800px">

## 9. Resultados esperados:
    
Como podemos observar que los contenedores funcionan correctamente, ya que el acceso a pgadmin esta disponible, se puede iniciar sesión. Ademas pgadmin permite gestionar la base de datos de postgresql. 

## 10. Bibliografía
    
- Docker, Inc. (2023). Docker Documentation. Recuperado de https://docs.docker.com/
- Otro Profe Marco. (2024, 27 abril). Postgresql y pgAdmin con docker [Vídeo]. YouTube. https://www.youtube.com/watch?v=F_aL2Aw5wcE
