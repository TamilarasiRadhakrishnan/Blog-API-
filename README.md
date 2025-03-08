# Blog-API-
Blog API 

Blog API with Comments & Likes
📌 Description
This is a Node.js Express API for a blogging platform, allowing users to create, read, update, and delete blog posts. It also includes features for adding comments and likes to posts. The backend uses Sequelize as the ORM with MySQL/PostgreSQL for database management.

🚀 Features
User Authentication (Signup, Login, JWT-based Authentication)
Create, Read, Update, Delete (CRUD) operations for blog posts
Comment System: Users can add, edit, and delete comments
Like System: Users can like/unlike blog posts
Sequelize ORM for database interactions
RESTful API design following best practices
🛠️ Tech Stack
Backend: Node.js, Express.js
Database: MySQL / PostgreSQL (Sequelize ORM)
Authentication: JSON Web Tokens (JWT)
Development Tools: GitHub Codespaces, Postman for API testing
📂 Folder Structure
bash
Copy
Edit
📁 blog-api  
 ┣ 📂 src  
 ┃ ┣ 📂 config       # Database configuration  
 ┃ ┣ 📂 controllers  # Handles request logic  
 ┃ ┣ 📂 middleware   # Authentication & authorization  
 ┃ ┣ 📂 models       # Sequelize models  
 ┃ ┣ 📂 routes       # API endpoints  
 ┃ ┣ app.js          # Express app setup  
 ┃ ┣ server.js       # Main entry point  
 ┣ package.json  
 ┣ README.md  
⚡ Installation & Setup
1️⃣ Clone the repository
sh
Copy
Edit
git clone https://github.com/TamilarasiRadhakrishnan/Blog-API-.git
cd blog-api
2️⃣ Install dependencies
sh
Copy
Edit
npm install
3️⃣ Configure the database
Set up MySQL/PostgreSQL
Update database settings in src/config/database.js
4️⃣ Run migrations (if using Sequelize)
sh
Copy
Edit
npx sequelize-cli db:migrate
5️⃣ Start the server
sh
Copy
Edit
node src/server.js
The API should be running on http://localhost:5000 (or your configured port).
🔥 API Endpoints
📌 Authentication
POST /api/auth/signup - User Signup
POST /api/auth/login - User Login
📌 Blog Posts
POST /api/posts - Create a new post
GET /api/posts - Get all posts
GET /api/posts/:id - Get a specific post
PUT /api/posts/:id - Update a post
DELETE /api/posts/:id - Delete a post
📌 Comments
POST /api/posts/:postId/comments - Add a comment
GET /api/posts/:postId/comments - Get comments
PUT /api/comments/:id - Update a comment
DELETE /api/comments/:id - Delete a comment
📌 Likes
POST /api/posts/:postId/like - Like a post
DELETE /api/posts/:postId/unlike - Unlike a post
📝 License
This project is licensed under the MIT License.

