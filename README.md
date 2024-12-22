# kanban_board

## Getting Started

### Prerequisites

- Node.js
- PostgreSQL

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/kanban_board.git
    cd kanban_board
    ```

2. Install server dependencies:
    ```sh
    cd server
    npm install
    ```

3. Install client dependencies:
    ```sh
    cd ../client
    npm install
    ```

4. Set up the database:
    - Create a PostgreSQL database named `kanban_db`.
    - Update the `.env` file with your database credentials.

5. Run the database migrations and seed the database:
    ```sh
    cd ../server
    npm run seed
    ```

### Running the Application

1. Start the server:
    ```sh
    cd server
    npm run dev
    ```

2. Start the client:
    ```sh
    cd ../client
    npm run dev
    ```

3. Open your browser and navigate to `http://localhost:3000`.

## API Endpoints

### Authentication

- `POST /auth/login` - Login a user

### Users

- `GET /api/users` - Get all users
- `GET /api/users/:id` - Get a user by ID
- `POST /api/users` - Create a new user
- `PUT /api/users/:id` - Update a user by ID
- `DELETE /api/users/:id` - Delete a user by ID

### Tickets

- `GET /api/tickets` - Get all tickets
- `GET /api/tickets/:id` - Get a ticket by ID
- `POST /api/tickets` - Create a new ticket
- `PUT /api/tickets/:id` - Update a ticket by ID
- `DELETE /api/tickets/:id` - Delete a ticket by ID

## License

This project is licensed under the MIT License.