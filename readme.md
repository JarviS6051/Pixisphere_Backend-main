📸 Pixisphere Backend
Pixisphere is the backend system for an AI-powered photography marketplace designed to connect clients with photographers and studios seamlessly. This backend handles everything from user authentication to partner onboarding and inquiry management.

🚀 Tech Stack
Node.js with Express.js

MongoDB with Mongoose

JWT for authentication

Joi for input validation

Cloudinary for image upload handling

🔐 Features
1. Authentication & Role-Based Access
User registration and login with JWT

Roles: client, partner, admin

Role-based access control via custom middleware

2. Partner Onboarding & Admin Approval
Partners can submit detailed onboarding forms (personal + service details)

Admins can view, approve, or reject partner requests

3. Inquiry Management
Clients submit inquiries for services

Partners can:

View inquiries relevant to them

Respond with price, message, and availability

4. Portfolio Management (In Progress)
Portfolio schema defined

Endpoint to add items is under development

🧾 API Endpoints
Method	Endpoint	Role	Description
POST	/api/auth/signup	All	Register a new user
POST	/api/auth/login	All	Login and receive authentication token
POST	/api/partner/onboard	Partner	Submit onboarding form
GET	/api/admin/verifications	Admin	View all pending partner verifications
PUT	/api/admin/verify/:id	Admin	Approve or reject a partner request
POST	/api/inquiry	Client	Submit a new service inquiry
GET	/api/partner/getAllQueries	Partner	Get all relevant client inquiries
POST	/api/partner/responseToInquiry/:id	Partner	Respond to a specific client inquiry

📁 Project Structure
bash
Copy
Edit
/backend
│-- /controllers
│-- /routes
│-- /models
│-- /middlewares
│-- /config
│-- app.js
│-- .env
📦 Environment Variables
To run the project, create a .env file in the root directory with the following:

makefile
Copy
Edit
MONGODB_URI=
SECRET_KEY=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
🧪 API Testing
A Postman collection is available for all API endpoints. Please include this collection in your submission for easy testing and validation.

📊 Project Status
Feature	Status
Authentication	✅ Completed
Partner Onboarding	✅ Completed
Admin Verification	✅ Completed
Inquiry Management	✅ Completed
Portfolio Management	🛠 In Progress
PostgreSQL Integration	❌ Not Started
Admin Dashboard	❌ Not Started

For any questions or contributions, feel free to reach out or fork the repository!