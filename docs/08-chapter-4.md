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

![KidWay Wireframe](../images/KidWay_Wireframe.png)

### 4.3.2. Landing Page Mockup

El Mockup de alta fidelidad representa la interfaz final de KidWay, integrando todos los elementos de la identidad visual y la arquitectura de información definida previamente. Este diseño busca equilibrar la funcionalidad técnica con una experiencia de usuario (UX) intuitiva y reconfortante para los padres.

![KidWay Landing Page Mockup](../images/Mockup-Landing-Page.png)

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

**Wireframe 1: User Login** ![Wireframe 1](../images/WIREFRAME%201.png)  
*Secure authentication portal for parents, drivers, and school administrators.*

**Wireframe 2: Parent Dashboard** ![Wireframe 2](../images/WIREFRAME%202.png)  
*Main control panel for parents, displaying active services and quick child status.*

**Wireframe 3: Live Tracking Map** ![Wireframe 3](../images/WIREFRAME%203.png)  
*Real-time GPS interface showing the bus location and Estimated Time of Arrival (ETA).*

**Wireframe 4: Student Profile Management** ![Wireframe 4](../images/WIREFRAME%204.png)  
*Section dedicated to managing student information, emergency contacts, and medical notes.*

**Wireframe 5: Trip History** ![Wireframe 5](../images/WIREFRAME%205.png)  
*Detailed log of past routes, including timestamps for every pick-up and drop-off.*

**Wireframe 6: Driver Main Interface** ![Wireframe 6](../images/WIREFRAME%206.png)  
*Operational view for drivers with active route navigation and stop management.*

**Wireframe 7: Attendance Checklist** ![Wireframe 7](../images/WIREFRAME%207.png)  
*Digital student roster for real-time boarding and deboarding confirmation.*

**Wireframe 8: School Admin Overview** ![Wireframe 8](../images/WIREFRAME%208.png)  
*Global monitoring dashboard for schools to track multiple units and safety status.*

**Wireframe 9: Route Optimization** ![Wireframe 9](../images/WIREFRAME%209.png)  
*Administrative tool for creating nodes and optimizing transportation paths.*

**Wireframe 10: Incident Reporting** ![Wireframe 10](../images/WIREFRAME%2010.png)  
*Standardized form for reporting delays, mechanical issues, or behavior alerts.*

**Wireframe 11: Notification Settings** ![Wireframe 11](../images/WIREFRAME%2011.png)  
*Preferences for push notifications, SMS alerts, and email communication.*

**Wireframe 12: Analytics & Reports** ![Wireframe 12](../images/WIREFRAME%2012.png)  
*Fleet performance dashboard displaying completed trips, average attendance, and incident metrics.*

### **4.4.2. Web Applications Wireflow Diagrams**

The following wireflow diagram illustrates the navigational architecture and interaction logic of the **KidWay** platform. It details the journey from the initial authentication phase to the role-specific dashboards designed for Parents, Drivers, and School Administrators, ensuring a logical flow across all 12 core wireframes.


---

**Wireflow Diagram: System Interaction Logic** ![KidWay Wireflow](../images/DIAGRAMA_WIREFLOW.png)  

---

### **4.4.2. Web Applications Mock-ups**

The **KidWay** Mock-ups represent the high-fidelity phase of our product design. In this stage, we integrated our visual identity—including the **KidWay Blue** and **Sun Gold** palette—with the structural layouts previously defined. These designs focus on creating a trustworthy and modern experience, ensuring that every interface is not only functional but also emotionally reassuring for parents and school staff.

Key visual elements applied:
* **Color Psychology:** Use of deep blues to evoke trust and gold accents for visibility and energy.
* **Accessibility:** High-contrast text and standard font sizes for readability in mobile and web environments.
* **Micro-interactions:** Visual feedback for buttons and input fields to guide the user intuitively.

---

**Mock-up 1: User Login** ![Mock-up 1](../images/MOCKUP%201.png)  
*Final high-fidelity login screen with branding and security-focused UI.*

**Mock-up 2: Parent Dashboard** ![Mock-up 2](../images/MOCKUP%202.png)  
*Color-coded overview for parents with real-time status indicators.*

**Mock-up 3: Live Tracking Map** ![Mock-up 3](../images/MOCKUP%203.png)  
*Interactive map interface featuring custom bus markers and dynamic ETA cards.*

**Mock-up 4: Student Profile Management** ![Mock-up 4](../images/MOCKUP%204.png)  
*Detailed view for managing student profiles with intuitive data entry fields.*

**Mock-up 5: Trip History** ![Mock-up 5](../images/MOCKUP%205.png)  
*Data-rich historical log with a clean, organized layout for past route analysis.*

**Mock-up 6: Driver Main Interface** ![Mock-up 6](../images/MOCKUP%206.png)  
*Optimized night/day mode for drivers, prioritizing navigation and large touch targets.*

**Mock-up 7: Attendance Checklist** ![Mock-up 7](../images/MOCKUP%207.png)  
*High-contrast checklist for real-time student boarding and security verification.*

**Mock-up 8: School Admin Overview** ![Mock-up 8](../images/MOCKUP%208.png)  
*Administrative dashboard with fleet metrics and active trip monitoring.*

**Mock-up 9: Route Optimization** ![Mock-up 9](../images/MOCKUP%209.png)  
*Visual route builder for administrators to design and assign pickup points.*

**Mock-up 10: Incident Reporting** ![Mock-up 10](../images/MOCKUP%2010.png)  
*Urgent alert interface designed for quick reporting under high-stress situations.*

**Mock-up 11: Notification Settings** ![Mock-up 11](../images/MOCKUP%2011.png)  
*Customization panel for alerts, maintaining visual consistency with the mobile app.*

**Mock-up 12: Analytics & Reports** ![Mock-up 12](../images/MOCKUP%2012.png)  
*Comprehensive performance graphs and data tables for school management.*

### **4.4.3. Web Applications User Flow Diagrams**

The **User Flow Diagrams** for KidWay map out the precise logical paths that different users follow to achieve their objectives. These flows are designed to minimize friction and ensure that critical actions—such as emergency reporting or real-time tracking—are accessible within a maximum of three interactions.

We have prioritized the following three critical flows:

1.  **Parental Monitoring Flow:** Focuses on the security check and the immediate access to the live location of the student.
2.  **Driver Operational Flow:** Streamlines the attendance process and the synchronization of route data with the central server.
3.  **Administrator Oversight Flow:** Provides a top-down view of fleet status and the generation of automated safety reports.

---

**User Flow Diagram: Core Platform Interactions** ![User Flow](../images/USER_FLOW.png)  
*This diagram details the decision nodes and action paths for Parents, Drivers, and Administrators within the web ecosystem.*

---
## **4.5. Web Applications Prototyping**
## **4.6. Domain-Driven Software Architecture**
### **4.6.1. Design-Level EventStorming**
### **4.6.2. Software Architecture Context Diagram**
### **4.6.3. Software Architecture Container Diagrams**
### **4.6.4. Software Architecture Components Diagrams**
## **4.7. Object-Oriented Design Software**
### **4.7.1. Class Diagrams**
## **4.8. Database Design**
### **4.8.1. Database Diagrams**