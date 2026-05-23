🔧 Backend – FinanControl

Este repositorio contiene la implementación del backend del sistema en dos tecnologías distintas:

🟢 Rama node-version → Implementación con Node.js
🔵 Rama php-version → Implementación con PHP

Cada rama contiene su propia estructura y configuración independiente.

👥 Integrantes

Nicolás David García Nieto-1202736 Paula Valentina Pirajón Flórez-1202745 Laura Sofia Vargas Morales-1202815

🎯 Objetivo del Backend

Implementar un servidor capaz de:

Gestionar solicitudes HTTP.
Procesar datos enviados por el cliente.
Conectarse a una base de datos.
Implementar operaciones CRUD.
Retornar respuestas en formato JSON.


Estructura del proyecto

🌿 Estructura de Ramas
🟢 Rama: node-version

Backend desarrollado con Node.js sin frameworks.

Ejecución Local
npm install
npm start

Servidor:
http://localhost:3000

Despliegue
Compatible con:
Render
Railway
VPS Node

Debe usar:
const PORT = process.env.PORT || 3000;

🔵 Rama: php-version

Backend desarrollado con PHP utilizando estructura modular básica.

Ejecución Local

Si usan servidor embebido de PHP:

php -S localhost:8000

Servidor:
http://localhost:8000

Despliegue

Compatible con:

Render (servicio PHP)
InfinityFree
Hostinger
XAMPP (local)

📡 Endpoints Implementados
Método	Ruta	Descripción
GET	/api/users	Obtener usuarios
POST	/api/users	Crear usuario
PUT	/api/users/{id}	Actualizar usuario
DELETE	/api/users/{id}	Eliminar usuario
🗄️ Base de Datos

Supabase

Ubicación del script:

/database/script.sql


🔐 Validaciones Implementadas

Campos obligatorios
Validación de formato email
Manejo de errores HTTP
Respuestas en formato JSON

🌍 URLs en Producción

Node:

https://nombre-app-node.onrender.com


PHP:

https://nombre-app-php.onrender.com
