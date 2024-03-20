# Arisavo E-commerce Platform

Welcome to Arisavo, a vibrant e-commerce platform dedicated to bringing the best of handmade goods directly to your doorstep. Our platform empowers artisans to share their unique, handcrafted items with a global audience, offering a diverse range of products that cater to various tastes and preferences.

## Features

Arisavo is designed with both artisans and shoppers in mind, providing a seamless and intuitive user experience. Key features include:

- **User Authentication:** Secure sign-up and login processes to protect user information.
- **Artisan Profiles:** Dedicated profiles for artisans to showcase their products, story, and more.
- **Product Listings:** A comprehensive listing feature that allows for easy browsing of available handmade goods.
- **Shopping Cart and Checkout Process:** An intuitive shopping cart and straightforward checkout process, integrated with Stripe or PayPal for secure payments.
- **Search and Filter Capabilities:** Advanced search and filter options to help users find exactly what they're looking for.
- **Responsive Design:** A mobile-friendly design ensures a great browsing experience on any device.

## Technology Stack

Our project leverages a modern technology stack to ensure high performance, scalability, and ease of development:

- **Frontend:** Blazor WebAssembly
- **Backend:** ASP.NET Core
- **Database:** Entity Framework Core with SQL Server
- **Payment Processing:** Stripe or PayPal
- **Design and UX:** Figma
- **CI/CD:** GitHub Actions

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- .NET 6.0 SDK
- SQL Server
- Node.js (for npm)
- Git

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/YourGitHub/Arisavo.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Arisavo
   ```
3. Install the required dependencies:
   ```sh
   dotnet restore
   ```
4. Start the development server:
   ```sh
   dotnet run
   ```

## Roadmap


### 1. User Authentication:
   - **Purpose**: Allow users to register, log in, and manage their accounts.
   - **Components**:
     - Registration page (`Register.razor`): Form to sign up new users.
     - Login page (`Login.razor`): Form to authenticate returning users.
     - User profile page (`Profile.razor`): Allows users to view and edit their profile.
   - **Backend**:
     - ASP.NET Core Identity for managing users and roles.
     - Secure token generation for authentication.
     - Database tables for Users and Roles.

### 2. Artisan Profiles:
   - **Purpose**: Enable artisans to create profiles and manage their personal storefront.
   - **Components**:
     - Artisan profile page (`ArtisanProfile.razor`): Display artisan details and their products.
     - Storefront management page (`Storefront.razor`): Allows artisans to add, edit, and remove products.
   - **Backend**:
     - Database tables for Artisan profiles and their relations to Users.
     - CRUD operations for profile management.

### 3. Product Listings:
   - **Purpose**: Showcase products with details for customers to view.
   - **Components**:
     - Product listing page (`Products.razor`): Displays a list of products.
     - Product detail page (`ProductDetail.razor`): Shows detailed view when a product is selected.
   - **Backend**:
     - Database tables for Products with fields for name, description, price, images, etc.
     - CRUD operations for product management.

### 4. Shopping Cart:
   - **Purpose**: Allow customers to select products and prepare for checkout.
   - **Components**:
     - Shopping cart page (`Cart.razor`): Lists items the user intends to purchase.
     - Cart management component (`CartManager.razor`): Used to add, remove, or change the quantity of products.
   - **Backend**:
     - A session or database-backed service to track cart items per user.

### 5. Checkout Process:
   - **Purpose**: Enable customers to purchase their selected items.
   - **Components**:
     - Checkout page (`Checkout.razor`): Form to collect shipping and payment information.
     - Order confirmation page (`OrderConfirmation.razor`): Shows the order details post-purchase.
   - **Backend**:
     - Integration with payment gateway (Stripe or PayPal) for payment processing.
     - Database tables for Orders and OrderItems.

### 6. Basic Search and Filter Capabilities:
   - **Purpose**: Allow customers to find products.
   - **Components**:
     - Search bar component (`SearchBar.razor`): Input for keyword searches.
     - Filter component (`Filter.razor`): Options to filter products by category, price, etc.
   - **Backend**:
     - Search and filter logic to query the database based on user input.

### 7. Responsive UI:
   - **Purpose**: Ensure the website is accessible on various devices.
   - **Components**:
     - Use of responsive design principles in CSS.
     - Media queries in `app.css` to adjust layout and components for different screen sizes.

### Technical Stack:
- **Frontend**:
  - Blazor WebAssembly for the client-side SPA.
  - Razor components for building the UI.
- **Backend**:
  - ASP.NET Core as the server-side framework.
  - Entity Framework Core for ORM.
  - SQL Server for the database.
- **Payment Processing**:
  - Stripe or PayPal API integration.
- **DevOps**:
  - GitHub for source control.
  - GitHub Actions for CI/CD to automate deployment.
- **Design**:
  - Figma for UX/UI design mockups.

### Development Steps:
1. Set up the development environment (IDE, .NET SDK, SQL Server, etc.).
2. Initialize the project with Blazor WebAssembly template.
3. Set up the ASP.NET Core backend and configure the database.
4. Implement user authentication using ASP.NET Core Identity.
5. Create the database schema for users, products, orders, etc.
6. Develop the frontend components and pages as Razor components.
7. Integrate the frontend with the backend services.
8. Test each feature individually and then as a whole system.
9. Set up GitHub Actions for CI/CD.
10. Deploy the MVP to a hosting environment.

