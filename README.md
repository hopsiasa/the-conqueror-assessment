
# The Conqueror Assessment

HTML implementation:
- The document follows the standard structure with a <!DOCTYPE html> declaration.
- The 'head' section includes meta tags for character set and viewport settings.
- Each HTML page includes a title reflecting the content ("The Conqueror Assessment" and "Order Summary").
- A main container div with the class '.container' is used to group  items.
- The items are represented as anchor 'a' elements with the class '.item'.
- Each item contains a nested structure with an image container, body container, and a select button.
- The grid layout is adjusted to show a different number of columns based on the screen width.
- The container for selected items 'div class="selected-items-container"' is initially set to 'display: none' and becomes visible when items are selected.
- JavaScript functionality is integrated to toggle the 'selected' class on items when clicked and selected items are dynamically updated in the selected items container.

CSS styling:
- Use of box-sizing: border-box to ensure predictable box models.
- Each item is styled with a border, border-radius, and background properties and image containers have a negative margin to create an overlay effect. (I think I should have done it more simpler here but I guess it could count this way also)
- Media queries used to create a responsive layout for different screen sizes (small, medium, large, and extra-large).

JavaScript:
- The 'DOMContentLoaded' event listener is used to ensure that the JavaScript executes after the HTML content has loaded .
- Click event listeners are added to each item to toggle the 'selected' class and update the selected items container.
- The 'updateSelectedItems' function dynamically creates selected item elements each with a remove button.
- The 'updateOrderLink' function updates the order link with selected items as URL parameters. (I could have stored the selected items in the browser's localStorage and to retrieve them when the user navigated to the order page but I thought that using URL parameters is more suitable for small sets of data)
- The total cost is calculated based on the selected items prices.
- A remove button is added to each selected item and clicking it removes the 'selected' class from the corresponding item and updates the selected items.

There are also comments in the code for better documentation.





## Run Locally

Clone the project

```bash
  git clone git@github.com:hopsiasa/the-conqueror-assessment.git
```

Go to the project directory

```bash
  cd the-conqueror-assessment
```

Open the index file in the browser

```bash
  open index.html
```