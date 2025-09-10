# 🛒 Symfony Product CRUD Application

This is a simple CRUD (Create, Read, Update, Delete) application built with **Symfony 6+**.  
It demonstrates how to manage a list of products using Symfony controllers, forms, validation, Doctrine ORM, and Twig templates.

---

## 🚀 Features

- List all products
- View a single product
- Add a new product
- Edit existing products
- Delete products
- Flash messages for user feedback
- Form validation with Symfony Validator

---

## 📂 Project Structure

Key files in this example:

- **Entity** → `App\Entity\Product`  
  Defines the Product model with fields: `id`, `name`, `description`, and `size`.

- **Form** → `App\Form\ProductType`  
  Symfony Form to create and edit products.

- **Controller** → `App\Controller\ProductController`  
  Contains all routes and logic for CRUD operations.

- **Templates** → `templates/product/`  
  Twig views for listing, showing, creating, editing, and deleting products.

---

## ⚙️ Requirements

- PHP >= 8.1
- Composer
- Symfony CLI (optional but recommended)
- Database (SQLite/MySQL/PostgreSQL supported)
- Node.js & Yarn/NPM (if using Symfony UX or assets)

---

## 🔧 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/symfony-product-crud.git
   cd symfony-product-crud

2. Install dependencies:
    ```bash
        composer install

3. Configure your database in .env:
  `DATABASE_URL="sqlite:///%kernel.project_dir%/var/data.db"`
    or for MySQL
  `DATABASE_URL="mysql://user:password@127.0.0.1:3306/my_database"`

4. Run database migrations
   ```bash
   php bin/console doctrine:database:create
   php bin/console doctrine:migrations:migrate

5. Start the Symfony local server:
   ```bash
   symfony server:start
