# visa-companion

# MERN Stack Application Documentation

This documentation provides instructions to set up and run the MERN stack application locally. The project is structured with the frontend named `client` and the backend named `server`.

---

## Prerequisites

Ensure you have the following tools installed on your machine:

- [Node.js](https://nodejs.org/) (version 14.x or higher)
- [Yarn](https://yarnpkg.com/) (for managing frontend dependencies)
- [npm](https://www.npmjs.com/) (for managing backend dependencies)
- [MongoDB](https://www.mongodb.com/) (for the database)

---

## Getting Started

### Step 1: Clone the Repository

```bash
git clone https://github.com/Nmesoma-solomon-peter/visa-companion.git
cd visa-companion
```


### Step 2: Set Up the Backend (`server`)

1. Navigate to the backend folder:
   ```bash
   cd server
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the `server` folder and configure the following variables:
   ```env
   PORT=5000
   MONGO_URI=<your-mongodb-connection-string>
   JWT_SECRET=<your-jwt-secret>
   ```
 
4. Start the backend server:
   ```bash
   nodemon app.js
   ```
   The server should now be running on `http://localhost:5000`.

### Step 3: Set Up the Frontend (`client`)

1. Navigate to the frontend folder:
   ```bash
   cd ../client
   ```

2. Install dependencies:
   ```bash
   yarn install
   ```

3. Start the frontend development server:
   ```bash
   yarn dev
   or 
   yarn dev --host 
   ```
   The frontend should now be running on `http://localhost:5173` (default Vite port).

---

## Running the Application

With both the backend (`server`) and frontend (`client`) running, you can:

- Access the frontend at [http://localhost:5173](http://localhost:5173)
- Interact with the backend API at [http://localhost:5000](http://localhost:5000)

---

## Scripts

### Backend Scripts

Run these commands in the `server` folder:

<!-- - `npm start`: Start the backend server
- `npm run dev`: Start the backend server in development mode with hot reloading (if configured) -->
`nodemon app.js`

### Frontend Scripts

Run these commands in the `client` folder:

- `yarn dev`: Start the frontend development server
- `yarn build`: Build the frontend for production
- `yarn preview`: Preview the production build locally

---

## Troubleshooting

- **Database Connection Issues**: Ensure your MongoDB server is running and the `MONGO_URI` in the `.env` file is correct.
- **Port Conflicts**: Verify that ports `5000` (backend) and `5173` (frontend) are not in use by other applications.
- **Environment Variables**: Ensure your `.env` files are correctly set up.

---

## Contributing

Feel free to fork the repository and create pull requests for improvements or bug fixes.

---

