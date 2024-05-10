# Shopping Cart Application

This is a simple command-line shopping cart application written in C++. It allows users to add products to a cart, view the cart contents, and proceed to checkout.

## Features

- Add items to the cart
- View the cart
- Checkout and pay for items

## Files

### `cart_main.cpp`

This file contains the main logic of the shopping cart application.

#### Functions

1. **`chooseProduct()`**: Allows the user to choose a product from a list of available products. It displays the list of products, prompts the user for input, and returns the chosen product.

2. **`checkout(Cart &cart)`**: Handles the checkout process. It calculates the total amount of the items in the cart, prompts the user for payment, and provides change if necessary.

3. **`main()`**: The main function of the program. It contains the main loop where users can choose actions like adding items to the cart, viewing the cart, or checking out.

### `datamodel.h`

This header file defines the data model used in the application, including classes for `Product`, `Item`, and `Cart`.

#### Classes

1. **`Product`**: Represents a product with attributes like ID, name, and price. It provides methods to get the display name and short name of the product.

2. **`Item`**: Represents an item in the cart, consisting of a product and quantity. It calculates the price of the item and provides information about the item.

3. **`Cart`**: Represents the shopping cart, which stores items added by the user. It allows adding products, calculating the total amount, viewing the cart contents, and checking if the cart is empty.

## Usage

To run the application, compile `cart_main.cpp` and run the executable. Follow the on-screen instructions to interact with the shopping cart.

```bash
g++ cart_main.cpp -o shopping_cart
./shopping_cart
