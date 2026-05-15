# **Chapter IV: Product Design**
## **4.1. Style Guidelines**
### 4.1.1. General Style Guidelines

The visual identity of **KidWay** is built on trust, safety, and modern efficiency. We aim to provide parents with peace of mind through a clean and friendly interface.

| Attribute | Description | Goal |
| :--- | :--- | :--- |
| **Personality** | Trustworthy, tech-savvy, and friendly. | To reduce parental anxiety regarding school transit. |
| **Shapes** | Rounded corners and organic lines. | To create a soft, non-intimidating user experience. |
| **Typography** | Montserrat / Sans Serif family. | To ensure high legibility on mobile and web screens. |

#### Color Palette
| Sample | Color | Hex Code | Primary Usage |
| :---: | :--- | :--- | :--- |
| 🔵 | **KidWay Blue** | `#1A4F8B` | Logo, headings, and primary buttons (Trust). |
| 🟡 | **Sun Gold** | `#FFB800` | Routes, sun icons, and highlights (Safety/Energy). |
| 🔘 | **Soft Gray** | `#F2F2F2` | Background sections to reduce eye strain. |

### 4.1.2. Web Style Guidelines

These rules ensure the platform remains consistent and easy to use across all browsers:

| Component | Visual Style | Purpose |
| :--- | :--- | :--- |
| **Buttons** | "Pill" shape (50px border-radius). | Makes the UI look modern and touch-friendly. |
| **Shadows** | Soft, subtle drop shadows. | To make important info (like Route Status) "pop" out. |
| **Spacing** | Generous whitespace. | To avoid clutter and help users focus on key data. |
| **Transitions** | Smooth hover effects on buttons. | To provide immediate feedback to the user. |

## **4.2. Information Architecture**
### 4.2.1. Organization Systems

Information is grouped logically based on the user's specific needs:

| User Role | Primary Focus | Org. Logic |
| :--- | :--- | :--- |
| **Parents** | Real-time child location & ETA. | Hierarchical (General to specific). |
| **Drivers** | Route list and pickup points. | Sequential (Step-by-step journey). |
| **Schools** | Fleet overview and safety reports. | Matrix (Summary of multiple data points). |

### 4.2.2. Labeling Systems

We use clear, empathetic language to guide the user without technical jargon:

| Label | Meaning to the User |
| :--- | :--- |
| **Live Route** | View the bus moving on the map right now. |
| **Guardian Mode** | Security settings for child monitoring. |
| **Route Status** | Quick update on pickup or arrival progress. |
| **Request Demo** | For schools to test the platform before joining. |

### 4.2.3. SEO Tags and Meta Tags

To ensure KidWay is easily found by schools and parents on Google:

| Tag Type | Content Example |
| :--- | :--- |
| **Title** | KidWay | Smart School Mobility & Real-Time Tracking |
| **Description** | Helping families keep every school route predictable and safe. |
| **Keywords** | School bus tracker, student safety, KidWay app, Lima mobility. |

### 4.2.4. Searching Systems

The search functionality in KidWay is not just a text box; it is a multi-layered system designed for high-stress situations where parents or administrators need information instantly.

* **Predictive Student Search:** We implemented an "Autocomplete" feature that queries the database in real-time as the user types. This is essential for parents with multiple children or school coordinators managing hundreds of students.
* **Filter-Based Discovery:** To avoid information overload, the system allows users to "Search by State." For example, an administrator can filter for "Delayed" units to focus only on vehicles currently facing issues in traffic.
* **Geographical Search:** Users can search for specific "Nodes" or "Pickup Points" on the map. By entering an address, the system identifies the nearest active route, facilitating the onboarding of new students.
* **Search Results Prioritization:** The system is programmed to show "Active" alerts first in search results, ensuring that urgent information is never buried under historical data.

### 4.2.5. Navigation Systems

KidWay’s navigation is designed to minimize "cognitive load," ensuring that even users who are not tech-savvy can find their way around the platform within seconds.

