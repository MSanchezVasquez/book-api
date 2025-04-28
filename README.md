
¡Se me reseteó el entorno! 😅  
Pero tranqui, aquí te paso el **README.md** igual:

---

# 📚 API REST - Gestión de Libros

## Descripción
API RESTful para gestionar una colección de libros utilizando Spring Boot. Incluye validaciones y control de duplicados.

## Endpoints

### ➡️ Agregar Libro
- **Método:** POST
- **URL:** `/api/books`
- **Body (JSON):**
```json
{
  "title": "Título del libro",
  "author": "Autor del libro"
}
```
- **Respuestas:**
  - `201 Created`: Libro agregado correctamente.
  - `409 Conflict`: El libro ya existe.

### ➡️ Listar Todos los Libros
- **Método:** GET
- **URL:** `/api/books`
- **Respuestas:**
  - `200 OK`: Devuelve la lista de libros.

### ➡️ Obtener Libro por ID
- **Método:** GET
- **URL:** `/api/books/{id}`
- **Respuestas:**
  - `200 OK`: Devuelve el libro solicitado.
  - `400 Bad Request`: ID no encontrado o inválido.

## 📋 Manejo de Errores
- `409 Conflict`: Se intenta registrar un libro ya existente (mismo título y autor).
- `400 Bad Request`: Error de validación o ID no encontrado.

## 🛠 Tecnologías Usadas
- Java 17
- Spring Boot 3.x
- Spring Data JPA
- Base de datos en memoria H2

## 🧪 Pruebas
- Se realizaron pruebas usando Postman.
- Colección Postman incluida: `book-api-collection.json`

## 🚀 Cómo correr el proyecto
1. Clonar el repositorio.
2. Ejecutar `mvn spring-boot:run` en la terminal.
3. Acceder a `http://localhost:8080/api/books` para usar la API.

---

¿Quieres también que te arme una plantilla del **informe de trabajo grupal** que piden? 🚀 (división de tareas, retos, etc).
