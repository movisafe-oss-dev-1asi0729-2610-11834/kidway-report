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
| Repository        | Branch            | Commit Id | Commit Message                   | Commit Message Body                           | Committed on |
| ----------------- | ----------------- | --------- | -------------------------------- | --------------------------------------------- | ------------ |
| kidway-landing    | feature/wireframe | a1b2c3    | feat: add landing page wireframe | Initial structure and layout defined in Figma | 2026-04-10   |
| kidway-landing    | feature/content   | d4e5f6    | feat: add landing page content   | Added problem and solution sections text      | 2026-04-11   |
| kidway-landing    | feature/ux-flow   | g7h8i9    | feat: improve landing page flow  | Improved logical order of sections            | 2026-04-12   |

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
| Collaboration tools like Figma and Trello improved workflow visibility. |
| Early definition of the value proposition reduced future rework.        |
| Task distribution among members improved efficiency and accountability. |


## **5.3. Validation Interviews**

### **5.3.1. Interview Design**

### **5.3.2. Interview Recording**

### **5.3.3. Evaluations Based on Heuristics**

## **5.4. About-the-Product Video**
