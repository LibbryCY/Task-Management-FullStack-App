# Task Management FullStack App

Task Management FullStack App is a web application for managing tasks that allows users to create, view, update, and delete tasks. The application is built using NestJS for the backend, React for the frontend, and PostgreSQL for the database. It provides a simple and intuitive interface for task management.

## Features
- **Create Tasks**: Users can add new tasks with a title, description, and status.
- **View Tasks**: Display all tasks in a tabular format with filtering and sorting options.
- **Update Tasks**: Ability to modify existing tasks.
- **Delete Tasks**: Remove tasks that are no longer needed.
- **Registration and Login**: Users can create accounts and log in to access their tasks.

## Technologies
- **Frontend**: React.js, HTML, CSS, JavaScript
- **Backend**: NestJS, TypeScript
- **Database**: PostgreSQL
- **Authentication**: JWT (JSON Web Tokens)
- **Other Libraries and Tools**: Axios, Prime, React Router, Bootstrap

## How to Run the Project

### Prerequisites
- Node.js and npm installed on your machine.
- PostgreSQL database.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/LibbryCY/Task-Management-FullStack-App.git
   cd Task-Management-FullStack-App
   ```

2. Install backend dependencies:
   ```bash
   cd backend
   npm install
   ```

3. Install frontend dependencies:
   ```bash
   cd ../frontend
   npm install
   ```

4. Configure PostgreSQL:
   - Create a `.env` file in the backend directory and add the following variables:
   ```env
   DATABASE_HOST=your_database_host
   DATABASE_PORT=your_database_port
   DATABASE_USER=your_database_user
   DATABASE_PASSWORD=your_database_password
   DATABASE_NAME=your_database_name
   JWT_SECRET=your_jwt_secret_key
   ```

5. Run database migrations:
   ```bash
   cd backend
   npm run migration:run
   ```

6. Start the backend server:
   ```bash
   npm run start
   ```

7. Start the frontend application:
   ```bash
   cd ../frontend
   npm start
   ```

8. Access the application:
   - Open your browser and go to [http://localhost:3000](http://localhost:3000).

## Project Structure
- **backend**: NestJS application with modules, controllers, services, and entities.
- **frontend**: React application with components, routes, and services for backend communication.
- **migrations**: SQL migrations for the PostgreSQL database.
- **entities**: TypeORM entities for tasks and users.
- **services**: Business logic for handling requests.
- **controllers**: Controllers for handling HTTP requests.

## Additional Information
- The application uses JWT for authentication, ensuring secure login and registration.
- Tasks are associated with users, so each user can only see their own tasks.

## Author
LibbryCY - GitHub Profile

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
