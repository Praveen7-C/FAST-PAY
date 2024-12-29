# FastPay - Digital Payment Wallet

## Overview
**FastPay** is a digital payment wallet built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. This project allows users to sign up, log in, and perform transactions securely with a unique UPI ID. It also provides features like transaction history and account management, making digital payments seamless and user-friendly.

---

## Features
- **User Authentication**: Secure user registration and login.
- **Digital Wallet**: Unique UPI IDs generated for each user.
- **Balance Management**: Track wallet balance in real-time.
- **Transaction Management**: Transfer funds between accounts and view transaction history.
- **Responsive UI**: Intuitive interface built with React and Bootstrap.
- **Data Security**: Secure backend using MongoDB and Express.js.

---

## Technologies Used
- **Frontend**: React.js, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Other Tools**: React Router, JSON Web Tokens (JWT), Crypto module for secure ID generation

---

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Praveen7-C/FAST-PAY.git
cd FAST-PAY
```

### 2. Install Required Packages

Ensure Node.js, npm, MongoDB, and Git are installed. Using VS Code editor, navigate to your project directory and open the terminal, then install the necessary dependencies:

In the frontend directory:
```bash
npm install react react-router-dom react-bootstrap axios bootstrap recharts web-vitals
```

In the backend directory:
```bash
npm install express mongoose cors body-parser crypto  
```

### 3. Set Up MongoDB Database  

- Launch MongoDB and create a new connection.  
- Use the connection URL: `mongodb://localhost:27017/user` with port `4003`.  
- Update this URL into your project files wherever database access is required (e.g., **home.js**, **Signup.js**, **Login.js**, **transaction.js**, **App.js**).

### 4. Run the Application

Start MongoDB:
Ensure MongoDB is running locally.

Backend:
```bash
cd backend
node server.js
```

Frontend:
```bash
cd frontend
npm start
```
This will run the React app, which should be accessible at `http://localhost:3000`.

---

## API Endpoints

### 1. User Authentication

POST /api/signup: Register a new user.

POST /api/login: Authenticate a user.

### 2. User Management

GET /api/user/:upi_id: Fetch user details by UPI ID.

### 3. Transactions

POST /api/transaction: Perform a transaction between users.

GET /api/transactions/:upi_id: Fetch all transactions for a user.

---

## Usage

1. **Sign Up**: Create a new account and get a unique UPI ID.
2. **Log In**: Use your email and password to log in.
3. **Transfer Money**: Enter the recipient's UPI ID and amount to transfer.
4. **View Transactions**: Access your transaction history on the dashboard.
5. **Transaction Graph**: Visualizes transaction history as a line chart using Recharts library, mapping transaction amounts against timestamps for an intuitive financial overview.

---

## Directory Structure

```plaintext
FAST-PAY/
├── frontend/                 # React frontend
│   ├── node_modules/         # React dependencies
│   ├── public/               # Public assets (index.html, App.js etc.)
│   ├── src/                  # React components and pages
│   │   ├── pages/            # Your React pages like Home.js, Login.js, Signup.js, Transaction.js.
│   │   │   ├── Login.js      # Login page component
│   │   │   ├── Signup.js     # Signup page component
│   │   │   ├── Transaction.js# Transaction page component
│   │   │   └── Home.js       # Home page component
│   ├── package-lock.json     # NPM lock file for frontend dependencies
│   ├── package.json          # NPM package configuration for frontend
├── backend/                  # Node.js backend
│   ├── node_modules/         # Backend dependencies
│   ├── .gitignore            # .gitignore file to ignore node_modules and unnecessary files.
│   ├── package-lock.json     # NPM lock file for backend dependencies
│   ├── package.json          # NPM package configuration for backend
│   ├── server.js             # Express server file
```

---

## Contributing

Contributions are welcome! If you have suggestions for improvements or additional features, feel free to fork the repository and submit a pull request.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments  

Special thanks to the following technologies and resources that made this project possible:  
- [React.js](https://reactjs.org/) - For building the frontend interface.  
- [Node.js](https://nodejs.org/) - As the runtime environment for backend development.  
- [Express.js](https://expressjs.com/) - For creating the server-side application.  
- [MongoDB](https://www.mongodb.com/) - For the database used to store user and transaction data.  
- [Bootstrap](https://getbootstrap.com/) - For styling the application with responsive design components.  

---

For any questions or issues, feel free to contact [gmail](nagaraju736881@gmail.com).
