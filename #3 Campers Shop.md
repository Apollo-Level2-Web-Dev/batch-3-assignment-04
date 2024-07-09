# #3 Campers Shop

# Project Overview

Campers Shop is an e-commerce website dedicated to providing all the necessary and fun items for camping enthusiasts. The design should be user-friendly and visually appealing, taking inspiration from sites like [Adventure Shop](https://adventureshop.mt/) , [Camping Shop](https://www.decathlon.co.uk/sports/camping), [The Camperco Shop](https://thecampercoshop.com/) (do not copy-paste, just use it for brainstorming).

## Core Pages and Functionalities

Develop a comprehensive e-commerce website with the following core pages and functionalities:

*   Homepage
*   Products Page
*   Product Details Page
*   Product Management
*   Cart Page
*   About Us Page

## Detailed Requirements

### 1\. Homepage

*   **Header:** Include logo and site name.
*   **Navbar:** Navigation links to other pages such as About Us, Products Page, and other necessary links. Include a cart icon, wishlist icon, or other essential icons or links.
*   **Hero Section:** Create a visually appealing section to captivate visitors.
*   **Best Selling/Recommended Products Section:** Highlight products you want to introduce to the market. add a view more button under this section, that will navigate to the products page.
*   **Categories Section:** Display product categories with images or icons.
*   **Featured Products:** Show a few highlighted products with a button to view the details page.
*   **Unique Section:** Add a distinctive section, such as video blogs, testimonials, or featuring tour groups.
*   **FAQ Section:** Include frequently asked questions about products, shipping, or other important thing.
*   **Footer:** Include contact information, social media links, and other relevant links.

### 2\. Products Page

*   **Product Listings:** Display all products in a grid or list view.
*   **Product Details Button:** Redirect to the Product Details page upon clicking.
*   **Searching and Filtering:**
    *   Search bar for searching products by name or description.
    *   Filters for categories and price range.
    *   Sorting options (ascending and descending by price).
    *   Clear button to reset all filters.

### 3\. Product Details Page

*   **Product Information:** Display product name, price, stock-quantity, description, category, ratings, and images.
*   **Add to Cart Button:** Allow users to add the product to the cart.
    *   **Note:** Duplicate products cannot be added to the cart. If a product is already in the cart, only its quantity will increase, up to the available stock. If the quantity reaches the stock limit or the product is out of stock, the "Add to Cart" button for that product will be disabled.

### 4\. Product Management

*   **Product List Table:** Display products in a table format with columns for product image, name, price, category, and actions.
*   **Actions:**
    *   Button to create a new product.
    *   Allow modification of existing details for updating a product.
    *   Allow to Delete products, add Prompt confirmation for deleting a product.

### 5\. Cart Page

*   **Cart Items:** List products added to the cart with their quantities.
*   **Quantity Controls:** Increase or decrease the quantity of each product.
    *   **Minimum Quantity:** 1
    *   **Maximum Quantity:** Limited by the available stock of the product.
*   **Remove Product Button:** Allow users to remove a product from the cart. Should prompt for confirmation before removing.
*   **Pricing Details:** Display detailed total pricing below the product list. Update dynamically when a product is added, removed, or when the quantity is increased or decreased.
*   **Place Order Button:** Allow the user to place an order.
    *   If the product is in stock, this button will be activated. If the product is out of stock, the button will be deactivated. Clicking this button will take the user to the checkout page.

### **6\. Checkout Page**

**User Details:** Collect user information, including name, email, phone number, and delivery address, through a form.

**Payment Methods:**

*   **Cash on Delivery:** Selecting this option and clicking the "Place Order" button will redirect the user to a success page, and the product quantity will be deducted from the stock.
*   **Stripe (optional):** Selecting this option and clicking the "Place Order" button will redirect the user to the Stripe payment page. After a successful payment, the user will be directed to a success page, and the product quantity will be deducted from the stock.

### 7\. About Us Page

*   **Contact Information:** Display phone number, email address, and physical address.
*   **Map:** Embed a Google Map showing the location of the shop.
*   **Social Media Links:** Include icons linking to social media pages.
*   **Mission Statement:** Share the mission and values of the company.
*   **Team Members:** Introduce key team members with photos and brief bios.

### 8\. UI/UX Enhancements

*   **Responsive Design:** Ensure the website is fully responsive and optimized for all devices (desktops, tablets, smartphones).
*   **State Management:** Use Redux for state management to ensure a consistent and scalable application state across the website.
*   **Fast Loading Times:** Optimize images and use efficient code to ensure fast loading times.
*   **Intuitive Navigation:** Design a clear and easy-to-use navigation system.
*   **Consistent Design Language:** Maintain consistent colors, fonts, and styles across all pages.
*   **Accessibility (optional):** Ensure the website meets accessibility standards (e.g., WCAG 2.1) for users with disabilities.
*   **Interactive Elements:** Use animations and interactive elements sparingly to enhance the user experience without overwhelming the user.

### Bonus Features

*   **Image Gallery:** Showcase images of products page. Implement a magnifier effect on product images (example: [W3Schools Image Magnifier](https://www.w3schools.com/howto/tryit.asp?filename=tryhow_js_image_magnifier_glass)).
*   **Page Refresh Warning:** Show a warning message when refreshing the page if the cart is not empty, to prevent loss of cart data.

### Optional Features

*   **Stripe Integration:** Implement a payment gateway.
*   **Random Featured Product:** Display 3 products by default and fetch random data every 10 seconds using RTK Query.

## Technical Specifications

*   **Frontend:** Use a modern JavaScript framework React, Redux, etc.
*   **Backend:** Implement necessary CRUD operations for managing products with node, and express.
