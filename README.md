# 📦 Inventory Management System

A full-featured **Inventory Management Backend API** built using **Node.js**, **Express.js**, and **MongoDB**, with secure **JWT authentication**.

---

## 🚀 Features

- ✅ User Signup & Login
- 🔐 JWT-based Authentication
- 🧾 CRUD operations on Products
- 📦 Product details: Name, Description, Price, Quantity
- 🧠 Middleware for route protection
- 🗂️ RESTful API structure

---

## 🛠️ Tech Stack

| Technology | Description                  |
|------------|------------------------------|
| Node.js    | Backend JavaScript runtime   |
| Express.js | Web framework for Node.js    |
| MongoDB    | NoSQL database                |
| Mongoose   | MongoDB object modeling tool |
| JWT        | Authentication with tokens   |

---

## 📁 Project Structure

inventory-system/
├── controllers/
│ ├── authController.js # Handles login/signup
│ └── productController.js # Handles product logic
├── middleware/
│ ├── authMiddleware.js # Middleware for role validation
│ └── verifyToken.js # JWT verification middleware
├── models/
│ ├── User.js # User schema
│ └── Product.js # Product schema
├── routes/
│ ├── authRoutes.js # /api/auth routes
│ └── productRoutes.js # /api/products routes
├── server.js # Entry point
├── .gitignore # Node modules ignored
├── package.json
└── README.md


---

## 🔐 Environment Variables

Create a `.env` file inside the `inventory-system/` folder:

MONGO_URI=mongodb+srv://<your-cluster-url>
JWT_SECRET=your_jwt_secret_key


---

## 🚦 How to Run the Project Locally

```bash
# Clone the repo
git clone https://github.com/acharyaraksha84/inventory_management.git

# Move into the project directory
cd inventory_management/inventory-system

# Install dependencies
npm install

# Run the server
node server.js

🧪 API Endpoints
Method	Endpoint	Description
POST	/api/auth/register	Register new user
POST	/api/auth/login	Login user
GET	/api/products	Get all products
GET	/api/products/:id	Get product by ID
POST	/api/products	Add a new product
PUT	/api/products/:id	Update a product
DELETE	/api/products/:id	Delete a product

📬 Contact
Author: Shriraksha P Acharya
🔗 GitHub: @acharyaraksha84

💡 License
This project is licensed under the MIT License.

✅ TODO (Optional Enhancements)
Add role-based user access (admin, manager)

Add pagination and filtering for products

Add image upload to products

Happy Coding 💻✨