# Shopping-Cart-with-Updated-List-Feature
This code creates a navigation bar with a list of items and their stock numbers. Each item has a button that, when clicked, moves one item into the shopping cart. The code uses React.useState to keep track of the items in the cart and the stock items.

The NavBar component takes an array of stockitems as a prop, which contains objects with the name and stock number of each item. It then renders the list of items and buttons, with each button calling the moveToCart function when clicked.

The moveToCart function extracts the name and number of the item from the button's innerHTML, finds the corresponding item in the stock state using map, and decreases its instock property by one. It then updates the stock state with the new stock array.

The cart state starts as an empty array, and each time an item is moved to the cart, it is added to this array. The list of items in the cart is rendered below the list of stock items.

This code uses the ReactBootstrap library to render the buttons, and ReactDOM.render to render the NavBar component on the webpage.
