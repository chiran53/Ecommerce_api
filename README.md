# eCommerce_API
A basic eCommerce API built with Django REST Framework, allowing for product management, cart operations, and order processing. Under development – additional features and improvements to come.



# Simple Ecommerce API #

This API allows you to add items or create orders for the product.

The API is available at https://simple-ecommerce-n1gt.onrender.com

## Endpoints ##

### Products ###

GET `/products/`

returns a list of all products.

GET `/products/{id}/`

return detailed information about a product.

POST `/products/`

creates a new product.

PUT `/products/{id}/`

update detail of specific product.

DELETE `/products/{id}/`

delete specific product.

### Cart ###

GET `/cart/`

return the current cart and it's items.

POST `/cart/add_item/`

allows you to add items in the cart.

POST `/cart/remove/`

remove item from the cart

#### Example ####

POST`/cart/add_item/`

{
    
    "product_id": 1,
    
    "quantity": 2

}




### Oders ###

GET `/orders/`

return a list of orders.

GET `/orders/{id}/`

return details of specific order.

POST `/orders/place/`

place and order with current cart items.