* **Primary Navigation (Global):** The header acts as the main anchor, providing access to public-facing information. We kept it minimalist to ensure the "Login" and "Sign Up" actions are the most prominent elements for new users.
* **Secondary Navigation (Dashboard):** Once logged in, the user encounters a "Sidebar" or "Tab Bar" (on mobile) that provides access to the Live Map, Trip History, and Profile Settings. 
* **Action-Driven Navigation:** We use "Call to Action" (CTA) buttons as navigational shortcuts. For instance, a "View Live Route" button appears on the home screen only when a trip is active, bypassing three steps of traditional menu navigation.
* **Feedback Loops:** The navigation system includes "Breadcrumbs," allowing users to see their path (e.g., Home > History > Route April 26) and return to previous states without using the browser's back button.

## **4.3. Landing Page UI Design**

### 4.3.1. Landing Page Wireframe
El wireframe de nuestra Landing Page se enfoca en una estructura de "Confianza Primero". Utilizamos un diseño que guía la vista del usuario desde la propuesta de valor hacia la evidencia social.

* **Hero Section:** Diseñada con un titular de alto impacto a la izquierda y un espacio dedicado para la identidad visual de KidWay (el escudo) a la derecha.
* **Sección de Métricas:** Ubicada estratégicamente debajo del hero para validar la fiabilidad del sistema con datos reales (segmentos, flujos y experiencia de confianza).

![KidWay Wireframe](../assets/chapter-4/KidWay_Wireframe.png)

### 4.3.2. Landing Page Mockup

El Mockup de alta fidelidad representa la interfaz final de KidWay, integrando todos los elementos de la identidad visual y la arquitectura de información definida previamente. Este diseño busca equilibrar la funcionalidad técnica con una experiencia de usuario (UX) intuitiva y reconfortante para los padres.

![KidWay Landing Page Mockup](../assets/chapter-4/Mockup-Landing-Page.png)

#### Análisis del Diseño Final:

El diseño se divide en bloques estratégicos para guiar al usuario a través del embudo de conversión:

| Sección | Descripción del Diseño | Propósito UX |
| :--- | :--- | :--- |
| **Hero Section** | Uso de tipografía Sans Serif en azul marino y acentos amarillos. | Captar la atención inmediata y comunicar el beneficio principal: seguridad. |
| **Value Proposition** | Cuadrícula de tarjetas con iconos y descripciones breves. | Detallar los beneficios para familias y operadores de forma digerible. |
| **Service Cards** | Tarjetas con bordes redondeados y botones "Sign Up" claros. | Facilitar la elección del plan o servicio adecuado según el tipo de usuario. |
| **Social Proof** | Carrusel de testimonios sobre fondo azul institucional. | Generar confianza a través de la validación de otros usuarios y entrevistas. |
| **FAQ & Contact** | Sección de acordeones para preguntas y formulario limpio. | Resolver dudas comunes y proporcionar un canal directo de comunicación. |

#### Especificaciones Técnicas de la Interfaz:
* **Jerarquía Visual:** Se utiliza el patrón de lectura en "Z" para asegurar que los elementos clave (CTA) no pasen desapercibidos.
* **Micro-interacciones:** Los botones y campos de entrada poseen estados claros (hover/focus) para mejorar la respuesta del sistema.
* **Accesibilidad:** Contraste de colores verificado para garantizar que la información sea legible en diversas condiciones de iluminación.

## **4.4. Web Applications UX/UI Design**

### **4.4.1. Web Applications Wireframes**

The wireframes for the **KidWay** web application represent the structural foundation of our interface, focusing on functionality and the user’s journey. These low-fidelity designs allow us to validate the information hierarchy and ensure that parents, drivers, and administrators can navigate the platform with zero friction.

Our core design objectives include:
* **Safety-First Navigation:** Prioritizing real-time data and emergency alerts.
* **Operational Efficiency:** Minimizing the steps required for drivers to manage student attendance.
* **Consistency:** Maintaining a unified layout across all administrative and user modules.

---

**Wireframe 1: User Login** ![Wireframe 1](../assets/chapter-4/WIREFRAME%201.png)  
*Secure authentication portal for parents, drivers, and school administrators.*

**Wireframe 2: Parent Dashboard** ![Wireframe 2](../assets/chapter-4/WIREFRAME%202.png)  
*Main control panel for parents, displaying active services and quick child status.*

**Wireframe 3: Live Tracking Map** ![Wireframe 3](../assets/chapter-4/WIREFRAME%203.png)  
*Real-time GPS interface showing the bus location and Estimated Time of Arrival (ETA).*

