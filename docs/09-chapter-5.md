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

### **5.2.1. Sprint 1**

#### **5.2.1.1. Sprint Planning 1**
During Sprint 1, the team focused on defining the structure and initial design of the KidsOnWay Landing Page. The objective was to clearly communicate the value proposition and present the problem and solution to potential users.
| Sprint #                       | Sprint 1                                             |
| ------------------------------ | ---------------------------------------------------- |
| **Sprint Planning Background** | Definition and conceptual design of the Landing Page |
| **Date**                       | 2026-04-10                                           |
| **Time**                       | 07:00 PM                                             |
| **Location**                   | Virtual meeting via Google Meet                      |
| **Prepared By**                | Rudas Chavarria, Jose                                |
| **Attendees**                  | Team Members                                         |

Sprint Goal & User Stories
| Sprint Goal         | Description                                                                                                                                                                                                                                          |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Sprint 1 Goal       | Our focus is on designing a clear and structured Landing Page. We believe it delivers understanding of the product’s value to potential users. This will be confirmed when users can identify the problem and solution within the first interaction. |
| Sprint 1 Velocity   | 10 Story Points                                                                                                                                                                                                                                      |
| Sum of Story Points | 10                                                                                                                                                                                                                                                   |

#### **5.2.1.2. Aspect Leaders and Collaborators**
During this Sprint, the team worked on Landing Page design, UX structure, and content creation.
| Team Member           | GitHub Username | Wireframe Design | Content Writing | UX Structure |
| --------------------- | --------------- | ---------------- | --------------- | ------------ |
| Rudas , Jose          | jose-rudas      | L                | C               | L            |
| Higa, Alonso          | alonso-higa     | C                | L               | C            |
| Huaco, Luis           | luis-huaco      | C                | C               | C            |
| Paredes, Tomas        | tomas-paredes   | C                | C               | L            |
| Carlos, Ever          | ever-carlos     | C                | C               | C            |

#### **5.2.1.3. Sprint Backlog 1**
The Sprint Backlog focused on defining the structure and initial design of the Landing Page.
| User Story | Work-Item / Task Id | Title              | Description                                   | Estimation (Hours) | Assigned To | Status |
| ---------- | ------------------- | ------------------ | --------------------------------------------- | ------------------ | ----------- | ------ |
| LP-01      | T1                  | Define structure   | Identify main sections of Landing Page        | 4                  | Jose        | Done   |
| LP-02      | T2                  | Create wireframe   | Design low-fidelity prototype in Figma        | 6                  | Alonso      | Done   |
| LP-03      | T3                  | Write content      | Draft problem and solution texts              | 5                  | Luis        | Done   |
| LP-04      | T4                  | UX flow validation | Validate section order and user understanding | 3                  | Tomas       | Done   |
| LP-05      | T5                  | Internal review    | Review design and content consistency         | 2                  | Ever        | Done   |

#### **5.2.1.4. Development Evidence for Sprint Review**
During this Sprint, the team completed the conceptual design of the Landing Page.
| Repository        | Branch            | Committed on |
| ----------------- | ----------------- | ------------ |
| kidway-landing    | feature/chapter-4 | 2026-04-10   |
| kidway-landing    | feature/chapter-4 | 2026-04-11   |
| kidway-landing    | feature/chapter-4 | 2026-04-12   |

#### **5.2.1.5. Execution Evidence for Sprint Review**
During this Sprint, the team validated the structure and clarity of the Landing Page.
| Evidence Type   | Description                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------- |
| Wireframes      | Low-fidelity design showing layout                                                                 |
| UX validation   | Logical flow between sections                                                                      |
| Internal review | Feedback from team members                                                                         |

#### **5.2.1.6. Services Documentation Evidence for Sprint Review**
| Status                                                                   |
| ------------------------------------------------------------------------ |
| Not applicable. No RESTful services were implemented during this Sprint. |

#### **5.2.1.7. Software Deployment Evidence for Sprint Review**
| Status                                                          |
| --------------------------------------------------------------- |
| Not applicable. The Landing Page was still in the design phase. |

#### **5.2.1.8. Team Collaboration Insights during Sprint**
| Insight                                                                 |
| ----------------------------------------------------------------------- |
| The team successfully aligned research with design decisions.           |
| Collaboration tools like Figma improved workflow visibility.            |
| Early definition of the value proposition reduced future rework.        |
| Task distribution among members improved efficiency and accountability. |

### **5.2.2. Sprint 2**

#### **5.2.2.1. Sprint Planning 2**
Sprint Planning Background
| Item        | Detail                                                              |
| ----------- | ------------------------------------------------------------------- |
| Date        | 2026-04-10                                                          |
| Time        | 08:00 PM                                                            |
| Location    | Virtual meeting (Google Meet)                                       |
| Prepared By | Jose Rudas                                                          |
| Attendees   | Jose Rudas / Alonso Higa / Luis Huaco / Tomas Paredes / Ever Carlos |

