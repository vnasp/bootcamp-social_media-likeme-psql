# LikeMe - Red Social (PostgreSQL)

Aplicación full-stack de red social donde los usuarios pueden compartir sketches, ver un feed y dar likes. Frontend en React conectado a un backend Node.js/Express con PostgreSQL.

> Nota: Este es un proyecto académico desarrollado durante el Bootcamp Full Stack JavaScript de Desafío LATAM.

## Funcionalidades

- Crear posts con título, URL de imagen y descripción
- Ver feed de posts con contador de likes
- Dar likes a posts
- Eliminar posts
- API RESTful con arquitectura MVC

## Tecnologías

**Cliente**

- React 18
- Vite
- Material UI (MUI)
- Axios

**Servidor**

- Node.js / Express
- PostgreSQL (pg)
- CORS / dotenv

## Estructura del Proyecto

```
client/
├── src/
│   ├── components/
│   │   ├── CardSketch.jsx
│   │   ├── Footer.jsx
│   │   ├── Form.jsx
│   │   ├── Header.jsx
│   │   └── Main.jsx
│   ├── App.jsx
│   └── main.jsx
server/
├── controllers/
│   └── postsController.js
├── models/
│   └── postsModel.js
├── routes/
│   └── postsRoutes.js
├── db/
│   ├── connectionDB.js
│   └── schema.sql
└── server.js
```

## Instalación

1. Crear la base de datos con `server/db/schema.sql`
2. Configurar `server/.env` con las credenciales de PostgreSQL
3. Ejecutar `npm install` en `client/` y `server/`
4. Iniciar servidor: `npm start` (desde `server/`)
5. Iniciar cliente: `npm run dev` (desde `client/`)
