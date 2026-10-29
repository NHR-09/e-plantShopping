# Paradise Nursery Shopping Application

Welcome to **Paradise Nursery**, where green meets serenity! This is a complete e-commerce shopping cart web application for an online houseplant nursery, developed using React and Redux Toolkit.

---

## Project Overview
**Project Name:** Paradise Nursery Shopping Application (`e-plantShopping`)  
**Course:** Developing Front-End Apps with React (Coursera / IBM)

Paradise Nursery allows users to browse through a diverse collection of indoor plants categorized by their unique benefits, inspect details, add plants to their shopping cart, dynamically update quantities, and calculate real-time totals.

---

## Key Features

### 1. Landing Page (`App.jsx`, `AboutUs.jsx`, `App.css`)
- Header featuring company name **Paradise Nursery** and tagline *"Where Green Meets Serenity"*.
- Atmospheric greenhouse background image styled in `App.css`.
- An **About Us** section providing insight into the company's commitment to nature, plant health, and sustainable living.
- Interactive **"Get Started"** button that smoothly transitions to the product catalog.

### 2. Navigation Bar (`ProductList.jsx`)
- Persistent navigation bar appearing on both the Product Catalog and Shopping Cart views.
- Direct navigation links: **Home**, **Plants**, and **Cart**.
- Dynamic shopping cart badge displaying the total quantity of items currently in the cart.

### 3. Product Catalog (`ProductList.jsx`)
- Over 30 unique houseplants organized across 5 distinct categories (minimum 6 plants per category):
  - **Air Purifying Plants**
  - **Aromatic Fragrant Plants**
  - **Insect Repellent Plants**
  - **Medicinal Plants**
  - **Low Maintenance Plants**
- Each plant card displays a high-resolution thumbnail image, plant name, description, and price.
- **"Add to Cart"** functionality:
  - Dispatches product to the Redux cart slice.
  - Dynamically increments the cart counter in the navbar.
  - Disables the button and marks it as *"Added to Cart"*.

### 4. Shopping Cart (`CartItem.jsx`, `CartSlice.jsx`)
- Displays all added plant items with thumbnail, name, unit cost, and line subtotal.
- Calculates and shows the overall **Total Cart Amount**.
- Increment (`+`) and Decrement (`-`) buttons to adjust quantities in real time.
- Decrementing below 1 or clicking the **Delete** button removes the item from the cart.
- **"Continue Shopping"** button returning to the product catalog.
- **"Checkout"** button displaying a "Coming Soon" prompt.

---

## State Management (`CartSlice.jsx`)
Built with Redux Toolkit:
- `addItem`: Adds an item to the cart or increments its quantity if already present.
- `removeItem`: Removes a product from the cart by name.
- `updateQuantity`: Adjusts item quantity directly.

---

## Technologies Used
- **React 18**
- **Redux Toolkit (`@reduxjs/toolkit`)**
- **React-Redux**
- **Vite**
- **HTML5 & CSS3**

---

## Getting Started

### Installation
```bash
npm install
```

### Running the Application
```bash
npm run dev
```

### Building for Production
```bash
npm run build
```
