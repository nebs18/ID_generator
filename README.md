# ID and Calling Card Generator

A web-based application for generating customizable IDs and Calling Cards with dynamic SVG templates.

## 🚀 Features

- Interactive web interface with live preview
- Dynamic SVG template editing
- Form-based input with real-time updates
- Template management (Upload, Edit, Delete)
- PDF export functionality
- Docker-ready deployment
- (Tentative) AI-powered SVG template generation

## 🛠️ Tech Stack

- **Backend:** Node.js
- **Frontend:** Vue.js
- **Database:** PostgreSQL
- **Deployment:** Docker

## 📁 Project Structure

```
src/
├── backend/
│   ├── config/             # Environment and database configuration
│   ├── controllers/        # API request handlers
│   ├── models/            # Database models
│   ├── routes/            # Express route definitions
│   ├── migrations/        # Database migrations
│   ├── app.js            # Main application entry point
│   ├── package.json
│   └── Dockerfile        # Backend container configuration
│
├── frontend/
│   ├── public/           # Static assets
│   ├── src/
│   │   ├── components/   # Reusable Vue components
│   │   ├── views/        # Page-level components
│   │   ├── App.vue      # Root Vue component
│   │   └── main.js      # Vue entry point
│   ├── package.json
│   └── Dockerfile       # Frontend container configuration
│
├── docker-compose.yml   # Multi-container orchestration
├── README.md
└── .gitignore
```

## 🚦 Getting Started

### Prerequisites

- Docker and Docker Compose
- Node.js (for local development)
- PostgreSQL

### Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd id-generator
```

2. Start the application using Docker:
```bash
docker-compose up --build
```

3. Access the application at `http://localhost:[port]`

## 💻 Development

### Backend Setup

1. Navigate to the backend directory:
```bash
cd src/backend
npm install
```

2. Set up environment variables:
```bash
cp .env.example .env
# Configure your environment variables
```

3. Run migrations:
```bash
npm run migrate
```

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd src/frontend
npm install
```

2. Start development server:
```bash
npm run serve
```

## 🔑 Key Features

### Template Management
- Upload SVG templates with customizable placeholders
- Edit existing templates through an intuitive interface
- Delete outdated templates
- (Tentative) AI-powered template generation using DeepSeek API

### Dynamic Editing
- Real-time preview of changes
- Form-based input system
- Automatic placeholder updates
- PDF export functionality

## 📝 Documentation

- [Vue.js Documentation](https://vuejs.org/guide/introduction.html)
- [Docker Documentation](https://docs.docker.com/)
- [DeepSeek API Documentation](https://platform.deepseek.com/)
