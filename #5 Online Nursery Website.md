# #5 Online Nursery Website 🌱

## Project Overview 🌱

Develop an online nursery website using React, Redux, Node.js, and Express.js. The website will allow users to browse, filter, and search for products, add products to their cart, and make online payments via Stripe.js. Additionally, there will be a product and category management section for CRUD operations.

## 🌟Features

### 1\. Public Routes 🚀

All routes on the website are accessible without authentication.

### 2\. Product and Category Management 🛠️

-   **CRUD Products and Categories**: Create, read, update, and delete (CRUD) products and categories.
-   **Management Routes**: Available on the frontend for easy management.

### 3\. Product Browsing 🌿

- **Filtering, Pagination, Sorting, and Searching**: Users can efficiently browse through our product offerings with advanced filtering, pagination for easy navigation across multiple pages of products, sorting options to arrange products by relevance, price, name, etc and robust searching capabilities to quickly find specific items.
- **Product Details**: Users can view detailed information about a product.

### 4\. Shopping Cart 🛒

- **Add to Cart**: Users can add products to their cart by clicking an "Add to Cart" button. If a product is out of stock, it cannot be added to the cart.
- **Quantity Management**: Duplicate products are not added; instead, the quantity of the existing product is increased. Users cannot add more products than the available quantity in stock
- **Proceed to Checkout**: Users can proceed to the checkout page from the cart section.

### 5\. Checkout and Payment 💳

- **Order Creation**: Orders are created in the database with customer details including name, phone number, address, and other required information collected from a form filled out before proceeding to the payment page. If any selected product is out of stock, the order creation process will be prevented. Upon order creation, the system automatically decreases the quantity of each product in the order from available stock levels.
- **Payment Options**
  - **Stripe Integration**: Users can make online payments securely using Stripe.js. (Optional)
  - **Cash on Delivery (COD)**: Alternatively, customers can choose to pay in cash upon delivery of their order.

  

## 📋Landing Page Components

- **Navbar**: Navigation bar with links to various sections and pages.
- **Hero Section**: Highlighting the main features or promotions.
- **Product Search, Filter, and Pagination**: Options for users to refine their product search.
- **Category Section**: Display different product categories.
- **Product List**: Display products in card format with title, price, rating, and an "Add to Cart" button.
- **Product Details**: Clicking on a product card navigates to the product details page with comprehensive information including title, description, price, rating, and an "Add to Cart" button.
- **Image Gallery**: Showcases images of healthy individuals who have used your products, displayed in a mosaic view (For reference: [https://ps.w.org/photo-gallery/assets/screenshot-5.png?rev=2039606](https://ps.w.org/photo-gallery/assets/screenshot-5.png?rev=2039606) , [https://assets.hongkiat.com/uploads/free-responsive-image-gallery/8-bootstrap-gallery.jpeg](https://assets.hongkiat.com/uploads/free-responsive-image-gallery/8-bootstrap-gallery.jpeg)).
- **Footer**: Additional links and information.

## 📑Page List

- **Landing Page**: Main page with product search, filtering, pagination, category section, and product list.
- **Products Page**: Dedicated page with product pagination, filtering, and searching.
- **Product Details Page**: Detailed information about a specific product.
- **Checkout/Cart Page**: Displays products added to the cart and allows users to proceed to checkout.
- **Payment Page**: Page for handling payments through Stripe.js.
- **Product and Category Management Page**: Interface for managing products and categories.

## 🗂️State Management

- **Redux**: Use Redux to manage the state for products, categories, cart, and other actions.
- **Actions and Reducers**: Create actions and reducers for managing state changes.

## 🎨UI/UX

- **Quality**: The user interface should be reasonably good, with wisely chosen color combinations. The user experience should be smooth and intuitive. Use UI/UX design principles to enhance the overall aesthetics and usability of the site.
- **Marks Allocation**: There will be a dedicated mark allocated for UI/UX quality.

## 🎁Bonus Features

- **Debounce API Calls**: Implement debouncing for the search functionality to reduce the number of API calls.
- **Page Refresh Warning**: Show a warning message when refreshing the page if the cart is not empty, to prevent loss of cart data.

## ⭐Optional Features

These features are recommended to enhance the project but do not have dedicated marks.

- **Integrate Stripe Payment**: For processing payments.
- **Implement Pagination**: In the Products page, with a custom implementation.

## 🌐References for Idea Generation

Here are some websites to inspire ideas for your project. These references are only for idea generation and should not be copied directly:

- [Treevaly](https://treevaly.com/)
- [Nursery Plants BD](https://nurseryplantsbd.com/)
- [Trees Direct](https://treesdirect.co.uk/)
- [Garden Goods Direct](https://gardengoodsdirect.com/)
- [The Tree Center](https://www.thetreecenter.com/)

> Note: The references are only for idea generation. Do not copy the design from these sources.