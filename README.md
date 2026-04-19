# LikeMe - Social Media (PostgreSQL)

Full-stack social media app where users can share sketches, view a feed and give likes. Built with React frontend and Node.js/Express backend connected to PostgreSQL.

> Academic project developed during the Full Stack JavaScript Bootcamp at Desafío LATAM.

### Features

- Create posts with title, image URL and description
- View posts feed with like counter
- Give likes to posts
- Delete posts
- RESTful API with MVC architecture

### Technologies

**Client**
- React 18
- Vite
- Material UI (MUI)
- Axios

**Server**
- Node.js / Express
- PostgreSQL (pg)
- CORS / dotenv

### Project Structure

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

### Setup

1. Create the database using `server/db/schema.sql`
2. Configure `server/.env` with your PostgreSQL credentials
3. Run `npm install` in both `client/` and `server/`
4. Start server: `npm start` (from `server/`)
5. Start client: `npm run dev` (from `client/`)