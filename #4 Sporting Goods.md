# #4 Sporting Goods

Suppose, you are building a comprehensive e-commerce website for your sporting goods business, offering a wide range of equipment and accessories for various sports. **On this platform, there will be a single user role that can handle both customer and admin tasks.**

  

This website will have the following core pages:

*   **Homepage**
*   **About Us Page**
*   **All Products Page**
*   **Manage Products Page**
*   **Single Product Page**
*   **Cart Page**
*   **Checkout Page**

  

* * *

### Main Requirements

  

### **1\. Navbar & Footer**

*   A navbar with logo and necessary menu items **(e.g. All Products, Manage Products, Cart, About Us)**
*   A meaningful footer. Must contain social media icons and the websites' page links

  

### 2. **Homepage**

*       *   **Hero Section** - Must use a carousel with discount information
    *   **Featured section** - This section will feature latest products in card view. Each card will have product name, category, stock quantity, brand, rating using a third party package [react-rating](https://www.npmjs.com/package/react-rating), product description, price, image and View Details button. On clicking View Details, the user will be redirected to the Single Product page.
    *   **Category** \- A section will display the categories of sporting goods. If a user clicks on a category, they will be redirected to the 'All Products' page, showing only the products based on that category.
    *   **Contact Us Section -** This section will have a form with relevant fields.

  

**Note:**

*       *       *   **`[optional]`** You can use [EmailJS](https://www.emailjs.com/) or **NodeMailer** to make the contact form functional.

  

### 3\. **About Us**

*       *   Information about the company
    *   Mission and vision statements
    *   Contact information
    *   Our Team Section
    *   Our Store Location Information

  

### 4\. **All Products**

*       *   Display all available products.
    *   Search functionality for users to find specific products based on **name**
    *   Filter functionality for users to find specific products based on **sport category, price, brand, rating** etc.
    *   Sorting options (ascending and descending by price).
    *   "Clear filter" button to reset all filters.

  

**Note:** Make sure each card has relevant information

  

### 5\. **Single Product**

*       *   Detailed view of a single product.
    *   Includes **product name, description, category, brand, stock quantity**, **rating using a third party package** [**react-rating**](https://www.npmjs.com/package/react-rating)**, product description, price, image** and **Add To Cart button**.
    *   You can use [react-photo-view](https://github.com/MinJieLiu/react-photo-view) package to view the image of each product **\[optional\]**
    *   **Add to Cart Button:** Allows adding the product to the cart.

**Note**

*       *       *   Duplicate products cannot be added to the cart. If a product that is already in the cart is added again, only the quantity for that product will increase, up to the stock count of that product. When the quantity reaches the stock count, the "Add to Cart" button for that product will be disabled.
        *   Give relevant information and ensure that the design is visually appealing and user-friendly.

  

### 6\. **Cart Page**

*       *   Can be a page or a modal
    *   View all products added to the cart.
    *   Implement functionalities to increase/decrease quantity and to remove items from the cart for each products.
    *   A section that will show the total price including 15% vat for the overall purchase.
    *   **Proceed to checkout Button:** Allows the user to place an order.
        *   If the product is in stock, this button will be activated. If the product is out of stock, the button will be deactivated. Clicking this button will take the user to the checkout page.

  

### **7\. Checkout Page**

  

**User Details:** Here, you will collect user information such as name, email, phone number, and delivery address.

  

**Payment Methods:** There will be two types of payment methods:

1. **Cash on Delivery:** By choosing this option and then clicking the "Place Order" button, the user will be directed to a success page with **Go To Home** link and the quantity will be deducted from the actual product stock.
2. **Stripe (optional):** By choosing this option and then clicking the "Place Order" button, the user will be redirected to the Stripe payment method. After a successful payment, the user will be directed to a success page, and the quantity will be deducted from the actual product stock.

  

#### 8\. Manage Products

*   User can add a product, delete a product and update a product using RTK Query.
*   Make sure while updating the product the user will not have to update every field of the form. The fields should be prefilled with existing data so that the user can update a particular field only.

  

**Note**

*       *   Make sure to inform the users with the help of modal/toast after every delete, update and create
    *   You must show changes on the UI after every actions
    *   Make sure to make the interface visually appealing and user friendly

  

### 9\. Backend

*   You must integrate the backend. You can either use the single-page backend you learned in Level 1 or the backend you learned in the NoSQL track.

  

### 10\. Design Requirements

  

*   The design will carry significant marks, emphasizing user experience and visual appeal.
*   Responsive design to ensure compatibility across different devices (desktop, tablet, mobile).
*   Consistent color scheme and branding related to sports.

  

### Bonus Requirements

1. Using RTK Query Polling to show latest products after every 30s
2. Implement animations using any other libraries on the homepage.
3. A detailed overview of your projects in your readme file and significant amount of meaningful commits

  

### Optional Features

*   **Integrate Stripe Payment**: For processing payments.
*   **Implement Pagination**: Implement pagination in the All Products page.

  

_Note: We highly recommend implementing these optional features, as they will make your project stand out._

  

* * *

  

### **References for Idea Generation**

  

*   [Badger](https://www.bsgsports.com/)
*   [Spartax](https://websitedemos.net/sports-wear-store-04/?customize=template)
*   [Sport Store](https://ordasoft.com/demo.php?view=pc&t=Sport%20store)
*   [MKS](https://mkscricket.com/)

  

Note: The references are only for idea generation. Do not copy the design from these sources.
