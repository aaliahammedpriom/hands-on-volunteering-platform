# HandsOn Volunteering Platform

## 📌 Project Overview
**HandsOn** is a community-driven social volunteering platform designed to connect individuals with meaningful social impact opportunities. Users can discover and join volunteer-driven events, post requests for community help, form teams for large-scale initiatives, and track their impact. The platform encourages social responsibility, collaboration, and recognition of contributions.

---

## 📚 Git Repositories
- **[Client Repository](https://github.com/aaliahammedpriom/hands-on-volunteering-platform-client)**
- **[Server Repository](https://github.com/aaliahammedpriom/hands-on-volunteering-platform-server)**

---

## 🛠 Technologies Used
### Frontend:
- **React.js**
- **Tailwind CSS**
- **DaisyUI**

### Routing:
- **React Router**

### Forms:
- **React Hook Form**

### Icons:
- **Lucide React**

### API Requests:
- **Axios**

### Authentication:
- **JWT & Firebase**

---

## ✨ Features

### **Client-Side Features:**
- User registration and profile management
- Browse, filter, and join volunteer events
- Create and manage community help requests
- One-click event registration
- Team formation for large-scale initiatives (Bonus)
- Volunteer impact tracking with leaderboards (Bonus)

### **Server-Side Features:**
- User authentication and authorization (JWT & Firebase)
- CRUD operations for user profiles, posts, and events
- Efficient data handling with MongoDB

---

## 📊 Database Schema

### **Users**:
Stores user profiles, skills, and supported causes

### **Events**:
Contains event details, participants, and categories

### **Requests**:
Tracks community help requests and responses

### **Teams (Bonus)**:
Manages public and private team memberships

### **Impact Logs (Bonus)**:
Records volunteer hours and contributions

---

## ⚙️ Setup Instructions

### Client Setup:
 Clone the client repository:
   ```bash
   git clone https://github.com/aaliahammedpriom/hands-on-volunteering-platform-client.git
   cd hands-on-client
   ```

Install dependencies:
   ```bash
   npm install
   ```

Configure environment variables: Create a .env file in the root directory and add your Firebase configuration details:
   ```plaintext
   VITE_API_KEY=your-api-key
   VITE_AUTH_DOMAIN=your-auth-domain
   VITE_PROJECT_ID=your-project-id
   VITE_STORAGE_BUCKET=your-storage-bucket
   VITE_MESSAGING_SENDER_ID=your-messaging-sender-id
   VITE_APP_ID=your-app-id
   ```

Run the development server:
   ```bash
   npm run dev
   ```

### Server Setup:
Clone the server repository:
   ```bash
   git clone https://github.com/aaliahammedpriom/hands-on-volunteering-platform-server.git
   cd handson-server
   ```

Install dependencies:
   ```bash
   npm install
   ```

Configure environment variables: Create a .env file in the root directory and add the required credentials:
   ```plaintext
   DB_USER=your_DB_USER
   DB_PASS=your_DB_PASS
   ACCESS_TOKEN=your_ACCESS_TOKEN
   ```

Run the development server:
   ```bash
   nodemon
   ```

---

## 🔗 API Documentation

### **User Authentication**
- `POST /jwt` – Generate JWT token
- `POST /users` – Register a new user
- `GET /users/:uid` – Get user details by UID
- `GET /users` – Search users by email
- `GET /user/:email` – Get user details by email
- `PATCH /update/:uid` – Update user details
- `PATCH /users/log` – Increment user log count

### **Events**
- `POST /events` – Create a new event
- `GET /events` – Fetch all events (supports filtering by location, category, and availability)
- `GET /events/user/:uid` – Fetch events created by a user
- `GET /events/:id` – Get event details by ID

### **Community Help Requests**
- `POST /communityhelp` – Create a new help request
- `GET /communityhelp` – Fetch all community help requests (supports filtering by location, urgency, and availability)
- `POST /communityhelpmessage` – Send a message related to a community help request
- `GET /communityhelpmessage/:creator` – Fetch messages sent to a community help request creator

### **Contributions**
- `POST /contribution` – Join a contribution
- `GET /contribution` – Fetch all contributions
- `GET /contribution/user/:uid` – Fetch contributions by a specific user

### **Teams**
- `POST /team` – Create a new team
- `GET /team` – Fetch all teams (supports leaderboard sorting)
- `GET /teamowner` – Fetch teams owned by a user
- `GET /teamdetails` – Fetch team details by ID

### **Team Requests**
- `POST /teamrequest` – Send a team join request
- `PATCH /teamrequest` – Update team join request status
- `GET /teamrequest/:id` – Fetch approved team requests by team ID

### **Team Discussions**
- `POST /teamdiscussion` – Create a discussion post in a team
- `GET /teamdiscussion/:id` – Fetch discussion posts by team ID

---

## 🚀 Running the Project

### Locally:
To run both client and server locally, follow the setup instructions for both and run:
   ```bash
   # For Client:
   npm run dev

   # For Server:
   nodemon
   ```

### Production Build:
To build the production version:
   ```bash
   # For Client:
   npm run build
   ```
The build files will be generated in the `dist/` folder and can be deployed to a hosting service of your choice.

---

## 💟 Contributions are welcome!
If you'd like to improve HandsOn, feel free to submit a pull request. 🎉

---


**Happy Volunteering!** 🌍🤝

