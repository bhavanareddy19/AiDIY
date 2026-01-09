<div align="center">

# 🌟 AiDIY - AI-Powered Financial Literacy Platform

### Empowering Children with Smart Money Management Skills

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![React](https://img.shields.io/badge/React-18.2-61DAFB.svg)](https://reactjs.org/)
[![Flask](https://img.shields.io/badge/Flask-2.3-000000.svg)](https://flask.palletsprojects.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Latest-47A248.svg)](https://www.mongodb.com/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o-412991.svg)](https://openai.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

[Live Demo](#) • [Documentation](#getting-started) • [Report Bug](#) • [Request Feature](#)

</div>

---

## 📋 Table of Contents

- [About The Project](#about-the-project)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Screenshots](#screenshots)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🎯 About The Project

**AiDIY** is an innovative educational platform that revolutionizes financial literacy education for children by combining cutting-edge artificial intelligence with gamification principles. The platform creates a safe, engaging environment where children can learn essential money management skills through personalized learning experiences, interactive challenges, and real-world practice scenarios.

### 🌈 The Vision

In today's digital age, financial literacy is more crucial than ever. AiDIY bridges the gap between traditional financial education and modern technology, making learning about money fun, interactive, and accessible for children of all ages.

### 🎖️ What Makes It Special

- **AI-Powered Learning**: Leverages OpenAI's GPT-4o for personalized financial coaching
- **Gamification**: Makes financial education engaging through rewards, achievements, and challenges
- **Parent Dashboard**: Comprehensive tools for parents to monitor and guide their children's financial journey
- **Multi-Modal Interaction**: Supports text, voice, and image-based communication with the AI assistant
- **Real-World Application**: Provides practical experience with saving, goal-setting, and earning through chores

---

## ✨ Key Features

### 👨‍👩‍👧‍👦 For Parents

- **📊 Comprehensive Dashboard**
  - Real-time monitoring of children's progress
  - Visual analytics and insights
  - Multi-child profile management

- **🤖 AI Financial Coach**
  - Personalized advice based on child's assessment
  - Voice and chat interface with GPT-4o
  - Image recognition for teaching financial concepts

- **📝 Task & Chore Management**
  - Create and assign age-appropriate financial tasks
  - AI-powered chore recommendations
  - Customizable reward system

- **📈 Progress Tracking**
  - Detailed learning journey analytics
  - Goal completion monitoring
  - Financial knowledge assessments

### 👧👦 For Children

- **🎮 Gamified Learning Experience**
  - Earn rewards and unlock achievements
  - Interactive financial challenges
  - Fun, age-appropriate content

- **🏦 Virtual Piggy Bank**
  - Practice saving in a safe environment
  - Set and track financial goals
  - Learn money management fundamentals

- **🎯 Goal-Setting System**
  - Create personalized savings goals
  - Track progress visually
  - Learn delayed gratification

- **⭐ Achievement System**
  - Complete chores to earn rewards
  - Build financial responsibility
  - Develop good money habits

---

## 🛠️ Tech Stack

### Frontend
```
⚛️  React 18.2          - Modern UI library
🔄  Redux Toolkit       - State management
🎨  Tailwind CSS        - Utility-first styling
🚦  React Router v6     - Client-side routing
📡  Axios               - HTTP client
```

### Backend
```
🐍  Python 3.8+         - Core language
🌶️  Flask 2.3          - Web framework
🍃  MongoDB             - NoSQL database
🔐  JWT                 - Authentication
🧠  OpenAI GPT-4o       - AI integration
📧  Flask-Mail          - Email services
```

### DevOps & Tools
```
🐳  Docker              - Containerization
☁️  Vercel/Railway      - Deployment platforms
🔧  Git                 - Version control
📝  Postman             - API testing
```

---

## 🏗️ Architecture

### System Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                     Frontend (React)                        │
│  ┌────────────┬──────────────┬─────────────┬─────────────┐ │
│  │  Dashboard │  Auth Pages  │  Kid Pages  │  AI Chat    │ │
│  └────────────┴──────────────┴─────────────┴─────────────┘ │
└───────────────────────────┬─────────────────────────────────┘
                            │ REST API
┌───────────────────────────┴─────────────────────────────────┐
│                    Backend (Flask)                          │
│  ┌──────────┬───────────┬──────────┬────────────────────┐  │
│  │   Auth   │  User Mgmt │  AI API  │  Task Management  │  │
│  └──────────┴───────────┴──────────┴────────────────────┘  │
└───────────────────────────┬─────────────────────────────────┘
                            │
        ┌───────────────────┼───────────────────┐
        │                   │                   │
┌───────▼────────┐  ┌──────▼──────┐   ┌───────▼────────┐
│    MongoDB     │  │  OpenAI API │   │   Gmail SMTP   │
│   (Database)   │  │  (AI Coach) │   │  (Email OTP)   │
└────────────────┘  └─────────────┘   └────────────────┘
```

### Database Schema

**Collections:**
- `users` - Parent account information
- `children` - Child profiles and data
- `goals` - Savings goals and progress
- `chores` - Task assignments and completion
- `chat_sessions` - AI conversation history
- `notifications` - System notifications
- `otps` - One-time passwords for authentication

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

```bash
# Required
- Python 3.8 or higher
- Node.js 14.x or higher
- MongoDB 4.x or higher
- Git

# Recommended
- pip (Python package manager)
- npm (Node package manager)
- MongoDB Compass (for database management)
```

### API Keys Required

1. **OpenAI API Key** - [Get it here](https://platform.openai.com/api-keys)
2. **Google OAuth Credentials** - [Console](https://console.cloud.google.com/)
3. **Gmail App Password** - [Setup Guide](https://support.google.com/accounts/answer/185833)

---

## 📥 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/AiDIY.git
cd AiDIY
```

### 2️⃣ Backend Setup

```bash
# Create and activate virtual environment
python -m venv .venv

# On Windows:
.venv\Scripts\activate

# On macOS/Linux:
source .venv/bin/activate

# Install Python dependencies
pip install -r requirements.txt
```

### 3️⃣ Frontend Setup

```bash
# Navigate to client directory
cd client

# Install dependencies
npm install

# Return to root directory
cd ..
```

### 4️⃣ Environment Configuration

Create a `.env` file in the root directory:

```bash
# Copy the example file
cp .env.example .env

# Edit .env with your actual credentials
```

**Important Environment Variables:**

```env
# MongoDB
MONGO_URI=mongodb://localhost:27017/aidiy_app

# Security
JWT_SECRET=your_super_secret_jwt_key
FLASK_SECRET_KEY=your_flask_secret_key

# OpenAI
OPENAI_API_KEY=sk-your_openai_api_key

# Email (Gmail)
MAIL_USERNAME=your_email@gmail.com
MAIL_PASSWORD=your_app_password

# Development
DEV_MODE=True
```

### 5️⃣ Database Setup

```bash
# Start MongoDB
# On Windows:
net start MongoDB

# On macOS (Homebrew):
brew services start mongodb-community

# On Linux:
sudo systemctl start mongod
```

---

## 💻 Usage

### Running the Application

**Option 1: Manual Start (Recommended for Development)**

Terminal 1 - Backend:
```bash
# Activate virtual environment
.venv\Scripts\activate  # Windows
source .venv/bin/activate  # macOS/Linux

# Start Flask server
python app.py

# Server runs on http://localhost:5500
```

Terminal 2 - Frontend:
```bash
# Navigate to client directory
cd client

# Start React development server
npm start

# App opens on http://localhost:3000
```

**Option 2: Using Start Script**

```bash
# Make script executable (macOS/Linux only)
chmod +x start.sh

# Run the script
./start.sh
```

### 🎯 Testing the Application

1. **Access the Application**
   - Open browser: `http://localhost:3000`

2. **Create a Parent Account**
   - Click "Sign Up"
   - Fill in registration details
   - Verify email with OTP
   - Complete profile setup

3. **Add a Child Profile**
   - Navigate to "Add Child"
   - Enter child's information
   - Set up login credentials

4. **Explore Features**
   - Try the AI Coach
   - Create chores and tasks
   - Set up savings goals
   - Monitor progress

---

## 📡 API Documentation

### Authentication Endpoints

#### Register User
```http
POST /api/auth/register
Content-Type: application/json

{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john@example.com",
  "password": "SecurePass123!",
  "phoneNumber": "+1234567890"
}
```

#### Login
```http
POST /api/auth/login
Content-Type: application/json

{
  "email": "john@example.com",
  "password": "SecurePass123!"
}

Response: {
  "success": true,
  "appToken": "jwt_token_here",
  "user": { ... }
}
```

#### Verify OTP
```http
POST /api/auth/verify-otp
Content-Type: application/json

{
  "email": "john@example.com",
  "otp": "123456"
}
```

### User Management

#### Get Profile
```http
GET /api/users/profile
Authorization: Bearer {token}

Response: {
  "success": true,
  "user": { ... }
}
```

#### Update Profile
```http
PUT /api/users/profile
Authorization: Bearer {token}
Content-Type: application/json

{
  "firstName": "John",
  "lastName": "Doe",
  "parentRole": "Dad",
  "choreCategories": ["Kitchen", "Cleaning"]
}
```

### Children Management

#### Get Children
```http
GET /api/users/children
Authorization: Bearer {token}
```

#### Add Child
```http
POST /api/users/children
Authorization: Bearer {token}
Content-Type: application/json

{
  "firstName": "Emma",
  "lastName": "Doe",
  "birthDate": "2015-05-20",
  "username": "emma_doe",
  "loginCode": "1234",
  "nickName": "Emmy",
  "avatar": "👧"
}
```

### AI & Chat

#### Chat with AI
```http
POST /api/ai/chat
Authorization: Bearer {token}
Content-Type: application/json

{
  "message": "How can I teach my child about saving?",
  "session_id": "optional_session_id",
  "image": "base64_encoded_image_optional"
}

Response: {
  "success": true,
  "response": "AI response here",
  "session_id": "session_id"
}
```

#### Speech to Text
```http
POST /api/ai/speech-to-text
Authorization: Bearer {token}
Content-Type: multipart/form-data

{
  "audio": audio_file
}
```

### Goals & Progress

#### Create Goal (Child)
```http
POST /api/goals
Authorization: Bearer {token}
Content-Type: application/json

{
  "title": "New Bicycle",
  "category": "Toy",
  "amount": 150.00,
  "duration": 30,
  "description": "A cool mountain bike"
}
```

#### Approve Goal (Parent)
```http
POST /api/goals/{goal_id}/approve
Authorization: Bearer {token}
```

### Chores

#### Get Chores
```http
GET /api/chores
Authorization: Bearer {token}
```

#### Create Chore (Parent)
```http
POST /api/chores
Authorization: Bearer {token}
Content-Type: application/json

{
  "title": "Clean Room",
  "description": "Organize toys and make bed",
  "category": "Cleaning",
  "difficulty": "Easy",
  "reward": 5.00,
  "dueDate": "2026-01-15",
  "assignedTo": "emma_doe"
}
```

### Notifications

#### Get Notifications
```http
GET /api/notifications
Authorization: Bearer {token}

Response: {
  "success": true,
  "notifications": [ ... ],
  "unread_count": 3
}
```

---

## 📸 Screenshots

> Add screenshots of your application here once deployed

```
[Parent Dashboard]     [Child Interface]      [AI Chat]
[Goal Tracking]        [Chore Management]     [Progress Analytics]
```

---

## 🗺️ Roadmap

### Current Version (v1.0)
- ✅ User authentication (Email & Google OAuth)
- ✅ Parent and child profiles
- ✅ AI-powered financial coach
- ✅ Goal setting and tracking
- ✅ Chore management system
- ✅ Progress notifications

### Upcoming Features (v2.0)
- 🔲 Mobile app (React Native)
- 🔲 Multiple language support
- 🔲 Advanced analytics dashboard
- 🔲 Social features (share achievements)
- 🔲 Marketplace for virtual goods
- 🔲 Parent-child messaging system
- 🔲 Integration with real banks (future)
- 🔲 Augmented reality learning modules

---

## 🔒 Security Features

- **🔐 Password Hashing**: Bcrypt encryption for all passwords
- **🎫 JWT Tokens**: Secure session management with expiration
- **📧 Email Verification**: OTP-based email confirmation
- **🛡️ CORS Protection**: Configured cross-origin resource sharing
- **🔑 Environment Variables**: Sensitive data stored securely
- **✅ Input Validation**: Server-side validation for all inputs
- **🚫 SQL Injection Prevention**: NoSQL database with sanitized queries

---

## 🧪 Testing

```bash
# Run backend tests
pytest

# Run frontend tests
cd client
npm test

# Run with coverage
npm test -- --coverage
```

---

## 📦 Deployment

### Deploy to Vercel (Frontend)

```bash
cd client
npm run build
vercel --prod
```

### Deploy to Railway (Backend)

```bash
# Install Railway CLI
npm i -g @railway/cli

# Login
railway login

# Deploy
railway up
```

### Docker Deployment

```bash
# Build image
docker build -t aidiy .

# Run container
docker run -p 5500:5500 -p 3000:3000 aidiy
```

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` file for more information.

---

## 👨‍💻 Author

**Your Name**

- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)
- Email: your.email@example.com
- Portfolio: [yourwebsite.com](https://yourwebsite.com)

---

## 🙏 Acknowledgments

- [OpenAI](https://openai.com/) for the GPT-4o API
- [MongoDB](https://www.mongodb.com/) for the database platform
- [React](https://reactjs.org/) and [Flask](https://flask.palletsprojects.com/) communities
- All contributors and testers who helped improve this project
- Parents and educators who provided valuable feedback

---

## 💡 Project Highlights for Recruiters

### Technical Achievements

✨ **Full-Stack Development**
- Built complete MERN-style stack (MongoDB, Express-like Flask, React, Node.js)
- Implemented RESTful API architecture
- Real-time data synchronization

✨ **AI Integration**
- Integrated OpenAI GPT-4o for intelligent responses
- Multi-modal AI (text, voice, image processing)
- Context-aware conversation management

✨ **Authentication & Security**
- JWT-based authentication
- OAuth 2.0 integration (Google)
- OTP email verification system
- Bcrypt password encryption

✨ **State Management**
- Redux Toolkit for complex state management
- Optimistic UI updates
- Persistent session handling

✨ **Database Design**
- NoSQL schema design with MongoDB
- Efficient indexing strategies
- Data relationship management

✨ **User Experience**
- Responsive design for all devices
- Intuitive navigation flows
- Gamification elements
- Real-time notifications

### Business Value

📊 **Addresses Real Problem**: Financial illiteracy in children
🎯 **Target Market**: Parents with children aged 5-18
💰 **Monetization Potential**: Premium features, subscriptions
📈 **Scalability**: Cloud-ready architecture
🌍 **Market Reach**: Global accessibility

### Code Quality

- Clean, maintainable code structure
- Comprehensive error handling
- RESTful API conventions
- Component-based architecture
- Separation of concerns

---

<div align="center">

### ⭐ Star this repository if you find it helpful!

**Made with ❤️ and lots of ☕**

[Back to Top](#-aidiy---ai-powered-financial-literacy-platform)

</div>
