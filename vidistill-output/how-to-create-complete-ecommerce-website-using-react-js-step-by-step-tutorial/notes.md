# Notes

This video provides a comprehensive guide to building the frontend of an e-commerce website using the MERN stack, focusing primarily on React and CSS. The tutorial covers setting up the project structure, implementing a dynamic navigation bar, creating reusable product components, and managing state using the React Context API. Viewers learn how to build essential pages including the homepage, category-specific product listings, detailed product views, and a functional shopping cart with real-time total calculations.

## Key Decisions

### [00:05:49] Use React Router DOM for client-side navigation

To enable seamless transitions between pages like Shop, Mens, Womens, and Kids without reloading the browser.

### [01:23:00] Implement state management via React Context API

The presenter chooses Context over Redux to centralize product data and cart state, making it accessible to deeply nested components like the Navbar and CartItems.

### [00:07:23] Adopt a component-based directory structure

Separating assets, components, context, and pages into distinct folders ensures the project remains scalable and organized.

### [02:23:51] Use a functional component with an index-based cart state

The cart is initialized as an object where keys correspond to product IDs and values to quantities, allowing for O(1) updates when adding or removing items.

### [02:22:37] Implement window.scrollTo(0,0) on item clicks

To ensure that when a user selects a product from the related products or collection lists, the page loads at the top rather than staying at the previous scroll position.

## Key Concepts

### [00:20:28] Conditional Rendering with Ternary Operators

Used in the Navbar and ShopCategory components to display active states (underlines) or filter products based on props.

### [01:47:50] Dynamic Routing with useParams

Extracting the ':productId' from the URL to fetch and display the correct item details on the Product page.

### [01:24:40] Prop Drilling vs. Context API

The video demonstrates why Context is superior for data like 'all_product' which needs to be accessed by virtually every page component.

### [00:49:15] Higher-Order Functions (Array.map)

Used extensively to transform raw JSON product data into a list of rendered 'Item' components.

## Topics

### Project Setup and Navigation _(00:04:42, 00:32:51)_

Initializing the folder structure, installing dependencies, and building a responsive Navbar with active link states and routing.

- Setting up the frontend folder and installing react-router-dom.
- Creating functional components for Navbar and individual pages.
- Using React Router's Link and Route components for single-page application behavior.

### Homepage Component Architecture _(00:33:07, 01:22:31)_

Building the visual elements of the landing page, including the Hero section, Popular items, exclusive Offers, and Footer.

- Designing the Hero section with a linear gradient and image assets.
- Creating a reusable Item component for product cards.
- Mapping through data arrays to display 'Popular' and 'New Collections' sections.

### Global State and Context API _(01:23:00, 01:28:31)_

Setting up a centralized data store for products and cart logic that spans the entire application.

- Creating ShopContext to hold product data and cart functions.
- Using the Provider pattern to wrap the App component.
- Accessing context data using the 'useContext' hook in child components.

### Dynamic Product and Category Pages _(01:28:51, 02:19:50)_

Implementing product filtering by category and detailed product views using URL parameters.

- Passing category props to the ShopCategory component to filter display items.
- Using useParams to fetch specific product details on the Product page.
- Developing Breadcrumbs and ProductDisplay sub-components.

### Cart Logic and Real-time Updates _(02:23:18, 02:58:57)_

Building the shopping cart backend logic and the corresponding frontend UI for item management and price calculation.

- Initializing a cart object with zeros for all product IDs.
- Implementing addToCart and removeFromCart functions within context.
- Calculating subtotal, total items, and displaying them in the Cart page and Navbar.

## Questions Raised

- **[01:30:00]** How can we display a specific banner for each shopping category while using the same ShopCategory component? (answered)
- **[01:32:42]** How can we prevent the 'underline' style from the Link tag from appearing on navigation text? (answered)
- **[01:49:15]** What is the best way to handle numeric IDs when comparing URL strings (useParams) to data objects? (answered)

## Action Items

- **[00:05:23]** Initialize the React project using 'npx create-react-app .' — _SPEAKER_00 (GreatStack)_
- **[00:22:00]** Import Google Font 'Poppins' and set as the default font family in index.css — _SPEAKER_00 (GreatStack)_
- **[01:27:01]** Create the ShopContext and wrap the entire application in the ShopContextProvider in index.js — _SPEAKER_00 (GreatStack)_
- **[02:51:36]** Develop the 'getTotalCartAmount' logic to iterate through cart state and multiply quantities by product prices. — _SPEAKER_00 (GreatStack)_
- **[02:57:09]** Link the 'nav-cart-count' div in the Navbar to the 'getTotalCartItems' context function to show live updates. — _SPEAKER_00 (GreatStack)_