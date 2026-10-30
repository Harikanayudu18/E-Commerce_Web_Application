# NovaCart — Responsive E-commerce Frontend

A clean, professional, beginner-friendly e-commerce storefront built with **HTML5, CSS3, JavaScript and Bootstrap 5**. It is a frontend-only demo suitable for learning, portfolio presentation, and further customization.

## Preview

NovaCart includes a responsive landing page, product catalogue, category filters, product search, sorting, a shopping-cart drawer, quantity controls, persistent cart storage, and a newsletter form interaction.

## Tech stack

- **HTML5** — semantic page structure
- **CSS3** — custom styling, responsive layout and visual design
- **JavaScript (ES6)** — product rendering and interactive behaviour
- **Bootstrap 5.3** — responsive grid, navbar and utility classes
- **Bootstrap Icons** — interface icons
- **LocalStorage** — remembers the demo cart in the current browser

## Project structure

```text
novacart-ecommerce/
├── index.html
├── README.md
└── assets/
    ├── css/
    │   └── style.css
    └── js/
        └── app.js
```

## Getting started

### Option 1 — Open directly

1. Download and extract the project ZIP.
2. Open the `novacart-ecommerce` folder.
3. Double-click `index.html` to open the website in your browser.

### Option 2 — Use VS Code (recommended)

1. Open the extracted folder in Visual Studio Code.
2. Install the **Live Server** extension if you do not already have it.
3. Right-click `index.html`.
4. Select **Open with Live Server**.

No npm install, build command, backend, or database is required.

## Features

| Feature | Description |
|---|---|
| Responsive navigation | Bootstrap navbar with mobile menu |
| Hero section | Large editorial-style landing section |
| Product catalogue | Product cards generated from JavaScript data |
| Category filtering | Filter Home, Accessories and Lifestyle products |
| Search | Search by product name or category |
| Sorting | Featured, price low-to-high and high-to-low |
| Add to cart | Add products from catalogue cards |
| Cart drawer | Slide-in cart with item details and subtotal |
| Quantity controls | Increase, decrease or remove cart items |
| Cart persistence | Cart data is saved using browser LocalStorage |
| Newsletter interaction | Basic client-side email form feedback |

## Customization

### Change products

Open `assets/js/app.js` and edit the `products` array. Each product uses this structure:

```js
{
  id: 1,
  name: "Example Product",
  category: "Home",
  price: 1299,
  oldPrice: 1599,
  badge: "NEW",
  rating: "4.9",
  image: "https://example.com/product-image.jpg"
}
```

Use a unique numeric `id`. Supported categories in the current filter are `Home`, `Accessories`, and `Lifestyle`.

### Change colors and styles

Open `assets/css/style.css`. The main theme colors are defined at the top using CSS variables:

```css
:root {
  --ink: #20231f;
  --muted: #777d75;
  --cream: #f5f4ef;
  --sage: #dce4d9;
  --line: #e9e9e3;
  --accent: #a9b8a4;
}
```

### Change store name and content

Edit the brand text, page copy, footer and metadata in `index.html`.

## Important notes

- This is a **frontend demonstration project**, not a production-ready online store.
- The checkout button intentionally displays a demo message. It does not process payments or create orders.
- The newsletter form displays an on-page confirmation only. It does not send or store email addresses on a server.
- Products and cart state are managed in the browser. Cart data is stored in LocalStorage on that device/browser.
- Product photography and web fonts are loaded from external services (Unsplash and Google Fonts). An internet connection is needed for those assets.
- Bootstrap and Bootstrap Icons are loaded through jsDelivr CDN.

## Suggested next improvements

1. Build a product details page.
2. Add a backend API and database for products, users and orders.
3. Add authentication and user profiles.
4. Integrate a secure payment provider in a backend-supported checkout flow.
5. Add server-side newsletter subscriptions and order confirmation emails.
6. Add product image uploads, inventory management and admin dashboard.

## License

This starter project is provided for learning and personal portfolio use. Replace demo content, product images and branding as needed before publishing a commercial website.
