# ForoHubApp

ForoHubApp es una aplicación web para la creación y gestión de foros de discusión. Desarrollada en Java con Spring Boot, esta aplicación permite a los usuarios registrarse, iniciar sesión y participar en diferentes temas de discusión. Este proyecto es parte de un desafío de Alura Latam para implementar una API REST con las funcionalidades básicas de un foro.

## Descripción


- Crear un nuevo tópico.
- Mostrar todos los tópicos creados.
- Mostrar un tópico específico.
- Actualizar un tópico.
- Eliminar un tópico.

Esto es lo que comúnmente conocemos como CRUD (CREATE, READ, UPDATE, DELETE).

## Funcionalidades

- API con rutas implementadas siguiendo las mejores prácticas del modelo REST.
- Validaciones realizadas según las reglas de negocio.
- Implementación de una base de datos relacional para la persistencia de la información.
- Servicio de autenticación/autorización para restringir el acceso a la información.

## Requisitos

- Java 11 o superior
- Maven 3.6.3 o superior
- MySQL 8.0 o superior
- IntelliJ IDEA

## Tecnologías utilizadas 

- Java
- Spring Boot
- Spring Security
- JWT 
- JPA 
- H2 Database 
- Postman 


## Estructura del proyecto 

- **Entities**: Clases de entidad que representan las tablas de la base de datos.
- **Dto**: Clases de Data Transfer Object utilizadas para transferir datos entre el cliente y el servidor.
- **Repository**: Interfaces que extienden JpaRepository para realizar operaciones CRUD en las entidades.
- **Service**: Clases de servicio que contienen la lógica de negocio.
- **Controller**: Clases de controlador que manejan las solicitudes HTTP.
- **Security**: Clases relacionadas con la configuración de seguridad y la autenticación.


## Configuración

1. **Base de datos MySQL**:

   Recuerda crea una base 


2. **EndPoints**:
- `/login`: Endpoint para autenticación de usuarios. Envía una solicitud POST con un JSON que contiene `username` y `password`.
- `/usuarios`: Endpoint para listar usuarios. Requiere autenticación mediante un token JWT.
- `/topicos`: Endpoint para manejar la creación, actualización y eliminación de tópicos.


  