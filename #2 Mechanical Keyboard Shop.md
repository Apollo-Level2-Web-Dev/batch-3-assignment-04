# #2 Mechanical Keyboard Shop

## **Overview:**

We're developing an e-commerce website exclusively for mechanical keyboards using React, Redux, Mongoose, and Express. Our site will feature easy product browsing, detailed product pages, and a smooth cart system. Administrators will have powerful tools for managing products, and users will enjoy features like fast search, page refresh warnings, and filtering. Optional integration with Stripe ensures secure payments. Our goal is to create a modern and user-friendly online store for mechanical keyboard enthusiasts.

  

Please develop this comprehensive e-commerce website with the following core pages and functionalities:

*   Homepage
*   Products Page
*   Product Details Page
*   Cart Page
*   Checkout Page
*   Product Management/Dashboard Page
*   About Us Page
*   Contact Us Page

### Technology Stack

The project will be built using the following technologies:

**Frontend**: React with Vite, TypeScript, Redux, RTK Query.

**Backend:** TypeScript, Node, Express, MongoDB, Mongoose, Zod.

  

### Backend Requirements

The backend should be built using Node.js, Express, and MongoDB. You can make a single-page server like you did in level 1, or optionally, you can use TypeScript along with a modular pattern to structure the codebase.

  

### Detailed Requirements

#### 1\. Homepage / Landing Page

*   **Header Section** / **Navbar :**
    *   Display the logo or the website name at the top left of the navbar.
    *   Provide navigation links to the following _navbar items:_
        *   Home
        *   Products
        *   About Us
        *   Contact Us
        *   Product Management/Dashboard.
    *   Include a **Cart Icon** at the right most part of the navbar, that shows the number of items currently in the cart.

> All the navbar items including the website logo / website name, cart icon must be clickable and should redirect to their corresponding pages. You can also handle the active link.

*   **Hero Section:**
    *   A large, visually appealing section at the top of the page (below the navbar) showcasing the brand and products to attract visitors' attention.