**Wireframe 4: Student Profile Management** ![Wireframe 4](../assets/chapter-4/WIREFRAME%204.png)  
*Section dedicated to managing student information, emergency contacts, and medical notes.*

**Wireframe 5: Trip History** ![Wireframe 5](../assets/chapter-4/WIREFRAME%205.png)  
*Detailed log of past routes, including timestamps for every pick-up and drop-off.*

**Wireframe 6: Driver Main Interface** ![Wireframe 6](../assets/chapter-4/WIREFRAME%206.png)  
*Operational view for drivers with active route navigation and stop management.*

**Wireframe 7: Attendance Checklist** ![Wireframe 7](../assets/chapter-4/WIREFRAME%207.png)  
*Digital student roster for real-time boarding and deboarding confirmation.*

**Wireframe 8: School Admin Overview** ![Wireframe 8](../assets/chapter-4/WIREFRAME%208.png)  
*Global monitoring dashboard for schools to track multiple units and safety status.*

**Wireframe 9: Route Optimization** ![Wireframe 9](../assets/chapter-4/WIREFRAME%209.png)  
*Administrative tool for creating nodes and optimizing transportation paths.*

**Wireframe 10: Incident Reporting** ![Wireframe 10](../assets/chapter-4/WIREFRAME%2010.png)  
*Standardized form for reporting delays, mechanical issues, or behavior alerts.*

**Wireframe 11: Notification Settings** ![Wireframe 11](../assets/chapter-4/WIREFRAME%2011.png)  
*Preferences for push notifications, SMS alerts, and email communication.*

**Wireframe 12: Analytics & Reports** ![Wireframe 12](../assets/chapter-4/WIREFRAME%2012.png)  
*Fleet performance dashboard displaying completed trips, average attendance, and incident metrics.*

### **4.4.2. Web Applications Wireflow Diagrams**

The following wireflow diagram illustrates the navigational architecture and interaction logic of the **KidWay** platform. It details the journey from the initial authentication phase to the role-specific dashboards designed for Parents, Drivers, and School Administrators, ensuring a logical flow across all 12 core wireframes.


---

**Wireflow Diagram: System Interaction Logic** ![KidWay Wireflow](../assets/chapter-4/DIAGRAMA_WIREFLOW.png)  

---

### **4.4.2. Web Applications Mock-ups**

The **KidWay** Mock-ups represent the high-fidelity phase of our product design. In this stage, we integrated our visual identity—including the **KidWay Blue** and **Sun Gold** palette—with the structural layouts previously defined. These designs focus on creating a trustworthy and modern experience, ensuring that every interface is not only functional but also emotionally reassuring for parents and school staff.

Key visual elements applied:
* **Color Psychology:** Use of deep blues to evoke trust and gold accents for visibility and energy.
* **Accessibility:** High-contrast text and standard font sizes for readability in mobile and web environments.
* **Micro-interactions:** Visual feedback for buttons and input fields to guide the user intuitively.

---

**Mock-up 1: User Login** ![Mock-up 1](../assets/chapter-4/MOCKUP%201.png)  
*Final high-fidelity login screen with branding and security-focused UI.*

**Mock-up 2: Parent Dashboard** ![Mock-up 2](../assets/chapter-4/MOCKUP%202.png)  
*Color-coded overview for parents with real-time status indicators.*

**Mock-up 3: Live Tracking Map** ![Mock-up 3](../assets/chapter-4/MOCKUP%203.png)  
*Interactive map interface featuring custom bus markers and dynamic ETA cards.*

**Mock-up 4: Student Profile Management** ![Mock-up 4](../assets/chapter-4/MOCKUP%204.png)  
*Detailed view for managing student profiles with intuitive data entry fields.*

**Mock-up 5: Trip History** ![Mock-up 5](../assets/chapter-4/MOCKUP%205.png)  
*Data-rich historical log with a clean, organized layout for past route analysis.*

**Mock-up 6: Driver Main Interface** ![Mock-up 6](../assets/chapter-4/MOCKUP%206.png)  
*Optimized night/day mode for drivers, prioritizing navigation and large touch targets.*

**Mock-up 7: Attendance Checklist** ![Mock-up 7](../assets/chapter-4/MOCKUP%207.png)  
*High-contrast checklist for real-time student boarding and security verification.*

