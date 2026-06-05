MewStore!
A React based E-commerce Web App where users can browse cat breeds, add them to a cart, and place an order.

Features:
Home: Animated scrolling banner of cat photos
Browse: Fetches cat breeds from The Cat API, with search, pagination, and a detail modal for each breed
Cart: View and remove selected cats, with a checkout form that validates name, email, and delivery address
About & Contact: Informational pages

Cart contents are saved to localStorage so they persist on page refresh.

Tech Stack:
React 19 + Vite
React Router DOM
React Bootstrap + Bootstrap 5
The Cat API (https://api.thecatapi.com/v1/breeds)

How It Was Built:

React Router: handles navigation between pages (Home, Browse, Cart, Contact, About) using BrowserRouter, Routes, and Route

The Cat API: The Browse page fetches cat breeds using fetch() inside a useEffect hook, then displays them in a paginated grid with live search filtering

Context API (CartContext): Manages cart state globally using createContext and useContext, so any page can add or remove cats without passing props around. The cart is also saved to localStorage so it persists on page refresh

React Bootstrap: Used for layout components like Container, Modal, and Button, including the checkout popup in the Cart page

Cart & Checkout: The cart page displays all added cats with a remove button, and opens a checkout modal with form validation that checks for empty fields and a valid email format
Vite: Used as the build tool and development server for fast hot module reloading

Getting Started:
Prerequisites:

Node.js (v18 or higher recommended)

Install dependencies (in the terminal):
1. npm install
2. npm run dev
3. Then open http://localhost:5173 in your browser.
