📚 MongoDB CRUD Application
¡Bienvenido a MongoDB CRUD Application! 🎉 Este proyecto es una API RESTful desarrollada en Spring Boot que utiliza MongoDB como base de datos. Permite realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre una colección de tutoriales. Es ideal para aprender sobre la integración entre Spring Boot y MongoDB.

🚀 Comenzando
🛠️ Requisitos previos
Antes de correr la aplicación, asegúrate de tener lo siguiente instalado en tu máquina:

☕ Java 11+
🐘 Maven 3+
🍃 MongoDB (corriendo en mongodb://localhost:27017)
Un editor de código como 💡 IntelliJ IDEA o 🖥️ VS Code
⚙️ Instalación
Clonar el repositorio Abre tu terminal y ejecuta:
git clone https://github.com/anthonydavila/mongodb-crud.git

📂 Navegar al directorio del proyecto
cd mongodb-crud

🔗 Configurar la conexión a MongoDB Asegúrate de que MongoDB esté ejecutándose localmente en mongodb://localhost:27017. Si es necesario, modifica la configuración en el archivo application.properties ubicado en src/main/resources/.
spring.data.mongodb.uri=mongodb://localhost:27017/mongodbcrud
spring.application.name=Spring Boot MongoDB CRUD
spring.data.mongodb.username=admin
spring.data.mongodb.password=horus

🛠️ Construir el proyecto Ejecuta el siguiente comando para construir el proyecto con Maven:
mvn clean install

▶️ Ejecutar la aplicación Ejecuta el siguiente comando para iniciar la aplicación:
mvn spring-boot:run

La API estará corriendo en: http://localhost:8080. 🌐
📋 Uso de la API
A continuación, te presentamos los principales endpoints disponibles en esta API:

Tabla

Método	Endpoint	Descripción
GET	/api/tutorials	Obtener todos los tutoriales o buscar por título
GET	/api/tutorials/{id}	Obtener un tutorial por su ID
POST	/api/tutorials	Crear un nuevo tutorial
PUT	/api/tutorials/{id}	Actualizar un tutorial por su ID
DELETE	/api/tutorials/{id}	Eliminar un tutorial por su ID
DELETE	/api/tutorials	Eliminar todos los tutoriales
📥 Crear un Tutorial
Para crear un nuevo tutorial, envía una petición POST al endpoint /api/tutorials con el siguiente cuerpo en formato JSON:

JSON

{
  "title": "Aprendiendo Spring Boot",
  "description": "Guía completa para Spring Boot",
  "published": true
}
Código generado por IA. Revisar y usar cuidadosamente. Más información sobre preguntas frecuentes.
🔍 Obtener todos los Tutoriales
Envía una petición GET a /api/tutorials para obtener todos los tutoriales. Si quieres buscar por título, usa un query param:

GET /api/tutorials?title=Spring

¡Gracias por usar MongoDB CRUD Application! 🎉 Si tienes alguna duda, no dudes en consultar la documentación oficial de Spring Boot. 📚