**Mock-up 8: School Admin Overview** ![Mock-up 8](../assets/chapter-4/MOCKUP%208.png)  
*Administrative dashboard with fleet metrics and active trip monitoring.*

**Mock-up 9: Route Optimization** ![Mock-up 9](../assets/chapter-4/MOCKUP%209.png)  
*Visual route builder for administrators to design and assign pickup points.*

**Mock-up 10: Incident Reporting** ![Mock-up 10](../assets/chapter-4/MOCKUP%2010.png)  
*Urgent alert interface designed for quick reporting under high-stress situations.*

**Mock-up 11: Notification Settings** ![Mock-up 11](../assets/chapter-4/MOCKUP%2011.png)  
*Customization panel for alerts, maintaining visual consistency with the mobile app.*

**Mock-up 12: Analytics & Reports** ![Mock-up 12](../assets/chapter-4/MOCKUP%2012.png)  
*Comprehensive performance graphs and data tables for school management.*

### **4.4.3. Web Applications User Flow Diagrams**

The **User Flow Diagrams** for KidWay map out the precise logical paths that different users follow to achieve their objectives. These flows are designed to minimize friction and ensure that critical actions—such as emergency reporting or real-time tracking—are accessible within a maximum of three interactions.

We have prioritized the following three critical flows:

1.  **Parental Monitoring Flow:** Focuses on the security check and the immediate access to the live location of the student.
2.  **Driver Operational Flow:** Streamlines the attendance process and the synchronization of route data with the central server.
3.  **Administrator Oversight Flow:** Provides a top-down view of fleet status and the generation of automated safety reports.

---

**User Flow Diagram: Core Platform Interactions** ![User Flow](../assets/chapter-4/USER_FLOW.png)  
*This diagram details the decision nodes and action paths for Parents, Drivers, and Administrators within the web ecosystem.*

---
## **4.5. Web Applications Prototyping**

<p style="text-align: justify;">
  This section presents the Domain-Driven Software Architecture of KidWay, structured through strategic and tactical design principles to manage the complexity of a digital school transport management platform. The system is organized into well-defined Bounded Contexts, each representing an independent business domain such as Identity & Access Management, User Profiles, Subscription & Payments, Fleet Management, Driver Management, Route Management, Student Management, Assignment Management, Real-Time Tracking, Trip Management, Attendance Tracking, Alerts & Notifications, Incident Management, Analytics & Reports, and Company Management. This architectural approach promotes modularity, scalability, maintainability, and clear ownership of responsibilities across the solution. Through the use of Context, Container, Component, and Class Diagrams, the architecture aligns business processes with technical implementation, ensuring that KidWay can evolve efficiently while supporting secure operations, route coordination, real-time visibility, attendance control, and reliable transport services for independent operators, transport companies, schools, and families.
</P>

### **4.6.1. Design-Level EventStorming**

- Identity & Access Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/identity-access-bounded-context.png" width="70%" alt="identity-access-bounded-context">
</p>

- User Profiles Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/user-profiles-bounded-context.png" width="70%" alt="user-profiles-bounded-context">
</p>

- Subscription & Payments Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/subscription-payments-bounded-context.png" width="70%" alt="subscription-payments-bounded-context">
</p>

- Dashboard Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/dashboard-bounded-context.png" width="70%" alt="dashboard-bounded-context">
</p>

- Fleet Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/fleet-management-bounded-context.png" width="70%" alt="fleet-management-bounded-context">
</p>

- Driver Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/driver-management-bounded-context.png" width="70%" alt="driver-management-bounded-context">
</p>

- Route Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/route-management-bounded-context.png" width="70%" alt="route-management-bounded-context">
</p>

- Student Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/student-management-bounded-context.png" width="70%" alt="student-management-bounded-context">
</p>

- Assignment Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/assignment-management-bounded-context.png" width="70%" alt="assignment-management-bounded-context">
</p>

- Real-Time Tracking Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/real-time-tracking-bounded-context.png" width="70%" alt="real-time-tracking-bounded-context">
</p>

- Trip Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/trip-management-bounded-context.png" width="70%" alt="trip-management-bounded-context">
</p>

