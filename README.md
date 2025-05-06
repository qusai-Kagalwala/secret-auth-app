# 🔐 Secrets Project

## 🌟 Overview
A secure authentication application built with Node.js, Express, EJS templates, and PostgreSQL. This app allows users to register, login, and share secrets anonymously.

## ✨ Features
- 🔒 Secure user authentication with Passport.js
- 🛡️ Password encryption using bcrypt
- 📊 PostgreSQL database for user storage
- 🖌️ EJS templating for responsive UI
- 🔑 Session management for persistent login

## 🚀 Getting Started

### Prerequisites
- Node.js
- PostgreSQL
- npm

### 🛠️ Installation
1. Clone the repository:
```bash
git clone https://github.com/qusai-Kagalwala/secret-auth-app.git
cd secret-auth-app
```

2. Install dependencies:
```bash
npm install
```

3. Set up your database:
```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(100) UNIQUE NOT NULL,
  password VARCHAR(100) NOT NULL
);
```

4. Create a `.env` file in the root directory with the following variables:
```
# PostgreSQL Configuration
PG_USER=your_postgres_username
PG_HOST=localhost
PG_DATABASE=your_database_name
PG_PASSWORD=your_postgres_password
PG_PORT=5432

# Session Secret
SESSION_SECRET=your_session_secret
```

## 🏃‍♂️ Running the Application
```bash
node index.js
```
Access the application at `http://localhost:3000`

## 📝 Project Structure
```
secret-auth-app/
├── index.js           # Main server file
├── package.json       # Dependencies
├── public/            # Static assets
│   └── css/
│       └── styles.css # Custom styles
└── views/             # EJS templates
    ├── home.ejs       # Landing page
    ├── login.ejs      # Login form
    ├── register.ejs   # Registration form
    ├── secrets.ejs    # Protected content
    └── partials/      # Reusable template parts
        ├── header.ejs
        └── footer.ejs
```

## 🔒 Security Features
- Password hashing with bcrypt (salt rounds: 10)
- Session-based authentication
- Protected routes requiring authentication
- Environment variables for sensitive information

## 💻 Tech Stack
- 🖥️ **Node.js** - JavaScript runtime
- 🛣️ **Express** - Web framework
- 🎨 **EJS** - Templating engine
- 🗄️ **PostgreSQL** - Database
- 🔐 **Passport.js** - Authentication middleware
- 🔄 **Express-session** - Session management
- 🔒 **Bcrypt** - Password hashing

## 📝 Future Enhancements
- Add social login options (Google, GitHub, etc.)
- Implement ability to add and delete secrets
- Add profile management features
- Improve UI/UX with modern design

## 👨‍💻 Author
Qusai Kagalwala - [GitHub Profile](https://github.com/qusai-Kagalwala)

---

⭐️ **Star this repo if you find it useful!** ⭐️
