# **Chapter V: Product Implementation, Validation & Deployment**
## **5.1. Configuration Management Software**
This section describes the tools, configurations, and conventions adopted by the team to ensure consistency, quality, and traceability throughout the lifecycle of the KidsOnWay product.
The implementation of configuration management practices enabled effective collaboration, proper version control, and a structured development process, ensuring that all components of the solution were aligned and maintainable.
### **5.1.1. Software Development Environment Configuration**
To support the development of the project, the team used a set of tools covering all stages of the software lifecycle:

GitHub: used as the main platform for version control and team collaboration.
Visual Studio Code: primary development environment for frontend and backend implementation.
Node.js: runtime environment used for backend development and dependency management.
Postman: used for testing and validating RESTful API endpoints.
Figma: used for UI/UX design and prototyping.
Google Chrome: used for testing and validating the responsive behavior of the frontend.

These tools enabled efficient integration between design, development, testing, and validation processes.
### **5.1.2. Source Code Management**
The project uses GitHub as its version control system. Separate repositories were created for each main component of the solution:

Landing Page
Backend (RESTful Web Services)
Frontend Web Application

The team adopted the GitFlow branching model to manage development efficiently:

main: contains the stable production version
develop: integrates ongoing development work
feature/*: branches for new features

Naming conventions:

feature/boarding-system
feature/route-management
release/v1.0.0
hotfix/login-fix

Additionally, the team applied Semantic Versioning (SemVer):

v1.0.0 → initial stable release
v1.1.0 → new features added
v1.1.1 → bug fixes

Commit messages follow the Conventional Commits standard
This approach ensures a clear and traceable development history.
### **5.1.3. Source Code Style Guide & Conventions**
To ensure code quality and maintainability, the team adopted standard coding conventions:

All code elements (variables, functions, classes) are written in English
camelCase for variables and functions
Modular code structure for better organization

The following style guides were considered:

Google HTML/CSS Style Guide
JavaScript/TypeScript best practices
Clean Code principles

User Stories and Acceptance Criteria were written using a structured format based on Gherkin to improve clarity and readability.
### **5.1.4. Software Deployment Configuration**
The deployment process for each system component is defined as follows:

Backend
Install dependencies using: npm install
Run the server using: npm start
Configure environment variables (e.g., port, database connection)
Frontend
Install dependencies using: npm install
Run the application using: npm run dev
Access the application via a web browser
Landing Page
Open the main HTML file or deploy it on a hosting service
Validate responsiveness across different devices

This configuration allows any team member to run and deploy the system consistently.
## **5.2. Landing Page, Services & Applications Implementation**

### **5.2.X. Sprint n**

#### **5.2.X.1. Sprint Planning n**

#### **5.2.X.2. Aspect Leaders and Collaborators**

#### **5.2.X.3. Sprint Backlog n**

#### **5.2.X.4. Development Evidence for Sprint Review**

#### **5.2.X.5. Execution Evidence for Sprint Review**

#### **5.2.X.6. Services Documentation Evidence for Sprint Review**

#### **5.2.X.7. Software Deployment Evidence for Sprint Review**

#### **5.2.X.8. Team Collaboration Insights during Sprint**

## **5.3. Validation Interviews**

### **5.3.1. Interview Design**

### **5.3.2. Interview Recording**

### **5.3.3. Evaluations Based on Heuristics**

## **5.4. About-the-Product Video**
