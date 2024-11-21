
# DJTech Ruby on Rails E-Commerce Project

An e-commerce platform for DJTech built with **Ruby on Rails**. This project allows users to browse products, view individual product details, and list their own products.

---

## Features

### Core Features
- Browse available products.
- View details of individual products (including key features, price, and an image).
- Add new products to the store.

### Technologies Used
- **Ruby on Rails**: Backend framework.
- **SQLite**: Database for local development.
- **Tailwind CSS**: Styling the application.
- **HTML & CSS**: Frontend structure and design.

---

## Setup Instructions

### Prerequisites
- Ruby (version 3.3.6 or newer)
- Rails (version 8.0.0 or newer)
- Node.js and Yarn
- SQLite (or another database engine if desired)

### Installation
1. Clone the repository:
   ```bash
   git clone <REPOSITORY_URL>
   cd DJTech


2. Install dependencies:
   ```bash
   bundle install
   yarn install
   ```

3. Set up the database:
   ```bash
   rails db:create
   rails db:migrate
   rails db:seed
   ```

4. Start the server:
   ```bash
   rails server
   ```

5. Visit the app in your browser at:
   ```
   http://localhost:3000
   ```

---

## Project Structure

### Models
- **Product**: Represents an item in the store. Includes attributes such as `name`, `price`, `features`, and `image`.

### Views
- **Home Page**: Displays the app’s homepage.
- **Products Page**: Lists all products with their names, images, and prices.
- **Individual Product Page**: Provides detailed information about a single product.

### Controllers
- **ProductsController**:
  - `index`: Displays all products.
  - `show`: Displays details of a single product.
  - `new`: Form to create a new product.
  - `create`: Saves a new product.

---

## Development Notes

### Adding a Product
To add a new product:
1. Click the "List a Product" button on the products page.
2. Fill in the name, price, features (optional), and an image URL.
3. Submit the form to add the product to the store.

### Pending Features
- User authentication for restricted actions (e.g., editing and deleting products).
- Shopping cart and checkout functionality.
- Search and filter options for products.

---

## Troubleshooting

### Common Errors
1. **Pending Migrations**
   Run the following command to resolve:
   ```bash
   rails db:migrate
   ```

2. **Permission Errors**
   Ensure you have the necessary permissions for the project directory and all its files. Try running:
   ```bash
   chmod -R 755 .
   ```

3. **Missing Gems**
   Run:
   ```bash
   bundle install
   ```

4. **Assets Not Compiling**
   Recompile the assets:
   ```bash
   rails assets:precompile
   ```

---

## License

This project is licensed under the MIT License.

---

### Made by Jonathan Rodriguez and David Torres
