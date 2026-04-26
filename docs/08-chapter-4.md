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
### **4.4.2. Web Applications Wireflow Diagrams**
### **4.4.2. Web Applications Mock-ups**
### **4.4.3. Web Applications User Flow Diagrams**
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