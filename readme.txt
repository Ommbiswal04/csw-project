CSW Project 2 – E-Shop (Spring Boot + HTML/JS Frontend)
A simple e-commerce web application with a Spring Boot backend and a static HTML/CSS/JavaScript frontend.
Features include product listing, cart, order placement, and viewing/clearing order history.

Features
Product Catalog: Browse a list of products with images and prices.

Shopping Cart: Add products to the cart and place orders.

Orders & Returns: View your order history and clear it with one click.

Responsive Design: Clean, modern UI using Bootstrap.

Project Structure
text
CSW PROJECT 2/
│
├── backend/
│   ├── src/
│   │   └── main/
│   │       └── java/
│   │           └── com/
│   │               └── example/
│   │                   └── cswproject2/
│   │                       ├── CswProject2Application.java
│   │                       ├── controller/
│   │                       │   └── OrderController.java
│   │                       ├── model/
│   │                       └── service/
│   │                           └── ProductService.java
│   └── resources/
│       └── application.properties
│   └── pom.xml
│
└── frontend/
    ├── index.html
    ├── cart.html
    ├── offers.html
    ├── orders-returns.html
    ├── WhyChooseUs.html
    ├── WhyChooseUs.css
    └── images/
        └── (product images)
Getting Started
1. Backend Setup
Requirements: Java 8+ and Maven

Navigate to the backend/ directory.

Build the project:

bash
mvn clean install
Run the Spring Boot server:

bash
mvn spring-boot:run
The backend runs on http://localhost:8080.

2. Frontend Setup
No build step required.

Open frontend/index.html in your browser to start using the app.

For best results (especially for images), use a simple HTTP server or Live Server in VS Code:

Right-click index.html → “Open with Live Server” (recommended).

Or use Python’s HTTP server:

bash
cd frontend
python -m http.server 5500
Then visit http://localhost:5500/index.html

Usage
Browse Products: On the home page, view products and add them to your cart.

Place Orders: Go to the cart, review items, and place an order.

View Orders: Open orders-returns.html to see your order history.

Clear History: Click the “Clear History” button on the Orders & Returns page to delete all past orders.

Customization
Add/Edit Products:
Edit ProductService.java in the backend to change product names, images, or prices.

Product Images:
Place images in frontend/images/ and reference them in ProductService.java using relative paths (e.g., "images/my-product.jpg").

Troubleshooting
Images Not Displaying?

Make sure you are running a local server for the frontend (Live Server or python -m http.server).

Image paths in ProductService.java should be relative if opening HTML directly.

Backend Not Responding?

Ensure the Spring Boot server is running (mvn spring-boot:run).

Check for errors in the terminal.

This project is for educational/demo purposes.

Authors
--------
1. R. Subhransu Mahapatra (2341013014)
2. Om Biswal (2341002217)
3. Chandra Sekhar Jena (2341010049)

Happy Coding!
