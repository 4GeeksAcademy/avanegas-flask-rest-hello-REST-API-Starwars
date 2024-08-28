# Build a StarWars REST API
Este proyecto consiste en desarrollar una API REST que administra un blog de StarWars, donde los usuarios pueden listar personajes y planetas, así como agregar o eliminar favoritos. La API está diseñada siguiendo principios RESTful y está conectada a una base de datos, lo que permite manejar datos dinámicos como personajes, planetas y usuarios.

## Tecnologías Utilizadas
- **Backend:** Python (Flask) o Node.js (Express)
- **ORM:** SQLAlchemy para la interacción con la base de datos
- **Base de Datos:** PostgreSQL
- **Herramientas de Desarrollo:** Gitpod o Codespaces para un entorno de desarrollo instantáneo
- **Pruebas de API:** Postman

## Características del Proyecto
Endpoints Implementados

### Personajes (People)

- [GET] /people - Listar todos los personajes.
- [GET] /people/<int:people_id> - Obtener información de un personaje específico.

### Planetas (Planets)

- [GET] /planets - Listar todos los planetas.
- [GET] /planets/<int:planet_id> - Obtener información de un planeta específico.

### Usuarios (Users)

- [GET] /users - Listar todos los usuarios registrados.
- [GET] /users/favorites - Listar todos los favoritos del usuario actual.

### Favoritos (Favorites)

- [POST] /favorite/planet/<int:planet_id> - Añadir un planeta a favoritos del usuario.
- [POST] /favorite/people/<int:people_id> - Añadir un personaje a favoritos del usuario.
- [DELETE] /favorite/planet/<int:planet_id> - Eliminar un planeta de favoritos.
- [DELETE] /favorite/people/<int:people_id> - Eliminar un personaje de favoritos.

## Funcionalidades Adicionales

- Modelado de base de datos utilizando SQLAlchemy o TypeORM.
- Sistema de migraciones de base de datos con Alembic (Flask) o migraciones nativas de TypeORM (Express).
- Soporte para CRUD completo para los modelos de datos, permitiendo la administración completa del contenido a través de la API.

## Pruebas y Validación
Se utilizan herramientas como Postman para probar y validar todos los endpoints de la API, asegurando que cada operación cumpla con las especificaciones y el manejo adecuado de errores.

## Mejora Continua
Se recomienda extender el proyecto agregando endpoints adicionales para crear, modificar y eliminar personajes y planetas, proporcionando una gestión completa de la base de datos a través de la API.

## Cómo Comenzar
Utiliza el boilerplate para Flask REST o Express.js REST como punto de partida.
Configura la base de datos localmente o utiliza un entorno de desarrollo como Gitpod.
