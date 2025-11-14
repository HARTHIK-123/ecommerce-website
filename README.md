eCommerce Store (Vanilla JS)

A simple, responsive, and visually pleasant mock eCommerce front-end built with vanilla HTML, CSS and JavaScript.
It fetches product data from Fake Store API
 and demonstrates core e-commerce UI interactions: product listing, add-to-cart, wishlist, cart preview, notifications and a lightweight checkout flow.

Perfect for learning, demos, portfolio projects, or as a starter template to extend into a full-stack store.

🚀 Features

Fetches real-ish product data from Fake Store API.

Responsive product grid with product images, titles and prices.

Add to Cart — update cart items and total price dynamically.

Wishlist — toggle heart icon to add/remove favorites.

Cart panel and Wishlist panel with simple UI.

Lightweight toast notifications for user feedback.

Plain, readable code — easy to extend or integrate into frameworks.

📂 Repo Structure
.
├── index.html         # Main HTML file
├── style.css          # Styling and responsive layout
├── script.js          # App logic (fetching, cart, wishlist, UI)
├── fake1.png          # Placeholder logo used in nav
└── README.md          # (this file)

🛠️ Getting Started
Prerequisites

No build tools required — this is a static site. You only need a modern browser.

Run locally (quick)

Clone the repo:

git clone https://github.com/<your-username>/ecommerce-store.git
cd ecommerce-store


Open index.html in your browser (double-click or File → Open).

Or serve with a simple static server (recommended for consistent behavior):

# using Python 3
python -m http.server 8000
# then open http://localhost:8000

🧩 How it works (quick overview)

script.js sends a GET request to https://fakestoreapi.com/products and receives an array of product objects.

displayProducts() builds product cards dynamically and injects them into #products-container.

addToCart() validates and adds product objects to an in-memory cart array and updates totalPrice.

toggleWishlist() toggles items in the in-memory wishlist array.

toggleCart() and showWishlist() reveal the respective side panels and refresh the DOM content.

checkout() currently demonstrates a simple alert — replace with real flow when integrating backend/payment.

🎨 UI / UX Notes

Navigation bar with search (UI-only) and links.

Responsive design via CSS media queries:

Desktop: grid of cards

Tablet & Mobile: stacked cards and expanded cart/wishlist panels

Toast notifications appear in the top-right for short feedback.

To include screenshots in this README, add them to /assets (or /screenshots) and use:

![Product grid screenshot](./screenshots/products.png)

✅ Improvements & Ideas (nice-to-have)

Persist cart & wishlist in localStorage so data survives reloads.

Quantity controls, remove-from-cart, product details modal/page.

Search and filtering by category or price range.

Sorting (price low→high, rating, popularity).

Add authentication & backend (orders, payments), or connect to Firebase.

Replace alert() checkout with a styled checkout page and payment integration (Stripe/PayPal).

Unit tests and simple E2E UI tests (Playwright / Cypress).

🧑‍💻 Technologies Used

HTML5

CSS3 (responsive)

JavaScript (ES6+)

Fake Store API
 — demo product data

📦 Deployment

This is a static site — deploy anywhere static sites are supported:

GitHub Pages

Netlify

Vercel

Surge.sh

Example: Deploy to GitHub Pages

Push the repo to GitHub.

In repository settings → Pages → choose the main branch and / (root) folder.

Save and open the provided URL.

🤝 Contributing

Contributions are welcome! If you want to add features, fix bugs, or improve styles:

Fork the repository

Create a branch: git checkout -b feat/my-feature

Commit changes: git commit -m "Add my feature"

Push: git push origin feat/my-feature

Open a Pull Request

Please include a short description of what you changed and why.

📜 License

This project is free to use. Add a license file (e.g., MIT) if you want to make permissions explicit.

✉️ Contact / Author

Created by Kuppam Harthik.
If you'd like improvements, demo integration, or a version with backend & persistence — open an issue or drop a PR!

Enjoy — and have fun building on it! 🎉
