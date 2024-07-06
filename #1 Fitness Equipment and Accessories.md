# #1 Fitness Equipment and Accessories

## Overview

We're developing a comprehensive e-commerce website for fitness equipment using React, Redux, Mongoose, and Express. This platform will offer a seamless shopping experience with features like product listings, detailed product pages, and a user-friendly cart system. Additionally, it will include robust product management capabilities for administrators and bonus features such as debounced search and page refresh warnings to enhance performance and user experience. Optional integration with Stripe will provide secure payment processing. This project aims to create a modern, efficient, and user-centric online store for fitness enthusiasts.


### Backend Requirements

The backend should be built using Node.js, Express, and MongoDB. You can make a single-page server like you did in level 1, or optionally, you can use TypeScript along with a modular pattern to structure the codebase.

  

### Core Pages and Functionalities

1. **Homepage**
2. **Products Page**
3. **Product Management**
4. **Product Details Page**
5. **Cart Page**
6. **Checkout page**
7. **About Us Page**

### Detailed Requirements

### 1\. Homepage

*   **Header Section**: Includes the logo and site name.
*   **Navigation Links**: Links to other pages.
*   **Hero Section**: Visually appealing hero/branding section.
*   **Categories Section**: Displays product categories with images or icons. Clicking on a category redirects the user to the Products page, with the clicked category selected by default.
*   **Featured Products**: Displays a few products with a button to view the details page. There will be a button called explore more which will redirect the user to the products page.
*   **Benefits Section**: Highlights the benefits of using the products with images and text.
*   **Image Gallery**: Showcases images of healthy individuals who have used your products, displayed in a mosaic view (For reference: [https://ps.w.org/photo-gallery/assets/screenshot-5.png?rev=2039606](https://ps.w.org/photo-gallery/assets/screenshot-5.png?rev=2039606)).
*   **Footer**: Includes contact information, social media links, and other relevant links.

### 2\. Products Page

*   **Product Listings**: Displays all products with images, names, prices, and a button to view details.
*   **Searching and Filtering**:
    *   Search bar to search for products by name.
    *   Filters for categories and price ranges, allow multiple categories to be selected simultaneously.
        *   **Category Filters**: Allow multiple categories to be selected simultaneously. If multiple categories are selected, products from all selected categories will be shown. For example, if the "Cardio" and "Strength" categories are selected, products from both categories will be displayed in the product listings.
    *   Sorting options (ascending and descending by price).
    *   "Clear Filter" button to reset all filters.

### 3\. Product Details Page

*   **Product Information**: Displays product name, price, stock quantity, description, images, and category.
*   **Add to Cart Button**: Allows adding the product to the cart.
    *   **Note**: Duplicate products cannot be added to the cart. If a product that is already in the cart is added again, only the quantity for that product will increase, up to the stock count of that product. When the quantity reaches the stock count, the "Add to Cart" button for that product will be disabled.

  

### 4\. Cart Page

*   **Cart Items**: Lists products added to the cart with their quantities.
    *   Controls to increase or decrease the quantity of each product (The quantity should not exceed the available stock).
    *   Button to remove a product from the cart. Should prompt for confirmation before removing.
*   **Pricing Details**: Displays detailed total pricing below the product list, updating dynamically as product quantities change or products are removed.
*   **Proceed to checkout Button**: Allows the user to place an order.
    *   If the product is in stock, this button will be activated. If the product is out of stock, the button will be deactivated. Clicking this button will take the user to the checkout page.

### **5\. Checkout Page**

**User Details:** Here, you will collect user information such as name, email, phone number, and delivery address.

**Payment Methods:** There will be two types of payment methods:

1. **Cash on Delivery:** By choosing this option and then clicking the "Place Order" button, the user will be directed to a success page, and the quantity will be deducted from the actual product stock.
2. **Stripe (optional):** By choosing this option and then clicking the "Place Order" button, the user will be redirected to the Stripe payment method. After a successful payment, the user will be directed to a success page, and the quantity will be deducted from the actual product stock.

  

### 6\. Product Management

*   **Product List Table**: Displays products in a table format with columns for product name, price, category, and actions.
*   **Action Buttons**: For updating and deleting products.
    *   **Updating a Product**: Should allow modifying existing details. The fields should be prefilled with existing data.
    *   **Deleting a Product**: Should prompt for confirmation before deletion.
*   **Button to Create a New Product**: Allows adding a new product.
*   **Adding a Product**: Should include fields for name, price, description, images (you can use ImgBB for image upload or allow direct link entry), category, and stock.
*   **Note**: All update, delete, and create actions should reflect in real-time, implementing an optimistic update of the UI.

  

### 7\. About Us Page

*   **Company Overview**: Briefly describe the company's history, mission, and vision.
*   **Team Introduction**: Introduce the key members of the team with their roles and brief bios.
*   **Customer Testimonials**: Include a few testimonials from satisfied customers.
*   **Contact Information**: Provide detailed contact information and encourage users to reach out with questions or feedback.

_Note: Try to make the About Us page as attractive and creative as possible by using some basic animations and fancy gradients._

  

### 8\. UI/UX

*   **UI/UX Quality**: The user interface should be reasonably good, with wisely chosen colour combinations. The user experience should be smooth and intuitive. Consider using UI/UX design principles to enhance the overall aesthetics and usability of the site. There will be a dedicated mark allocated for UI/UX quality.
*   **Responsiveness**: The entire website must be responsive for both mobile and desktop devices.

### Bonus Features

*   **Debounce API Calls**: Implement debouncing for the search functionality to reduce the number of API calls.
*   **Page Refresh Warning**: Show a warning message when refreshing the page if the cart is not empty, to prevent loss of cart data.

### Optional Features

*   **Integrate Stripe Payment**: For processing payments.
*   **Implement Pagination**: In the Products page, with a custom implementation.

_Note: We highly recommend implementing these optional features, as they will make your project stand out._

###   

  

## References for Idea Generation

Here are some websites to inspire ideas for your project. These references are only for idea generation and should not be copied directly:

- [https://shop.lifefitness.com/](https://shop.lifefitness.com/)
- [https://mightyfitness.shop/](https://mightyfitness.shop/)
- [https://www.fitnessavenue.ca/](https://www.fitnessavenue.ca/)
- [https://www.northernfitness.ca/](https://www.northernfitness.ca/)

> Note: The references are only for idea generation. Do not copy the design from these sources.
