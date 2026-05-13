# e-plantShopping
🌿 Paradise Nursery - Shopping Cart Application
A responsive React-based e-commerce application for an indoor plant nursery. This project demonstrates state management using Redux Toolkit, component-based architecture, and dynamic UI updates.

🚀 Features
Product Listing: Browse a wide variety of plants categorized by their benefits (Air Purifying, Aromatic, etc.).

Redux State Management: Uses a centralized store to track items added to the cart across different views.

Dynamic Cart functionality:

Add to Cart: Adds plants to the bag and disables the button once added.

Update Quantity: Increment or decrement item counts directly in the cart.

Smart Removal: Automatically removes items from the cart if the quantity reaches zero.

Subtotal & Total Calculation: Real-time calculation of costs based on quantity and unit price.

Responsive Navigation: A sticky navbar featuring a live cart quantity badge.

🛠️ Tech Stack
Frontend: React.js (Hooks, Functional Components)

State Management: Redux Toolkit & React-Redux

Styling: CSS3 (Flexbox & Grid)

Icons: SVG & CSS-based iconography

📂 Project Structure
Plaintext
src/
├── components/
│   ├── CartItem.jsx       # Shopping cart view and logic
│   ├── ProductList.jsx     # Product display and "Add to Cart" logic
├── store/
│   ├── store.js            # Redux store configuration
│   └── CartSlice.jsx       # Reducer logic and action creators
├── App.js                  # Main entry point
└── index.js                # React DOM rendering
📖 Key Redux Logic
Actions
addItem: Adds a plant object to the state or increments its quantity if it already exists.

removeItem: Deletes a plant from the state using item.name.

updateQuantity: Modifies the quantity property of a specific plant in the store.

Selectors
calculateTotalQuantity: A derived state function that reduces the cartItems array to a single sum for the navbar badge.

🔧 Installation and Setup
Clone the repository:

Bash
git clone [your-repo-link]
Install dependencies:

Bash
npm install
Start the development server:

Bash
npm start