- Attendance Tracking Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/attendance-tracking-bounded-context.png" width="70%" alt="attendance-tracking-bounded-context">
</p>

- Alerts & Notifications Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/alerts-notifications-bounded-context.png" width="70%" alt="alerts-notifications-bounded-context">
</p>

- Incident Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/incident-management-bounded-context.png" width="70%" alt="incident-management-bounded-context">
</p>

- Analytics & Reports Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/analytics-reports-bounded-context.png" width="70%" alt="analytics-reports-bounded-context">
</p>

- Company Management Bounded Context:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/event-storming/company-management-bounded-context.png" width="70%" alt="company-management-bounded-context">
</p>


### **4.6.2. Software Architecture Context Diagram**

- KidWay Context Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/context-diagram/context-diagram.png" width="70%" alt="context-diagram">
</p>

### **4.6.3. Software Architecture Container Diagrams**

- KidWay Container Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/container-diagram/container-diagram.png" width="70%" alt="container-diagram">
</p>

### **4.6.4. Software Architecture Components Diagrams**

- KidWay Web Application Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/web-application-component-diagram.png" width="70%" alt="web-application-component-diagram">
</p>

- Identity & Access Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/identity-access-component-diagram.png" width="70%" alt="identity-access-component-diagram">
</p>

- User Profiles Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/user-profiles-component-diagram.png" width="70%" alt="user-profiles-component-diagram">
</p>

- Subscription & Payments Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/subscription-payments-component-diagram.png" width="70%" alt="subscription-payments-component-diagram">
</p>

- Dashboard Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/dashboard-component-diagram.png" width="70%" alt="dashboard-component-diagram">
</p>

- Fleet Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/fleet-management-component-diagram.png" width="70%" alt="fleet-management-component-diagram">
</p>

- Driver Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/driver-management-component-diagram.png" width="70%" alt="driver-management-component-diagram">
</p>

- Route Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/route-management-component-diagram.png" width="70%" alt="route-management-component-diagram">
</p>

- Student Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/student-management-component-diagram.png" width="70%" alt="student-management-component-diagram">
</p>

- Assignment Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/assignment-management-component-diagram.png" width="70%" alt="assignment-management-component-diagram">
</p>

- Real-Time Tracking Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/real-time-tracking-component-diagram.png" width="70%" alt="real-time-tracking-component-diagram">
</p>

- Trip Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/trip-management-component-diagram.png" width="70%" alt="trip-management-component-diagram">
</p>

- Attendance Tracking Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/attendance-tracking-component-diagram.png" width="70%" alt="attendance-tracking-component-diagram">
</p>

- Alerts & Notifications Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/alerts-notifications-component-diagram.png" width="70%" alt="alerts-notifications-component-diagram">
</p>

- Incident Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/incident-management-component-diagram.png" width="70%" alt="incident-management-component-diagram">
</p>

- Analytics & Reports Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/analytics-reports-component-diagram.png" width="70%" alt="analytics-reports-component-diagram">
</p>

- Company Management Component Diagram:

<p align="center">
  <img src="../assets/chapter-4/software-architecture/components-diagram/company-management-component-diagram.png" width="70%" alt="company-management-component-diagram">
</p>

## **4.7. Object-Oriented Design Software**

<p style="text-align: justify;">
This section presents the object-oriented design of the KidWay platform through UML Class Diagrams that model the internal structure of the system. The diagrams define the main entities, attributes, methods, enumerations, and relationships required to support the business logic of each bounded context. Following Domain-Driven Design (DDD) principles, the software model is organized into sixteen functional domains, including identity management, user profiles, subscriptions, dashboard, fleet, drivers, routes, students, assignments, real-time tracking, trips, attendance, alerts, incidents, analytics, and company management. These diagrams provide a clear blueprint for software implementation, promote maintainability, and ensure consistency between business requirements and the technical architecture.
</p>

### **4.7.1. Class Diagrams**

- Identity & Access Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/identity-access-management-class-diagram.png" width="70%" alt="identity-access-class-diagram">
</p>

- User Profiles Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/user-profiles-class-diagram.png" width="70%" alt="user-profiles-class-diagram">
</p>

- Subscription & Payments Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/subscription-payments-class-diagram.png" width="70%" alt="subscription-payments-class-diagram">
</p>

- Dashboard Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/dashboard-class-diagram.png" width="70%" alt="dashboard-class-diagram">
</p>

