 # 🎓 Lurnio – Learning Management System
<br/>
Lurnio is a MERN-stack Learning Management System designed to manage online courses, user access, and enrollments through a modern and responsive web interface.Built using React, Node.js, Express, and MongoDB with Clerk authentication and Stripe payments, enabling educators to publish courses and students to securely enroll and learn online.
<br/>

 ## 🌐 Live Demo(DEPLOYED):<br/>
https://lurnio-web-client.vercel.app/
 <br/>

 ## 🚀  Features

<br/>
•Secure authentication and role-based access using Clerk
<br/>
•Educator-driven course creation and management
<br/>
•Student enrollment, payments, and online course consumption
<br/>
•Stripe-powered secure checkout for paid courses
<br/>
•Structured learning with chapters, lectures, and free previews
<br/>
•Personalized My Enrollments and Educator Dashboard
<br/>
•Responsive, high-performance user interface
<br/>
•Scalable RESTful API backend
<br/>

## 🛠 Tech Stack
<br/>
Frontend: React.js (Vite), JavaScript (JSX), Tailwind CSS
<br/>
Backend: Node.js, Express.js
<br/>
Database: MongoDB (Mongoose)
<br/>
Authentication: Clerk (secure user login & role management)
<br/>
Payments: Stripe (course checkout & enrollment)
<br/>
Architecture: RESTful APIs, role-based access control
<br/>
Deployment: Vercel
<br/>

## ⚙️ Installation & Setup

 1. Clone the repository
```bash
git clone https://github.com/vattimillidivyasree/lurnio-lms.git
cd lurnio-lms
```

2. 🔐 Environment Variables on server side
<br/>
Create a `.env` file inside the server folder with the following variables: 

```bash
# Currency
CURRENCY=USD

# MongoDB Setup
MONGODB_URI=your_mongodb_uri

# Cloudinary Setup
CLOUDINARY_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key

# Clerk Setup 
CLERK_WEBHOOK_SECRET=your_clerk_webhook_secret 
CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key 
CLERK_SECRET_KEY=your_clerk_secret_key

# Stripe Setup 
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret 
STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
STRIPE_SECRET_KEY=your_stripe_secret_key
```
3.🔐 Environment Variables on client side
<br/>
Create a `.env` file inside the client folder with the following variables: 

```bash
VITE_CLERK_PUBLISHABLE_KEY="----- Clerk Publishable Key -----"
VITE_BACKEND_URL = 'http://localhost:5000'
VITE_CURRENCY = '$'
```
4.Start the backend server and run the frontend client:
```bash
npm install
npm run dev
```

## 📋 Prerequisites <br/><br/>

• Node.js (v18 or higher recommended) <br/>
• npm or yarn package manager <br/>
• MongoDB (local or MongoDB Atlas) <br/>
• Clerk account for authentication <br/>
• Stripe account for payments <br/>
• Cloudinary account for media storage <br/>
• Vercel account for deployment <br/>
• Modern web browser (Chrome / Edge / Firefox) <br/>

## 📦 Dependencies <br/><br/>

### 🎨 Frontend <br/>

- `@clerk/clerk-react` : `^5.17.1` <br/>
- `axios` : `^1.7.8` <br/>
- `humanize-duration` : `^3.32.1` <br/>
- `quill` : `^2.0.3` <br/>
- `rc-progress` : `^4.0.0` <br/>
- `react` : `^18.3.1` <br/>
- `react-dom` : `^18.3.1` <br/>
- `react-router-dom` : `^7.0.1` <br/>
- `react-simple-star-rating` : `^5.1.7` <br/>
- `react-toastify` : `^10.0.6` <br/>
- `react-youtube` : `^10.1.0` <br/>
- `uniqid` : `^5.4.0` <br/>

### Backend <br/>
- `@clerk/express` : `^1.3.24` <br/>
- `bcrypt` : `^5.1.1` <br/>
- `cloudinary` : `^2.5.1` <br/>
- `cors` : `^2.8.5` <br/>
- `dotenv` : `^16.4.7` <br/>
- `express` : `^4.21.2` <br/>
- `jsonwebtoken` : `^9.0.2` <br/>
- `mongoose` : `^8.8.4` <br/>
- `multer` : `^1.4.5-lts.1` <br/>
- `stripe` : `^17.5.0` <br/>
- `svix` : `^1.42.0` <br/><br/>

### Development Tools <br/>
- `nodemon` : `^3.1.7` <br/>

## 🔄 Course Flow <br/><br/>

1. User Registration & Login <br/>
Users sign up or log in using Clerk authentication <br/><br/>

2. Course Browsing <br/>
Students browse all available courses and search by keywords <br/><br/>

3. Course Enrollment <br/>
Students enroll in paid courses using Stripe payment gateway <br/><br/>

4. Learning Access <br/>
Enrolled students can watch lectures, view chapters, and access free previews <br/><br/>

5. Educator Management <br/>
Educators create, upload, and manage courses via the dashboard <br/>

## 🔌 API Endpoints <br/><br/>

### Authentication <br/>
Authentication is handled via Clerk. <br/>
No custom login/register endpoints are implemented <br/>
### Courses <br/>
- GET `/api/courses` – Get all courses <br/>
- GET `/api/courses/:id` – Get course details <br/>
- POST `/api/courses` – Create a course (Educator) <br/><br/>

### Enrollments <br/>
- POST `/api/enroll` – Enroll in a course <br/>
- GET `/api/enrollments` – View my enrollments <br/><br/>

### Payments <br/>
- POST `/api/payment/checkout` – Stripe payment session <br/>

## 🧪 Testing <br/><br/>

- Test authentication flows (login & signup) <br/>
- Verify course creation and enrollment <br/>
- Test Stripe payments using test keys <br/>
- Check protected routes for role-based access <br/>
- Validate API responses using Postman <br/>

## 🛠️ Troubleshooting <br/><br/>

### Server Issues <br/>
- Ensure MongoDB URI is correct in `.env` <br/>
- Check if server port is already in use <br/><br/>

### Authentication Issues <br/>
- Verify Clerk API keys <br/>
- Check allowed origins in Clerk dashboard <br/><br/>

### Payment Issues <br/>
- Use Stripe test keys <br/>
- Confirm webhook secrets are correct <br/><br/>

### Frontend Issues <br/>
- Run `npm install` before starting client <br/>
- Ensure backend server is running <br/>

 ## 📈  Future Enhancements <br/><br/>
•Certificates of completion <br/>
•Advanced analytics for educators <br/>
•Enhanced payment workflows <br/>

 ## 📄  License <br/>
This project is licensed under the MIT License. <br/><br/>


## 🤝 Contributing <br/><br/>

Contributions are currently not accepted for this project. <br/>
This repository is maintained as a completed full-stack project for learning and portfolio purposes. <br/>

## 🙏 Acknowledgements <br/><br/>

- Clerk for authentication and user management <br/>
- Stripe for secure payment processing <br/>
- MongoDB for database services <br/>
- Cloudinary for media storage <br/>
- React & Node.js open-source community <br/>


# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.<br/>

Currently, two official plugins are available:<br/>

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh<br/>
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh<br/>
