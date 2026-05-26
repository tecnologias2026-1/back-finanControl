🔧 Backend – FinanControl

Este repositorio contiene la implementación del backend del sistema en dos tecnologías distintas:


👥 Integrantes

Nicolás David García Nieto-1202736 Paula Valentina Pirajón Flórez-1202745 Laura Sofia Vargas Morales-1202815

🎯 Objetivo del Backend

Implementar un servidor backend para FinanControl capaz de:

Gestionar solicitudes HTTP mediante una API REST.
Procesar datos enviados desde el frontend.
Conectarse a una base de datos externa en Supabase.
Implementar operaciones CRUD para usuarios, metas y transacciones.
Retornar respuestas en formato JSON.
Manejar autenticación de usuarios mediante login y registro.
Permitir despliegue en servicios cloud como Render.

🧩 Tecnologías Utilizadas
Frontend
HTML5
CSS3
JavaScript
AJAX / Fetch API
Live Server (desarrollo local)
Backend
Node.js
Express.js
dotenv
cors
nodemon
Base de Datos
Supabase (PostgreSQL)

Estructura del proyecto

FinanControl/
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── routes/
│   ├── package.json
│   ├── server.js
│   └── .env
│
├── Dashboard.html
├── metas.html
├── iniciar.js
├── metas.js
├── registrarse.js
├── supabase.js
├── estilos.css
│
└── .gitignore

🌿 Estructura de Ramas
🟢 Rama: node-version

Backend desarrollado con Node.js y Express.js.

Ejecución Local
Instalar dependencias:
npm install
Ejecutar servidor:
npm run dev
npm start

Servidor local:

http://localhost:3000

Servidor:
http://localhost:3000

Despliegue
Backend preparado para desplegarse en:
Render
Railway
VPS Node.js

Debe usar:
const PORT = process.env.PORT || 3000;



📡 Endpoints Implementados
1.🔑 Autenticación
<img width="655" height="115" alt="image" src="https://github.com/user-attachments/assets/f89d6589-cadc-4af7-809e-eefa8cb7410c" />
2.🎯 Metas
<img width="689" height="209" alt="image" src="https://github.com/user-attachments/assets/76874ce6-326b-42ef-868d-28d4c1112749" />
3.💸 Transacciones
<img width="678" height="199" alt="image" src="https://github.com/user-attachments/assets/5c604aca-5089-452c-8478-b67f979706aa" />


🗄️ Base de Datos

La aplicación utiliza:

Supabase
PostgreSQL

Conexión realizada mediante:

createClient(
   process.env.SUPABASE_URL,
   process.env.SUPABASE_KEY
)

https://financontrol-backend.onrender.com

🔐 Validaciones Implementadas

- Campos obligatorios
- Validación de formato de correo electrónico
- Validación de longitud mínima de contraseña
- Verificación de usuarios existentes
- Manejo de errores HTTP
- Respuestas estructuradas en formato JSON
- Encriptación de contraseñas con bcrypt
- Validación de sesión mediante localStorage
