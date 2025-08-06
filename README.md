# 🩺 DrSmart – A Modern Healthcare Platform

**DrSmart** is a full-stack healthcare platform that facilitates appointment booking, visit tracking, and medical record sharing between patients and doctors. It features secure virtual appointments via Zoom and AI-powered health article suggestions personalized to each patient’s medical history.

> 🚧 **Note:** The project is currently under development. Live deployment coming soon. Please refer to the screenshots section for a visual overview.

---

## 🚀 Features

### 🧑‍⚕️ Doctor Features
- ✅ View all upcoming and past appointments  
- ✅ Confirm, cancel, or reject patient appointments  
- ✅ Set availability for patient bookings  
- ✅ Access patient visit history and medical records  
- ✅ Initiate Zoom calls for secure virtual consultations  

### 🧍 Patient Features
- ✅ Book appointments with available doctors  
- ✅ View past and upcoming visits  
- ✅ Share and review medical records and doctor’s notes  
- ✅ Join Zoom-based virtual appointments  
- ✅ Receive AI-powered health article recommendations  

---

## 📸 Screenshots

![Doctor's Dashboard](</screenshots/image-01.png>) *Doctor's Dashboard*  
![Selecting Schedule](</screenshots/image-02.png>) *Selecting Schedule*  
![Patient's Records](</screenshots/image-03.png>) *Patient's Records*  
![Appointment Management](</screenshots/image-04.png>) *Confirm/Cancel/Reject Appointments*  
![Virtual Call Session](</screenshots/image-05.png>) *Zoom Consultation*  
![Patient's Dashboard](</screenshots/image-06.png>) *Patient Portal*  
![Booking Appointment](</screenshots/image-07.png>) *Appointment Booking*  
![Notifications](</screenshots/image-08.png>) *Patient Notifications*  
![AI Suggestions](</screenshots/image-08.png>) *Health Article Recommendations*

---

## 🧱 Tech Stack

### 🔹 Frontend
- React 18
- Vite
- Ant Design
- Axios
- React Router DOM
- React Datepicker
- Zoom Video SDK

### 🔸 Backend
- Node.js + Express
- PostgreSQL
- dotenv
- puppeteer + cheerio (for scraping or article generation)
- socket.io (real-time features)
- helmet & cors (security)
- Zoom SDK integration
- RESTful API structure

### 🛠 Development Tools
- ESLint (with React & Hooks plugins)
- Sass (via `sass-embedded`)
- Vite plugin for React

---

## 🛠️ Getting Started

### 📦 Prerequisites

- Node.js (v18+)
- npm
- PostgreSQL

---

## 🔧 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/drsmart.git
cd drsmart
```

### 2. Set Up Environment Variables
Create a `.env` or `.env.development` file in `/backend/` with the following structure:
```bash
PGHOST=localhost
PGUSER=development
PGDATABASE=drsmart
PGPASSWORD=development
PGPORT=5432

OPENAI_API_KEY=sk-...
SDK_KEY=your_zoom_sdk_key
SDK_SECRET=your_zoom_sdk_secret
```
🚫 Replace placeholder values with your own credentials. Never commit this file to version control.

### 3. Install Dependencies

#### Backend
```bash
cd backend
npm install
```

#### Frontend
```bash
cd ../frontend
npm install
```

### 4. Set Up the Database
Ensure PostgreSQL is running. Then run the following script (from the `/backend` folder). If `npm run reset` is not available, manually run any schema/seed files provided::
```bash
npm run reset
```
This will:
- Create the schema (create.sql)
- Populate it with development data (development.sql)

### 5. Run the App
#### Backend
```bash
cd backend
npm start
```
#### Frontend
```bash
cd ../frontend
npm run dev
```
Visit http://localhost:5174 to use the app.
> 📌 If you're using Vite and the port is different, check your terminal output for the correct local URL.

---

## 📃 License
This project is licensed under the ISC License.

---

## Contributions
This project was developed by Fakeha Iftikhar, Bushra Patel, and Jorge Medina as the final group project of our Full Stack Web Development Bootcamp!

---

## 📬 Contact
For questions or collaborations, feel free to reach out via [email](mailto:fakeha.iftikhar@gmail.com) or [LinkedIn](https://www.linkedin.com/in/fakeha38/).
