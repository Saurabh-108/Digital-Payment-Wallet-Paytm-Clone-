##MERN Digital Wallet
##Overview
This project is a full-stack MERN application that allows users to send money to other users on the platform. Additionally, it includes a digital wallet feature where users can manage their balances and transactions. The system provides secure sign-in functionality and real-time money transfer between registered users.

##Features
User Authentication: Secure login and registration using JWT (JSON Web Tokens).
Digital Wallet: Each user has a personal digital wallet where they can view their current balance and transaction history.
Money Transfer: Users can send money to other users on the platform. All transactions are tracked and updated in real-time.
Transaction History: Complete history of incoming and outgoing transfers for each user.
Real-time Updates: Wallet balance and transaction history are updated in real-time upon every transfer.
Admin Panel: Admins can view all users, manage their accounts, and monitor all transactions on the platform.
Tech Stack
Frontend: React.js, Axios (or Material-UI) for responsive design
Backend: Node.js, Express.js
Database: MongoDB for storing user information, balances, and transactions
Authentication: JWT (JSON Web Tokens) for secure sign-in
Real-time Updates: WebSockets or polling for real-time updates (optional)
Deployment: (Add information on your deployment platform, e.g., Heroku, Vercel)
#Prerequisites
@Node.js
MongoDB
Git
A valid Admin JWT token for admin functionality.
Usage
For Regular Users:
Sign up or sign in to the application.
Once logged in, the user will have access to their digital wallet and transaction history.
Users can transfer money to other registered users by entering the recipient's username and the amount they wish to send.
The wallet balance will automatically update after each transaction.
For Admin Users:
Login with Admin Credentials: Admins will need a special admin JWT token to access the admin panel.
View All Users: Admins can view a list of all registered users, their wallet balances, and transaction histories.
Monitor Transactions: Admins can track all transactions on the platform, including transfers made between users.
Manage User Accounts: Admins can update user information, suspend accounts, and ensure the integrity of the platform.
Environment Variables
The following environment variables are required:

MONGO_URI: MongoDB connection string
JWT_SECRET: Secret key for JWT authentication
ADMIN_SECRET_KEY: Admin secret key for validating admin users.
Installation
Clone the repository:

bash
Copy
git clone https://github.com/yourusername/mern-wallet-app.git
cd mern-wallet-app
Install dependencies:

For the backend:

bash
Copy
cd backend
npm install
For the frontend:

bash
Copy
cd frontend
npm install
Configure environment variables:

Create a .env file in the backend directory and add the following variables:
bash
Copy
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret_key
ADMIN_SECRET_KEY=your_admin_secret_key
Start the application:

For the backend:
bash
Copy
cd backend
npm run dev
For the frontend:
bash
Copy
cd frontend
npm start
Access the Application:

The frontend will be running on http://localhost:3000 by default.
The backend API will be available on http://localhost:5000 (or the configured port).
