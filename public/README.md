# Snappy Chat Application

Snappy is a real-time chat application developed using **React** for the frontend and **Node.js** for the backend. It leverages WebSocket for bi-directional communication, enabling users to exchange messages in real-time. This project was developed as a final-year MCA project.

## Features

- **User Authentication**: Secure login and registration system.
- **Real-Time Messaging**: Instant communication powered by WebSocket.
- **Chat Rooms**: Users can create and join chat rooms.
- **Responsive Design**: Optimized for various devices including desktops and mobiles.

## Prerequisites

To run this project locally, ensure the following tools are installed on your system:

- **Node.js** (LTS version recommended)
- **npm** or **yarn** (comes with Node.js)
- **MongoDB** (for the database)

## Installation and Setup

Follow these steps to set up and run the project:

### Step 1: Clone the Repository

```bash
git clone <repository-url>
cd Snappy
```

### Step 2: Install Dependencies

#### Backend (Node.js)

Navigate to the `server` folder:

```bash
cd server
```

Install the required dependencies:

```bash
npm install
```

#### Frontend (React)

Navigate to the frontend folder:

```bash
cd ../public
```

Install the required dependencies:

```bash
npm install
```

### Step 3: Set Up Environment Variables

#### Backend

Create a `.env` file in the `server` folder and configure the following variables:

```env
PORT=5000
MONGO_URI=<your-mongodb-uri>
JWT_SECRET=<your-jwt-secret>
```

Replace `<your-mongodb-uri>` and `<your-jwt-secret>` with your MongoDB connection string and a secure secret key for JWT authentication.

#### Frontend

Create a `.env` file in the `public` folder and configure the following variable:

```env
REACT_APP_API_URL=http://localhost:5000
```

Ensure the `REACT_APP_API_URL` matches the backend server's URL.

### Step 4: Start the Servers

#### Backend

Start the backend server by running the following commands in the `server` folder:

```bash
npm start
```

#### Frontend

Start the frontend server by running the following commands in the `public` folder:

```bash
npm start
```

### Step 5: Access the Application

Once both servers are running:

- Open your browser and navigate to `http://localhost:3000` for the frontend.
- Ensure the backend server is running at `http://localhost:5000`.

## Project Structure

### Backend

- `index.js`: Entry point of the backend server.
- `controllers/`: Handles request logic.
- `models/`: Defines database schemas.
- `routes/`: API route definitions.
- `.env`: Contains backend environment variables.

### Frontend

- `src/components/`: Reusable React components.
- `src/pages/`: Main application pages.
- `src/context/`: Global state management.
- `src/utils/`: Utility functions for the frontend.

## Technologies Used

### Frontend

- React
- Axios
- Context API
- CSS for styling

### Backend

- Node.js
- Express.js
- MongoDB (Mongoose)
- WebSocket (Socket.io)
- JWT for authentication

## Future Enhancements

- Add file-sharing capabilities.
- Implement typing indicators.
- Improve UI/UX with animations and transitions.
- Deploy the application to a cloud platform.

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests to enhance the project.

## License

This project is licensed under the MIT License.

---

Feel free to reach out for any questions or support while setting up the project.

