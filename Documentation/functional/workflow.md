## Workflows for Functional Requirements

### Table of Contents

1. [User Management Workflow](#user-management-workflow)
2. [Product Management Workflow](#product-management-workflow)
3. [Category Management Workflow](#category-management-workflow)
4. [Cart Management Workflow](#cart-management-workflow)
5. [Order and Checkout Management Workflow](#order-and-checkout-management-workflow)
6. [Authentication and Authorization Workflow](#authentication-and-authorization-workflow)
7. [Public and Guest Access Workflow](#public-and-guest-access-workflow)
8. [Image and Media Management Workflow](#image-and-media-management-workflow)
9. [Data Validation Workflow](#data-validation-workflow)

---

### User Management Workflow

1. **User Registration**
   - Guest navigates to the registration page.
   - Guest fills out the registration form (name, email, password, etc.).
   - System validates the input and sends a verification email.
   - Guest clicks the verification link in the email.
   - System activates the user account.
2. **User Login/Logout**
   - User navigates to the login page.
   - User enters email and password.
   - System authenticates the user and grants access.
   - User logs out by clicking the logout button; session is terminated.
3. **User Profile Management」
   - Logged-in customer navigates to their profile page.
   - Customer updates personal or payment information.
   - System validates and saves the changes.
4. **User Role Management (Admin Only)」
   - Admin logs in and accesses the user management panel.
   - Admin assigns or changes user roles (Admin, Seller, Customer).
   - System updates the user’s role in the database.
5. **User Listing (Admin Only)」
   - Admin logs in and accesses the user management panel.
   - Admin views a list of all registered users.
   - Admin can filter or search for specific users.

---

### Product Management Workflow

1. **Product Creation」
   - Admin or seller logs in and navigates to the product management page.
   - User fills out the product form (name, price, description, images, etc.).
   - System validates the input and saves the product to the database.
2. **Product Listing」
   - User navigates to the product listing page.
   - System displays a list of products (all products for admins/sellers, filtered for customers/guests).
3. **Product Detail View」
   - User clicks on a product in the listing.
   - System displays detailed information and images for the selected product.
4. **Product Update」
   - Admin or seller navigates to the product management page.
   - User selects a product to edit, updates the information, and saves changes.
   - System validates and updates the product in the database.
5. **Product Deletion」
   - Admin or seller navigates to the product management page.
   - User selects a product to delete and confirms the action.
   - System removes the product from the database.
6. **Product Search and Filtering」
   - User enters search terms or applies filters (category, brand, price, etc.).
   - System displays matching products based on the criteria.

---

### Category Management Workflow

1. **Category Creation」
   - Admin logs in and navigates to the category management page.
   - Admin fills out the category form (name, description, image, etc.).
   - System validates the input and saves the category to the database.
2. **Category Listing」
   - User navigates to the category listing page.
   - System displays a list of categories.
3. **Category Detail View」
   - User clicks on a category in the listing.
   - System displays details and a list of products under the selected category.
4. **Category Update」
   - Admin navigates to the category management page.
   - Admin selects a category to edit, updates the information, and saves changes.
   - System validates and updates the category in the database.
5. **Category Deletion」
   - Admin navigates to the category management page.
   - Admin selects a category to delete and confirms the action.
   - System removes the category from the database.

---

### Cart Management Workflow

1. **Add to Cart」
   - Customer browses products and selects one to add to the cart.
   - System adds the product to the customer’s cart and updates the cart total.
2. **View Cart」
   - Customer navigates to the cart page.
   - System displays the contents of the cart.
3. **Remove from Cart」
   - Customer selects an item to remove from the cart.
   - System removes the item and updates the cart total.
4. **Cart Quantity Update」
   - Customer changes the quantity of an item in the cart.
   - System updates the cart total accordingly.

---

### Order and Checkout Management Workflow

1. **Checkout Process」
   - Customer proceeds to checkout from the cart page.
   - System prompts the customer to enter shipping and payment details.
2. **Order Placement」
   - Customer reviews the order and confirms the purchase.
   - System creates an order record and updates inventory.
3. **Order Listing」
   - Customer navigates to the order history page.
   - System displays a list of the customer’s orders.
4. **Order Detail View」
   - Customer clicks on an order in the list.
   - System displays detailed information about the selected order.
5. **Order Status Management」
   - Admin logs in and accesses the order management panel.
   - Admin updates the status of an order (pending, processing, shipped, delivered, canceled).
   - System notifies the customer of the status change.
6. **Payment Integration」
   - Customer selects a payment method at checkout.
   - System redirects to the payment gateway or processes the payment.
   - System confirms successful payment and updates the order status.

---

### Authentication and Authorization Workflow

1. **Authentication」
   - User attempts to access a restricted page or perform a sensitive action.
   - System checks if the user is logged in.
   - If not, the user is redirected to the login page.
2. **Role-Based Access Control (RBAC)」
   - After login, system checks the user’s role.
   - User is granted access only to features and data permitted for their role.

---

### Public and Guest Access Workflow

1. **Public Product Listing」
   - Guest navigates to the product listing page.
   - System displays a list of products.
2. **Public Product Detail View」
   - Guest clicks on a product in the listing.
   - System displays detailed information about the product.
3. **Registration Requirement」
   - Guest attempts to add a product to the cart, checkout, or place an order.
   - System prompts the guest to register or log in.

---

### Image and Media Management Workflow

1. **Product Image Upload」
   - Admin or seller logs in and navigates to the product or category management page.
   - User uploads an image for a product or category.
   - System validates and stores the image.
2. **Image Display」
   - User views a product or category page.
   - System displays the associated images.

---

### Data Validation Workflow

1. **Input Validation」
   - User submits a form (registration, product, category, cart, order).
   - System validates the input data (required fields, format, range, etc.).
   - If valid, the data is processed; if not, the user is prompted to correct the input.
