# GoFood

GoFood is a food-ordering web application with a React frontend and an Express/MongoDB backend. Users can browse food and categories, create an account or log in, add items to a cart, and view their orders.

## Tech stack

- React and React Router
- Bootstrap and Material-UI
- Node.js and Express
- MongoDB with Mongoose

## Run the frontend

From the repository root:

```bash
npm install
npm start
```

The development server opens at [http://localhost:3000](http://localhost:3000).

## Run the backend locally

The backend is in the `backend` directory and listens on port `5000`.

1. Configure a MongoDB connection in `backend/db.js`. The database should contain the `food_items` and `foodCategory` collections.
2. Install backend dependencies and start the server:

   ```bash
   cd backend
   npm install
   node index.js
   ```

The frontend currently sends API requests to the deployed service at `https://speedyeat.onrender.com`. To use a local backend, update those API URLs in the frontend to point to `http://localhost:5000`.

## Available frontend scripts

Run these commands from the repository root:

| Command | Description |
| --- | --- |
| `npm start` | Start the development server |
| `npm test` | Run tests in watch mode |
| `npm run build` | Create a production build |
