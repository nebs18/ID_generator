#### Project Overview
- This project is a web based ID and Calling Card Generator Application. It will consist of modular functions for uploading ID or Calling Card templates in the form of SVG. The user is then presented with a form that they can fillup and the contents of the template will change dynamically. It will also feature uploading of SVG Templates, Editing the SVG Templats, and Downloading the Final Template as PDF. 
Tech Stack:
    - Backend: Node.js
    - Database: PostgreSQL (for storing templates and other data)
    - Frontend: Vue, HTML, CSS
    - Deployment: Dockerized local server

- It will be deployed on a local server.

#### Core Functionalities
1. Web Interface
- The project will have a comprehensive and interactive web interface wherein users can generate IDs or Calling Cards. They will also be able add, delete, modify, and download SVG templates.
- Interactive UI: Users generate IDs or Calling Cards with a live preview.
- Dynamic Editing: Form-based inputs update designated placeholders in the SVG template immediately.

2. CRUD Operations
- The project will feature the following operations:
    - Add SVG: Uploading of SVG Templates
    - Edit SVG: Direct editing of SVG Templates
    - Delete SVG: Deletion of SVG Templates
    - Create SVG: Interface for the creation and modification of SVG Templates. (tentative)
    - AI SVG Generation: Possible implementation of DeepSeeks free API calls for in built generation of SVG templates. (tentative)

3. Dockerized Deployment
- The project needs to be deployed and built with docker deployment in mind.

#### Documentation
- DeepSeek Documentation
- Vue Documentation
- Docker Documentation

#### Implementation Notes
- Template Placeholders:
SVG templates will include identifiable placeholders (e.g., <text id="namePlaceholder">[Name]</text>) for dynamic content.

- Vue Reactivity:
Vue's data binding will automatically update SVG content as users fill out the form, providing a smooth live preview.

- Modularity & Scalability:
The project structure allows independent development of each module, ensuring flexibility for future enhancements like AI generation.

#### Project Structure
src/
├── backend/
│   ├── config/             # Environment and database configuration
│   ├── controllers/        # API request handlers
│   ├── models/             # Database models (e.g., ORM definitions)
│   ├── routes/             # Express route definitions
│   ├── migrations/         # Database migrations (if using a tool like Sequelize)
│   ├── app.js              # Main application entry point
│   ├── package.json
│   └── Dockerfile          # Node.js backend container configuration
│
├── frontend/
│   ├── public/             # Static assets (HTML, favicon, etc.)
│   ├── src/
│   │   ├── components/     # Reusable Vue components (e.g., SVGEditor.vue)
│   │   ├── views/          # Page-level Vue components (e.g., Home.vue, Editor.vue)
│   │   ├── App.vue         # Root Vue component
│   │   └── main.js         # Vue entry point
│   ├── package.json
│   └── Dockerfile          # Vue app container configuration (optional)
│
├── docker-compose.yml      # Orchestrates multi-container deployment
├── README.md
└── .gitignore

#### User Stories
1. **Upload SVG Template**  
   *As an administrator, I want to upload SVG templates so that I can expand the library of available designs for IDs and calling cards.*

2. **Edit SVG Template**  
   *As a user, I want to edit an SVG template using a form-based interface so that my input dynamically updates the template in real time.*

3. **Delete SVG Template**  
   *As an administrator, I want to delete outdated or unused SVG templates so that the system remains organized and up-to-date.*

4. **Create a New ID/Calling Card**  
   *As a user, I want to select a template and customize it with my information so that I can generate a personalized and professional ID or calling card.*

5. **Download as PDF**  
   *As a user, I want to download my finalized ID or calling card as a PDF so that I can print or share it easily.*

6. **(Tentative) AI-Generated SVG Template**  
   *As a user, I want the option to generate a new SVG template using an AI tool so that I can quickly create unique designs for my ID or calling card.*