- Fleet Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/fleet-management-class-diagram.png" width="70%" alt="fleet-management-class-diagram">
</p>

- Driver Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/driver-management-class-diagram.png" width="70%" alt="driver-management-class-diagram">
</p>

- Route Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/route-management-class-diagram.png" width="70%" alt="route-management-class-diagram">
</p>

- Student Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/student-management-class-diagram.png" width="70%" alt="student-management-class-diagram">
</p>

- Assignment Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/assignment-management-class-diagram.png" width="70%" alt="assignment-management-class-diagram">
</p>

- Real-Time Tracking Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/real-time-tracking-class-diagram.png" width="70%" alt="real-time-tracking-class-diagram">
</p>

- Trip Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/trip-management-class-diagram.png" width="70%" alt="trip-management-class-diagram">
</p>

- Attendance Tracking Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/attendance-tracking-class-diagram.png" width="70%" alt="attendance-tracking-class-diagram">
</p>

- Alerts & Notifications Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/alerts-notifications-class-diagram.png" width="70%" alt="alerts-notifications-class-diagram">
</p>

- Incident Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/incident-management-class-diagram.png" width="70%" alt="incident-management-class-diagram">
</p>

- Analytics & Reports Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/analytics-reports-class-diagram.png" width="70%" alt="analytics-reports-class-diagram">
</p>

- Company Management Class Diagram:

<p align="center">
  <img src="../assets/chapter-4/design-software/class-diagrams/company-management-class-diagram.png" width="70%" alt="company-management-class-diagram">
</p>

## **4.8. Database Design**

<p style="text-align: justify;">
This section defines the database design of the KidWay platform, focusing on the logical organization, persistence strategy, and data structure required to support the system functionalities. Based on the previously defined bounded contexts and object-oriented models, the database design ensures data integrity, scalability, traceability, and efficient access to operational information. It includes the identification of core entities, relationships, constraints, and storage considerations for modules such as users, subscriptions, fleets, vehicles, drivers, routes, students, trips, attendance, alerts, incidents, reports, and company records. The detailed database diagrams and relational implementation are presented in the following subsection.
</p>

### **4.8.1. Database Diagrams**

- KidWay Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/kidway-database-diagram.png" width="70%" alt="kidway-database-diagram">
</p>

- Identity & Access Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/identity-access-management-database-diagram.png" width="70%" alt="identity-access-management-database-diagram">
</p>

- User Profiles Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/user-profiles-database-diagram.png" width="70%" alt="user-profiles-database-diagram">
</p>

- Subscription & Payments Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/subscription-payments-database-diagram.png" width="70%" alt="subscription-payments-database-diagram">
</p>

- Dashboard Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/dashboard-database-diagram.png" width="70%" alt="dashboard-database-diagram">
</p>

- Fleet Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/fleet-management-database-diagram.png" width="70%" alt="fleet-management-database-diagram">
</p>

- Driver Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/driver-management-database-diagram.png" width="70%" alt="driver-management-database-diagram">
</p>

- Route Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/route-management-database-diagram.png" width="70%" alt="route-management-database-diagram">
</p>

- Student Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/student-management-database-diagram.png" width="70%" alt="student-management-database-diagram">
</p>

- Assignment Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/assignment-management-database-diagram.png" width="70%" alt="assignment-management-database-diagram">
</p>

- Real-Time Tracking Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/real-time-tracking-database-diagram.png" width="70%" alt="real-time-tracking-database-diagram">
</p>

- Trip Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/trip-management-database-diagram.png" width="70%" alt="trip-management-database-diagram">
</p>

- Attendance Tracking Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/attendance-tracking-database-diagram.png" width="70%" alt="attendance-tracking-database-diagram">
</p>

- Alerts & Notifications Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/alerts-notifications-database-diagram.png" width="70%" alt="alerts-notifications-database-diagram">
</p>

- Incident Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/incident-management-database-diagram.png" width="70%" alt="incident-management-database-diagram">
</p>

- Analytics & Reports Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/analytics-reports-database-diagram.png" width="70%" alt="analytics-reports-database-diagram">
</p>

- Company Management Database Diagram:

<p align="center">
  <img src="../assets/chapter-4/database-design/database-diagram/company-management-database-diagram.png" width="70%" alt="company-management-database-diagram">
</p>
