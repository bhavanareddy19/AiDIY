# 💰 AiDIY - AI-Powered Financial Literacy for Kids

<div align="center">

![Version](https://img.shields.io/badge/version-1.0-blue.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-86.3%25-yellow.svg)
![Python](https://img.shields.io/badge/Python-11.7%25-green.svg)
![License](https://img.shields.io/badge/license-MIT-purple.svg)

**Teaching children money management through gamification and AI-powered coaching**

[Features](#-key-features) • [Tech Stack](#-tech-stack) • [Installation](#-installation) • [Demo](#-demo)

</div>

---

## 📋 Overview

**AiDIY** is an innovative financial literacy platform that makes learning about money fun and engaging for children. By combining gamification, AI coaching, and practical money management tools, AiDIY helps kids develop healthy financial habits from an early age.

### 🎯 The Problem

- **70% of children** lack basic financial literacy skills
- Traditional financial education is boring and inaccessible
- Parents struggle to teach money management effectively
- Kids learn best through interactive, gamified experiences

### ✅ The Solution

AiDIY provides:
- **AI Financial Coach** powered by GPT-4o for personalized guidance
- **Gamified Learning** with challenges, rewards, and goal tracking
- **Practical Tools** for savings, budgeting, and chore management
- **Parent Dashboard** for monitoring progress and engagement

---

## ✨ Key Features

### 🤖 **AI-Powered Coaching**
- GPT-4o-based financial advisor tailored for children
- Multi-modal support: voice, text, and image interactions
- Personalized learning paths based on age and progress
- Real-time financial tips and encouragement

### 🎮 **Gamification System**
- Interactive challenges and quests
- Achievement badges and rewards
- Progress tracking and leaderboards
- Goal-setting and milestone celebrations

### 💼 **Money Management Tools**
- Virtual savings accounts with goal tracking
- Chore assignment with reward systems
- Budget planning and expense tracking
- Parent-supervised transactions

### 👨‍👩‍👧 **Parent Dashboard**
- Real-time progress monitoring
- Activity logs and reports
- Customizable chore assignments
- Notification system for milestones

### 🔒 **Security & Authentication**
- JWT and OAuth 2.0 authentication
- OTP email verification
- Multi-user profile management
- Secure data encryption

---

## 🛠️ Tech Stack

### **Frontend**
- **React 18.2** - Modern UI library with hooks
- **Redux Toolkit** - State management
- **Tailwind CSS** - Utility-first styling
- **React Router v6** - Client-side routing

### **Backend**
- **Python 3.8+**
- **Flask 2.3** - Lightweight web framework
- **MongoDB** - NoSQL database for flexible data models
- **OpenAI GPT-4o** - AI coaching intelligence
- **JWT** - Secure authentication

### **Deployment**
- **Vercel** - Frontend hosting
- **Railway/Docker** - Backend containerization
- **Git** - Version control

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────┐
│                   React Frontend                     │
│  ┌──────────────┐  ┌──────────────┐  ┌───────────┐ │
│  │   Dashboard  │  │   AI Chat    │  │  Rewards  │ │
│  │   (Parent)   │  │   (Child)    │  │  System   │ │
│  └──────┬───────┘  └──────┬───────┘  └─────┬─────┘ │
└─────────┼──────────────────┼─────────────────┼──────┘
          │                  │                 │
          └──────────────────┼─────────────────┘
                             ▼
          ┌─────────────────────────────────────┐
          │        Flask REST API Server        │
          │  ┌────────────┐  ┌───────────────┐ │
          │  │   Auth     │  │   AI Coach    │ │
          │  │  Service   │  │   (GPT-4o)    │ │
          │  └─────┬──────┘  └───────┬───────┘ │
          └────────┼──────────────────┼─────────┘
                   ▼                  ▼
          ┌────────────────┐  ┌──────────────┐
          │    MongoDB     │  │  OpenAI API  │
          │   Database     │  │              │
          └────────────────┘  └──────────────┘
```

---

## 🚀 Installation

### Prerequisites
- Node.js 16+ and npm
- Python 3.8+
- MongoDB instance
- OpenAI API key

### Backend Setup

```bash
# Clone the repository
git clone https://github.com/bhavanareddy19/AiDIY.git
cd AiDIY

# Install Python dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Add your OpenAI API key and MongoDB connection string

# Run the Flask server
python app.py
```

Server will be available at `http://localhost:5000`

### Frontend Setup

```bash
# Navigate to client directory
cd client

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Configure API endpoint

# Start development server
npm start
```

Application will open at `http://localhost:3000`

---

## 💡 Usage

### For Parents

1. **Create Account** - Sign up with email verification
2. **Add Children** - Create profiles for your kids
3. **Set Up Chores** - Assign tasks with reward amounts
4. **Monitor Progress** - Track savings, goals, and achievements
5. **Approve Transactions** - Review and approve spending requests

### For Children

1. **Talk to AI Coach** - Ask questions about money management
2. **Complete Chores** - Earn money through assigned tasks
3. **Set Goals** - Create savings goals for desired items
4. **Track Progress** - Watch savings grow and achievements unlock
5. **Learn & Play** - Complete challenges and earn badges

---

## 📸 Demo

### Parent Dashboard
*[Add screenshot of parent dashboard]*

### AI Coach Interface
*[Add screenshot of AI coach chat]*

### Child's Goal Tracker
*[Add screenshot of goal tracking]*

---

## 🎓 Technical Highlights

### What Makes This Project Stand Out

1. **AI Integration**
   - Real-world application of GPT-4o
   - Multi-modal AI interactions (text, voice, image)
   - Personalized learning algorithms

2. **Full-Stack Development**
   - Modern React frontend with Redux
   - RESTful API design with Flask
   - MongoDB schema design for flexibility

3. **User Experience Design**
   - Age-appropriate UX for children
   - Intuitive parent dashboard
   - Gamification psychology principles

4. **Security Best Practices**
   - OAuth 2.0 and JWT authentication
   - Email verification system
   - Secure parent-child access controls

5. **Scalable Architecture**
   - Microservices-ready design
   - Cloud deployment (Vercel + Railway)
   - Docker containerization

---

## 🗺️ Roadmap

### Version 1.0 (Current)
- ✅ AI financial coach with GPT-4o
- ✅ Parent and child dashboards
- ✅ Chore and reward system
- ✅ Goal tracking and savings
- ✅ Email notifications

### Version 2.0 (Planned)
- [ ] Mobile app (iOS and Android)
- [ ] Multi-language support
- [ ] Advanced analytics and insights
- [ ] Integration with real bank accounts (with parental controls)
- [ ] Social features (friend challenges, group goals)
- [ ] Enhanced AI capabilities (budget recommendations, spending analysis)

---

## 🧪 Testing

```bash
# Run backend tests
pytest tests/

# Run frontend tests
cd client && npm test
```

---

## 📁 Project Structure

```
AiDIY/
├── api/                    # API endpoints
│   ├── auth/              # Authentication routes
│   ├── coach/             # AI coach endpoints
│   └── user/              # User management
├── client/                # React frontend
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/         # Page components
│   │   ├── redux/         # State management
│   │   └── utils/         # Utility functions
│   └── public/            # Static assets
├── server/                # Flask backend
│   ├── models/            # Database models
│   ├── services/          # Business logic
│   └── utils/             # Helper functions
├── templates/             # HTML templates
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
└── Procfile              # Deployment configuration
```

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** - see the LICENSE file for details.

---

## 👤 Author

**Bhavana Reddy**

- GitHub: [@bhavanareddy19](https://github.com/bhavanareddy19)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/YOUR_PROFILE)

---

## 🙏 Acknowledgments

- OpenAI for GPT-4o API
- React and Flask communities
- All contributors and testers

---

<div align="center">

**Making financial literacy fun, one child at a time! 💰🎯**

[⬆ Back to Top](#-aidiy---ai-powered-financial-literacy-for-kids)

</div>
