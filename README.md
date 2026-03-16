# 🛒 Shopping Cart with Mongoose (Node.js)

A simple **Shopping Cart web application** built using **Node.js, Express.js and Mongoose**.

This project demonstrates how to build a basic e-commerce style application where users can view products, add them to a shopping cart, and manage orders.
The application uses **Mongoose (Object Data Modeling library)** to interact with MongoDB in a structured way using schemas and models.

---

# 🚀 Features

* Product listing
* Add products to cart
* Remove products from cart
* Update cart quantity
* Order creation
* Data stored using **Mongoose models**
* MVC-style project structure
* Server-side rendering using EJS

---

# 🧰 Tech Stack

### Backend

* Node.js
* Express.js

### Database Layer

* MongoDB
* **Mongoose ODM**

### Frontend

* EJS Templates
* HTML
* CSS

### Development Tools

* Nodemon

---

# 📂 Project Structure

```id="ffr9gk"
Shopping-Cart-with-Mongoose
│
├── controllers
│
├── models
│   ├── product.js
│   ├── user.js
│   └── order.js
│
├── routes
│
├── views
│
├── public
│
├── app.js
└── package.json
```

---

# ⚙️ Installation

### 1️⃣ Clone the repository

```id="xnd5i3"
git clone https://github.com/SP-9cloud/Shopping-Cart-with-Mongoose.git
```

---

### 2️⃣ Navigate to the project folder

```id="pkqlsg"
cd Shopping-Cart-with-Mongoose
```

---

### 3️⃣ Install dependencies

```id="93x0g7"
npm install
```

---

# 🗄️ Database Configuration

The application connects to MongoDB using **Mongoose**.

Example connection in `app.js`:

```javascript id="gcyqho"
const mongoose = require("mongoose");

mongoose.connect("mongodb://localhost:27017/shopping-cart")
  .then(() => {
    app.listen(3000);
  })
  .catch(err => console.log(err));
```

Mongoose is used to define **schemas and models** for application data.

Example model:

```javascript id="6sztxq"
const mongoose = require("mongoose");

const productSchema = new mongoose.Schema({
  title: String,
  price: Number,
  description: String
});

module.exports = mongoose.model("Product", productSchema);
```

---

# ▶️ Running the Application

Start the server:

```id="zfqndp"
npm start
```

or

```id="4qv2qf"
nodemon app.js
```

The application will run at:

```id="ut5ytg"
http://localhost:3000
```
---
