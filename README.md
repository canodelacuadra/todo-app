# Proyecto: Lista de Tareas (React + Express + MongoDB)

## Requisitos
- Node.js
- MongoDB Atlas
- Netlify (frontend)
- Render (backend)

---

## Instalación

### Backend
1. Copia `.env.example` a `.env` y añade tu cadena de conexión MongoDB:
   ```
   MONGO_URI=mongodb+srv://<usuario>:<password>@<cluster>.mongodb.net/tareas
   PORT=3000
   ```
2. Instala dependencias:
   ```bash
   cd backend
   npm install
   ```

3. Ejecuta el servidor local:
   ```bash
   npm start
   ```

4. Despliegue en Render:
   - Crea un nuevo servicio web.
   - Añade las variables de entorno: `MONGO_URI`, `PORT`.
   - Usa `npm start` como comando.

---

### Frontend
1. Copia `.env.example` a `.env` y ajusta la URL del backend (Render):
   ```
   VITE_API_URL=https://<tu-api-backend>.onrender.com/api/tareas
   ```

2. Instala dependencias:
   ```bash
   cd frontend
   npm install
   ```

3. Ejecuta localmente:
   ```bash
   npm run dev
   ```

4. Despliegue en Netlify:
   - Importa proyecto desde GitHub.
   - En "Build command": `npm run build`
   - En "Publish directory": `dist`
   - Añade variable de entorno: `VITE_API_URL`

---

## Resultado esperado
Una app funcional con:
- Formulario para añadir tareas.
- Lista con tareas (editar, eliminar, marcar como completadas).
- Backend en Render.
- Frontend en Netlify.
