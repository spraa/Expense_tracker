# Expense Tracker Application (MERN Stack)

## Overview
The **Expense Tracker Application** is a full-stack web app built using the MERN stack (MongoDB, Express.js, React.js, Node.js). It allows users to manage their personal finances by tracking income and expenses, visualizing spending habits, and budgeting effectively.

## Features

- **User Authentication**: Sign up and log in securely using email and password.
- **Income and Expense Tracking**: Add, edit, and delete income and expense records.
- **Category Management**: Categorize transactions for better organization.
- **Real-time Charts**: Visualize spending patterns with dynamic charts and graphs.
- **Monthly Reports**: Generate detailed monthly financial summaries.
- **Responsive Design**: Access the app seamlessly on desktop and mobile devices.

## Tech Stack

- **Frontend**: React.js, Context API (for state management)
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)
- **Styling**: Tailwind CSS

## Installation

### Prerequisites
Ensure you have the following installed on your system:
- Node.js (v14 or higher)
- MongoDB (local or cloud-based, e.g., MongoDB Atlas)

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/expense-tracker.git
   cd expense-tracker
   ```

2. **Install Dependencies**:
   Navigate to both the `client` and `server` directories to install dependencies:
   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```

3. **Set Up Environment Variables**:
   Create a `.env` file in the `server` directory with the following keys:
   ```env
   PORT=5000
   MONGO_URI=your-mongodb-connection-string
   JWT_SECRET=your-jwt-secret
   ```

4. **Run the Application**:
   - Start the backend server:
     ```bash
     cd server
     npm start
     ```
   - Start the frontend client:
     ```bash
     cd client
     npm start
     ```

5. **Access the App**:
   Open your browser and navigate to `http://localhost:3000`.

## Folder Structure

```
expense-tracker/
│
├── client/                # Frontend code
│   ├── public/            # Static files
│   ├── src/               # React app source code
│   │   ├── components/    # Reusable components
│   │   ├── pages/         # Pages for the app
│   │   ├── context/       # Context API setup
│   │   └── App.js         # Root component
│
├── server/                # Backend code
│   ├── models/            # MongoDB models
│   ├── routes/            # API routes
│   ├── controllers/       # Route handlers
│   └── server.js          # Entry point
│
└── README.md              # Documentation
```

## API Endpoints

### User Authentication
- **POST /api/auth/register**: Register a new user
- **POST /api/auth/login**: Log in an existing user

### Transactions
- **POST /api/transactions**: Add a new transaction
- **GET /api/transactions**: Fetch all transactions
- **GET /api/transactions/:id**: Fetch a specific transaction
- **PUT /api/transactions/:id**: Update a transaction
- **DELETE /api/transactions/:id**: Delete a transaction

### Reports
- **GET /api/reports/monthly**: Generate monthly financial reports

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`feature/your-feature-name`).
3. Commit your changes.
4. Push to the branch.
5. Submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgements
- Open-source libraries and tools that made this project possible.
- Inspiration from modern financial management applications.
