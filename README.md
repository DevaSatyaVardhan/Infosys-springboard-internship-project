# Wellness Marketplace for Alternative Therapies
**Infosys Springboard Internship Project**

A comprehensive full-stack healthcare and wellness marketplace application that connects patients with healthcare practitioners while offering wellness products, smart scheduling, integrated AI chatbot assistance, and community features.

## 🚀 Key Features

* **User Roles & Dashboards:** Distinct dashboards for Patients and Practitioners.
* **Authentication & Security:** Secure login/registration using JWT (JSON Web Tokens) and role-based access control.
* **Telemedicine & Scheduling:** Integrated calendar features for booking and managing consultation sessions.
* **E-Commerce & Products:** Browse wellness products, add to cart/wishlist, and provide reviews.
* **AI Chatbot Integration:** Embedded AI assistant powered by Google Gemini AI for instant support.
* **Medical Data Integration:** Leverages public health APIs like the NPI Registry (National Provider Identifier CMS) and OpenFDA.
* **Notifications & Reminders:** Automated email notifications and session reminders using Spring Mail and cron jobs.
* **Community Q&A:** A platform for users to ask questions and interact.

## 🛠️ Tech Stack

### Frontend
- **Framework:** React.js
- **Styling:** Tailwind CSS
- **State Management:** Context API (Cart, Wishlist)
- **Other Features:** Responsive UI, dynamic routing, image handling.

### Backend
- **Framework:** Java Spring Boot
- **Database:** MySQL (Hibernate/JPA)
- **Security:** Spring Security with JWT
- **Build Tool:** Maven
- **Integrations:** Google Gemini AI API, OpenFDA API, NPI Registry API, JavaMailSender for Emails.

## 📂 Project Structure

```text
springboard/
├── demo-backend/       # Spring Boot Backend API
│   └── demo/           # Core Backend source code (src, pom.xml, configs)
├── demo-frontend/      # ReactJS Frontend Web Application
│   ├── public/         # Static assets
│   └── src/            # React UI components, pages, services, and contexts
└── .gitignore          # Git ignore configuration
```

## ⚙️ Setup & Installation

### Prerequisites
- Java 17+
- Node.js (v16+) & npm
- MySQL Server
- Maven (optional, wrapper included)

### 1. Backend Setup (Spring Boot)

1. Open the `demo-backend/demo` directory in your terminal.
2. Create a MySQL database named `demo` (or update the properties).
3. Set the necessary environment variables in your system or IDE. You can also define them in `application.properties`:
   - `DB_PASSWORD`: Your MySQL root password
   - `JWT_SECRET`: A secure Base64 encoded string
   - `gemini.api.key`: Your Google Gemini API Key
   - `spring.mail.username` & `spring.mail.password`: Your email and app password for notifications.
4. Run the backend server:
   ```bash
   mvn spring-boot:run
   ```
   *The backend will start on `http://localhost:8080` (or the port defined in properties).*

### 2. Frontend Setup (React)

1. Open the `demo-frontend` directory in your terminal.
2. Install the necessary dependencies:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm start
   ```
   *The frontend will launch, typically accessible at `http://localhost:3000`.*

## 🔗 External APIs Used
- **Google Gemini API:** Smart Chatbot and recommendations.
- **CMS NPI Registry:** Practitioner verification and details.
- **OpenFDA:** Medication and drug label data.

## 📝 License
This project was developed as part of the Infosys Springboard Internship program.
