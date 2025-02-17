# Club Management System (CMS)

This repository contains both the frontend and backend code for the Club Management System (CMS) project. The CMS is designed to streamline the management of student clubs, providing features for users, admins, and super admins.

## Technologies Used

### Frontend
- **React**: JavaScript library for building user interfaces
- **Axios**: Promise-based HTTP client for making API requests
- **React Router**: Routing library for React applications

### Backend
- **Node.js**: JavaScript runtime environment
- **Express.js**: Web application framework for Node.js
- **MongoDB**: NoSQL database for data storage
- **Mongoose**: Object Data Modeling (ODM) library for MongoDB
- **JWT**: JSON Web Tokens for authentication
- **Bcrypt**: Library for hashing passwords
- **Nodemailer**: For sending emails

---
## Getting Started

### Clone the repository
```sh
git clone https://github.com/kulkamalsingh/CLUBHUB-mern-sms.git
cd clubhub
```

### Setting Up the Frontend
```sh
cd frontend
npm install
npm start
```
The development server will start running on `http://localhost:3000`.

### Setting Up the Backend
```sh
cd backend
npm install
```

#### Seed the database (if needed)
```sh
node server/config/seed.js
```

#### Set up environment variables
1. Rename `.env.example` to `.env`
2. Modify the `.env` file with your configurations (MongoDB connection string, JWT secret, etc.)

#### Start the server
```sh
npm start
```
The backend server will start running on `http://localhost:8000`.

---
## Folder Structure

```
clubhub/
│── frontend/     # Frontend source code
│   ├── src/
│   │   ├── components/   # Reusable UI components
│   │   ├── views/        # Page-specific components
│   │   ├── utils/        # Utility functions (API calls, auth handling)
│   │   ├── config.js     # Global constants
│   │   ├── App.js        # Main app entry point
│   │   ├── index.js      # Renders React DOM
│   ├── public/          # Static assets
│   ├── package.json     # Frontend dependencies
│
│── backend/      # Backend source code
│   ├── controllers/  # API controllers
│   ├── models/       # Mongoose models
│   ├── middlewares/  # Express middlewares
│   ├── routes/       # API routes
│   ├── config/       # Database config & seed files
│   ├── utils/        # Helper functions (auth, email, etc.)
│   ├── tests/        # Unit tests
│   ├── app.js        # Express app setup
│   ├── server.js     # Server entry point
│   ├── package.json  # Backend dependencies
│
│── .gitignore
│── README.md
```

---
## Available Scripts

### Frontend
- `npm start` - Starts the development server.
- `npm run build` - Builds the application for production.
- `npm test` - Runs the test suites.
- `npm run eject` - Ejects the Create React App configuration.

### Backend
- `npm start` - Starts the Express server.
- `npm test` - Runs backend test suites.

---
## API Endpoints (Backend)

### User Routes
- **GET** `/api/v1/super-admin/users` - Fetch all users
- **POST** `/api/v1/register` - Create a new user
- **PUT** `/api/v1/me/update` - Update a user profile

...and more.

---
## Contributing
Contributions are welcome! If you find any issues or have suggestions, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