*   **Service Advertisement:**
    *   A section advertising the benefits and services offered by the store. Example : Free Shipping, Lowest Delivery Charge, 24/7 Support etc. (For reference: [https://prnt.sc/Noo5bJlk\_QDc](https://prnt.sc/Noo5bJlk_QDc))

  

*   **Featured Products:**
    *   Show **6 featured products card** with a button that takes the user to the product details page.

> Always show the latest 6 created products from your database. hints: You can use the sort method in this case.
> 
> *   The featured products must have the following properties on the card:
>     *   Image
>     *   Title / Name
>     *   Brand
>     *   Available Quantity
>     *   Price
>     *   Rating (In Stars)
>     *   See Details Button
> *   **See More Button,** that will take the user to **Products Page,** showing all the products. The button should be at the bottom of this section.

  

*   **Top Featured Brands:**
    *   Display logo and title of popular keyboard brands.

> You can use static / dynamic json data for this section.

  

*   **Customer Reviews:**
    *   A section displaying testimonials and reviews from customers, with accompanying images.
    *   Carousel can be used to show the reviews.

> You can use static / dynamic json data for this section.

  

*   **Extra Sections:**
    *   Two additional sections relevant to mechanical keyboards, such as:
        *   "Why Choose Mechanical Keyboards?"
        *   "Customizable Options"
*   **Footer:**
    *   Include contact information, social media links, and other relevant links at the bottom of the page. The links must be clickable and should redirect to their corresponding pages
    *   Footer design should be standard.

#### 2\. Products Page :

*   Display all products in card view. Each product card should show :
    - Image
        *   Title / Name
        *   Brand
        *   Available Quantity
        *   Price
        *   Rating (In Stars)
        *   Show Details Button
*   **Searching and Filtering:**
    *   A search bar to allow users to search for products by name, brand.
    *   Filters for product price range.
    *   Options to sort products by price (low to high and high to low).
    *   A clear filter button to reset all applied filters.

#### 3\. Product Details Page

*   **Product Information:**
    *   Show the following properties:
        *   Image
        *   Title / Name
        *   Brand
        *   Available Quantity
        *   Price
        *   Rating (In Stars)
        *   Description
        *   Add To Cart Button
    *   Shopping Cart
        *   **Add to Cart**: Users can add products to their cart by clicking an "Add to Cart" button. If a product is out of stock, it cannot be added to the cart.
        *   **Quantity Management**: When adding a product to the cart, the quantity in the cart icon will increase. Duplicate products are not added; instead, the quantity of the existing product is increased. Users cannot add more products than the available quantity in stock

#### 4\. Cart Page

*   **Cart Items:**
    *   List all products that have been added to the cart, along with their quantities.
    *   Include controls to increase or decrease the quantity of each product.
    *   Provide a button to remove a product from the cart.
*   **Pricing Details:**
    *   Show the detailed total pricing below the product list.
    *   Update the total price dynamically as products are added, removed, or quantities are changed.
*   **Proceed To Checkout Button**: Allows the user to place an order.
    *   If the product is in stock, this button will be activated. If the product is out of stock, the button will be deactivated. Clicking this button will take the user to the checkout page.

  

#### **5\. Checkout Page**

*   **User Details:** Here, you will collect user information such as name, email, phone number, and delivery address.
*   **Payment Methods:** There will be two types of payment methods:
    1. **Cash on Delivery:** By choosing this option and then clicking the "Place Order" button, the user will be directed to a success page, and the quantity will be deducted from the actual product stock.
    2. **Stripe (optional):** By choosing this option and then clicking the "Place Order" button, the user will be redirected to the Stripe payment method. After a successful payment, the user will be directed to a success page, and the quantity will be deducted from the actual product stock.

  

#### 6\. Product Management/Dashboard Page

*   **Product List Table:**
    *   Display products in a table format. The table should include columns for the product name, price, brand, and actions.
*   **Action Buttons:**
    *   Include buttons for updating and deleting products.
    *   Updating a product should open a form in a modal allowing the user to modify existing details.
    *   Deleting a product should open a confirmation modal, asking the user for confirmation before removal.
*   **Adding a Product:**
    *   Include a button to create the new product.
    *   Provide a form to add new products with fields for name, price, description, available quantity, rating, image (you can use ImgBB for image upload or allow direct link entry), and brand.

> All update, delete, and create actions should reflect in real-time, implementing an optimistic update of the UI.

#### 7\. About Us Page

- Try to make the About Us page as attractive and creative as possible by using some basic animations and fancy gradients.

#### 8\. Contact Us Page

- Provide detailed contact information and encourage users to reach out with questions or feedback.
    *   Try to make the page as attractive by using some basic animations.

#### 9\. UI/UX

*   **UI/UX Quality**: The user interface should be reasonably good, with wisely chosen color combinations. The user experience should be smooth and intuitive. Consider using UI/UX design principles to enhance the overall aesthetics and usability of the site. There will be a dedicated mark allocated for UI/UX quality.
*   **Responsiveness**: The entire website must be responsive for both mobile and desktop devices.

  

### Bonus Features

*   **Debounce API Calls:**
    *   Implement debouncing for the search functionality to reduce the number of API calls and improve performance.
*   **Page Refresh Warning:**
    *   Show a warning message when the user attempts to refresh the page if the cart is not empty, to prevent the loss of cart data.
*   **Animations**:
    *   Try to use micro-animations on your website

### Optional Features

*   **Integrate Stripe Payment**: For processing payments.
*   **Implement Pagination**: In the Products page, with a custom implementation.

_Note: We highly recommend implementing these optional features, as they will make your project stand out._

  

### References for Idea Generation

Here are some websites to inspire ideas for your project. These references are only for idea generation and should not be copied directly:

- [https://mechanicalkeyboards.com/](https://mechanicalkeyboards.com/)
- [https://kbdfans.com/](https://kbdfans.com/)
- [https://keygem.com/](https://keygem.com/)
- [https://keebsforall.com/](https://keebsforall.com/)
- [https://kono.store/](https://kono.store/)

> Note: The references are only for idea generation. Do not copy the design from these sources.