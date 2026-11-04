# FindFound – Lost & Found Platform

FindFound is a web-based Lost and Found platform designed to help people report, discover, and recover lost belongings. It provides a centralized place where users can post lost or found items and communicate with others to improve the chances of recovering their belongings.

## Features

- **User Authentication:** Register and log in securely.
- **Lost Item Reporting:** Create reports for items that have been lost.
- **Found Item Reporting:** Post details about items that have been found.
- **Item Discovery:** Browse and search reported items.
- **Ownership Verification:** Verify ownership before returning an item.
- **Real-Time Communication:** Communicate with other users through messaging.
- **Notifications:** Receive updates about relevant activities.
- **OTP Verification:** Email-based OTP verification during registration.
- **Dashboard:** Manage reports and access platform features from a centralized dashboard.

## Tech Stack

### Frontend
- React.js
- Vite
- JavaScript
- HTML5
- CSS3

### Backend
- Node.js
- Express.js
- REST APIs
- JWT Authentication

### Database
- MongoDB
- Mongoose

### Tools
- Git and GitHub
- Visual Studio Code
- npm

## Project Structure

```text
FindFound/
│
├── findback/
│   └── client/
│       ├── public/
│       ├── src/
│       │   ├── assets/
│       │   ├── components/
│       │   ├── pages/
│       │   ├── App.jsx
│       │   ├── App.css
│       │   ├── config.js
│       │   ├── index.css
│       │   └── main.jsx
│       ├── package.json
│       └── vite.config.js
│
├── server/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── package.json
│
├── package.json
└── README.md
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/d4rsh4n/FindFound.git
cd FindFound
```

### 2. Install backend dependencies

```bash
cd server
npm install
```

### 3. Configure backend environment variables

Create a `.env` file inside the `server` directory.

```env
PORT=5001
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secure_jwt_secret
```

Add any email service credentials required by your configured OTP provider. Keep all credentials private.

### 4. Start the backend

From the `server` directory:

```bash
npm start
```

The backend should run at:

```text
http://localhost:5001
```

### 5. Install frontend dependencies

Open a second terminal:

```bash
cd FindFound/findback/client
npm install
```

If you are already in the project root, use:

```bash
cd findback/client
```

### 6. Start the frontend

```bash
npm run dev
```

Open the local development URL displayed by Vite, usually:

```text
http://localhost:5173
```

Keep both frontend and backend terminals running while using the application.

## Environment Variables

| Variable | Description |
|---|---|
| `PORT` | Backend server port |
| `MONGO_URI` | MongoDB connection string |
| `JWT_SECRET` | Secret used for JWT authentication |

Email-related environment variables depend on the email provider configured in the backend.

**Never upload your `.env` file, passwords, API keys, or private credentials to GitHub.**

## Running Locally

To run FindFound, you need:

1. A running MongoDB database (such as MongoDB Atlas).
2. A configured backend environment file.
3. The Express backend running on port 5001.
4. The Vite frontend running on port 5173.

## Future Improvements

- Advanced search and filtering.
- Improved item-matching recommendations.
- Enhanced ownership verification.
- Improved mobile responsiveness.
- Additional notification features.

## Author

**Darshan**

GitHub: [@d4rsh4n](https://github.com/d4rsh4n)

## License

This project is currently available for educational and development purposes. No open-source licence has been specified.
