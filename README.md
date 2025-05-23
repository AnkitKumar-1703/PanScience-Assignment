## Setup and Running the Application

### Clone the Repository

1. Clone the repository:
   ```bash
   git clone https://github.com/AnkitKumar-1703/PanScience-Assignment
   ```
2. Navigate to the project directory:
   ```bash
   cd PanScience-Assignment
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install all dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install all dependencies:
   ```bash
   npm install
   ```
3. Start the development server: If you have nodemon installed:
   ```bash
   npm run dev
   ```
   If you don't have nodemon:
   ```bash
   npm run start
   ```


## API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login and receive JWT
- `GET /api/auth/me` - Get current user profile

### Users
- `GET /api/users` - Get all users (admin only)
- `GET /api/users/:id` - Get user by ID (admin or owner)
- `POST /api/users` - Create a new user (admin only)
- `PUT /api/users/:id` - Update a user (admin or owner)
- `DELETE /api/users/:id` - Delete a user (admin only)

### Tasks
- `GET /api/tasks` - Get all tasks (filtered by permissions)
- `GET /api/tasks/:id` - Get task by ID
- `POST /api/tasks` - Create a new task
- `PUT /api/tasks/:id` - Update a task
- `DELETE /api/tasks/:id` - Delete a task
- `PATCH /api/tasks/:id/status` - Update task status with note