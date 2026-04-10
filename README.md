# 🛒 Full-Stack E-commerce Web Application (MERN Stack)

## 🧭 Project Overview
A MERN-based e-commerce application demonstrating complete e-commerce flows (auth → catalogue → cart → checkout) with MongoDB-backed data handling and a documented setup for local execution.

## ✨ Features
- User registration and sign-in
- Product catalogue and product details
- Search and category-based browsing (as implemented)
- Shopping cart workflow
- Admin operations (products/categories/orders) *(if configured in your current build)*
- Optional payment integration variables (Braintree)

## 🏗️ System Architecture
This repository follows a standard MERN separation:
- **Client:** React app (`/client`)
- **Server:** Express API (`server.js`) exposing `/api/*` routes
- **Database:** MongoDB via Mongoose
- **Auth:** JWT-based auth flow (configured via environment variables)

**Architecture flow (text):**  
`User → React Client → Express API (/api) → MongoDB`

## 🧰 Tech Stack
- **Frontend:** React (Create React App in `/client`)
- **Backend:** Node.js, Express
- **Database:** MongoDB, Mongoose
- **Auth:** JWT
- **Dev tooling:** Nodemon, Concurrently
- **Payments (optional):** Braintree

## ⚙️ Installation and Setup

### 1) Clone
```bash
git clone https://github.com/HamnaIqbal44/mern-ecommerce-master.git
cd mern-ecommerce-master
```

### 2) Install dependencies (backend + frontend)
```bash
npm install
cd client
npm install
cd ..
```

### 3) Configure environment variables
Create a `.env` file in the repo root:

```bash
MONGODB_URI=<YOUR_MONGODB_URI>
JWT_SECRET=<YOUR_JWT_SECRET>
BRAINTREE_MERCHANT_ID=<OPTIONAL>
BRAINTREE_PUBLIC_KEY=<OPTIONAL>
BRAINTREE_PRIVATE_KEY=<OPTIONAL>
```

Create `client/.env`:

```bash
REACT_APP_API_URL=<YOUR_API_URL>
```

### 4) Run locally (starts both servers)
```bash
npm run dev
```

> Backend defaults to port `5000` unless `PORT` is set; frontend runs via CRA defaults.  

## 🧪 Usage / Demo (reviewer quick test)
1. Start the app (`npm run dev`).
2. Register/login.
3. Browse products and add to cart.
4. Check admin flows (if configured).


### 👩‍🎓 Author
Hamna Iqbal

🎓 Final Year BS Software Engineering
📌 Project Domain: Software Engineering, Web Development
