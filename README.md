# FitnessHub - Gym Management & Review System

FitnessHub is a full-stack web application designed to bridge the gap between local fitness centers and enthusiasts. The platform allows users to discover, rate, and share experiences about gyms, while providing gym owners with a space to showcase their facilities.

**Live Demo:** [https://fitnesshub-woif.onrender.com](https://fitnesshub-woif.onrender.com)
P.S. - access to server services can be expired
---

## Technologies & Tools

### Frontend
* **HTML5 & CSS3:** Core structure and custom styling.
* **Bootstrap 5:** Responsive design and modern UI components.
* **JavaScript (ES6+):** Client-side logic and interactive elements.
* **MapTiler SDK:** Integration of interactive maps for gym geolocation.

### Backend
* **Node.js:** JavaScript runtime environment.
* **Express.js:** Web framework for building the RESTful API and handling routing.
* **EJS (Embedded JavaScript):** Server-side templating engine for dynamic content.
* **Passport.js:** Middleware for secure user authentication (Local Strategy).

### Database & Storage
* **PostgreSQL:** Relational database for storing user profiles, gym data, and reviews.
* **Cloudinary:** Cloud-based image management for gym photos.

### Deployment & Security
* **Render:** Cloud platform for hosting the application.
* **Helmet.js:** Security headers to protect against common web vulnerabilities.
* **Express-session & Cookies:** Session management and persistent login states.

---

##  System Architecture

The project follows the **MVC (Model-View-Controller)** design pattern to ensure clean code separation, scalability, and maintainability.

### Project Structure:
* `models/` – PostgreSQL data schemas (Users, Gyms, Reviews).
* `routes/` – Express routers for handling resource-specific endpoints.
* `controllers/` – Business logic and request handling.
* `views/` – Dynamic EJS templates.
* `public/` – Static assets (custom CSS, client-side JS, images).
* `middleware/` – Authentication guards and data validation logic.

---

##  Features & Functionality

### 1. User Authentication & Authorization
* Secure registration and login using **Passport.js**.
* Role-based access: Only authorized owners can modify or delete their gym listings.

### 2. Gym Management (CRUD)
* **Create:** Users can list fitness centers with descriptions, pricing, and images.
* **Read:** Detailed view of each gym, including photo galleries and location data.
* **Update/Delete:** Full control over user-owned content.

### 3. Interactive Review System
* Star rating system (1-5 stars).
* Comment section for community feedback.
* Real-time average rating calculation for each facility.

### 4. Geolocation & Maps
* **MapTiler API** integration for geocoding addresses into geographic coordinates.
* Interactive **Cluster Maps** for browsing gyms by region.

### 5. Security & Data Validation
* **Joi:** Schema-based validation for all incoming requests.
* **Sanitization:** Protection against XSS (Cross-Site Scripting) and SQL Injection.
* **Error Handling:** Centralized global error handling middleware.

---

##  Local Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Dniapro123/FitnessHub.git](https://github.com/Dniapro123/FitnessHub.git)