#### **5.2.2.2. Aspect Leaders and Collaborators**
| Team Member   | GitHub Username | HTML Structure | CSS Styling | Content Integration | Responsive Design |
| ------------- | --------------- | -------------- | ----------- | ------------------- | ----------------- |
| Jose Rudas    | jose-rudas      | L              | C           | C                   | C                 |
| Alonso Higa   | alonsohiga      | C              | L           | C                   | C                 |
| Luis Huaco    | lhuaco          | C              | C           | L                   | C                 |
| Tomas Paredes | tparedes        | C              | C           | C                   | L                 |
| Ever Carlos   | evercarlos      | C              | C           | C                   | C                 |

#### **5.2.2.3. Sprint Backlog 2**
| User Story | Work-Item / Task | Description                     | Estimation (Hours) | Assigned To   | Status |
| ---------- | ---------------- | ------------------------------- | ------------------ | ------------- | ------ |
| US01       | T1               | Create HTML structure           | 4                  | Jose Rudas    | Done   |
| US14       | T2               | Implement boarding section UI   | 3                  | Alonso Higa   | Done   |
| US12       | T3               | Add student list section (mock) | 3                  | Luis Huaco    | Done   |
| -          | T4               | Integrate CSS styles            | 4                  | Alonso Higa   | Done   |
| -          | T5               | Basic responsiveness            | 3                  | Tomas Paredes | Done   |

#### **5.2.2.4. Development Evidence for Sprint Review**
| Repository   | Branch                 | Date       |
| ------------ | ---------------------- | ---------- |
| landing-page | feature/chapter-4      | 2026-04-11 |
| landing-page | feature/chapter-4      | 2026-04-12 |
| landing-page | feature/chapter-4      | 2026-04-13 |

#### **5.2.2.5. Execution Evidence for Sprint Review**
During this Sprint, the Landing Page became functional in the browser.
Users can navigate through:

Hero section
Problem section
Solution section
#### **5.2.2.6. Services Documentation Evidence for Sprint Review**
Not applicable. No backend services were implemented.
#### **5.2.2.7. Software Deployment Evidence for Sprint Review**
The Landing Page was tested locally using Live Server.
Steps performed:

Open project in VS Code
Run Live Server
Validate rendering in browser
#### **5.2.2.8. Team Collaboration Insights during Sprint**
The team improved coordination and task distribution. Frontend implementation required close collaboration between design and development. Communication became more efficient.

### **5.2.3. Sprint 3**

#### **5.2.3.1. Sprint Planning 3**
| Item        | Detail                                                              |
| ----------- | ------------------------------------------------------------------- |
| Date        | 2026-04-17                                                          |
| Time        | 08:00 PM                                                            |
| Location    | Virtual meeting (Google Meet)                                       |
| Prepared By | Jose Rudas                                                          |
| Attendees   | Jose Rudas / Alonso Higa / Luis Huaco / Tomas Paredes / Ever Carlos |

#### **5.2.3.2. Aspect Leaders and Collaborators**
| Team Member   | GitHub Username | UI Improvements | Animations | Content Refinement | UX Optimization |
| ------------- | --------------- | --------------- | ---------- | ------------------ | --------------- |
| Jose Rudas    | jose-rudas      | L               | C          | C                  | C               |
| Alonso Higa   | alonsohiga      | C               | L          | C                  | C               |
| Luis Huaco    | lhuaco          | C               | C          | L                  | C               |
| Tomas Paredes | tparedes        | C               | C          | C                  | L               |
| Ever Carlos   | evercarlos      | C               | C          | C                  | C               |

#### **5.2.3.3. Sprint Backlog 3**
| User Story | Work-Item / Task | Description                | Estimation (Hours) | Assigned To   | Status |
| ---------- | ---------------- | -------------------------- | ------------------ | ------------- | ------ |
| US18       | T1               | Add visual indicators      | 3                  | Jose Rudas    | Done   |
| US16       | T2               | Improve interaction design | 3                  | Alonso Higa   | Done   |
| -          | T3               | Add About section          | 4                  | Luis Huaco    | Done   |
| -          | T4               | Add Benefits section       | 3                  | Tomas Paredes | Done   |
| -          | T5               | Add animations             | 3                  | Alonso Higa   | Done   |

#### **5.2.3.4. Development Evidence for Sprint Review**
| Repository   | Branch                  | Date       |
| ------------ | ----------------------- | ---------- |
| landing-page | feature/chapter-4       | 2026-04-18 |
| landing-page | feature/chapter-4       | 2026-04-19 |
| landing-page | feature/chapter-4       | 2026-04-20 |

#### **5.2.3.5. Execution Evidence for Sprint Review**
New sections added:

About the product
Benefits
Improved UI and animations
#### **5.2.3.6. Services Documentation Evidence for Sprint Review**
Not applicable.
#### **5.2.3.7. Software Deployment Evidence for Sprint Review**
Landing Page tested in multiple browsers:

Chrome
Edge
#### **5.2.3.8. Team Collaboration Insights during Sprint**
The team achieved better design consistency. Collaboration between designers and developers improved significantly. UI decisions were made faster.

## **5.3. Validation Interviews**

### **5.3.1. Interview Design**

### **5.3.2. Interview Recording**

### **5.3.3. Evaluations Based on Heuristics**

## **5.4. About-the-Product Video**
