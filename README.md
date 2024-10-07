# Overview

In this activity, you will use conditionals to determine which CSS stylesheet to apply to a
webpage. Which stylesheet is applied will be based on user click behavior.

## Instructions

1. Open `index.html` (from the .zip file) in Visual Studio Code as well as in your browser.
   </br></br>
   **Note:** The webpage is almost complete, but note that the theme buttons in the upper
   right don’t yet trigger an action. You will be adding JavaScript to dynamically change the
   CSS styles applied to the page.

### Add a Conditional

1. Open `themeChange.js` from the .zip file in Visual Studio Code.
2. Add an event listener for the `click` event on the `themeChange` class.</br>
   ○ **Note:** Recall the basic structure of an event listener:</br>
   `$("element").on("event", function(){`</br>
   `...`</br>
   `});`
3. Add an if-else statement within the click event listener.
   ○ This statement will determine which button the user clicked.
   ○ **Note:** Recall the structure for an if-else statement:</br>
   `if (condition) {`</br>
   `...`</br>
   `} else if (condition) {`</br>
   `...`</br>
   `}`</br>
4. Add a check for the first condition—if the button clicked has the `regular` class.</br>
   ○ You can check if `this` has a particular class by using the built-in jQuery function
   `hasClass`.</br>
   `$(this).hasClass("className")`</br>
   ○ If this condition is true, update the `href` attribute for the `theme` ID to
   css/blank.css. You can use the built-in jQuery function `attr` to update the
   value of an HTML element.
   `$("#idValue").attr("attributeName", "attributeValue")`
5. Next, add a conditional check if the button clicked has the blue class.</br>
   ○ If this condition is true, update the href attribute for the `theme` ID to
   `css/blue.css`.
6. Lastly, check if the button clicked has the `dark` class.</br>
   ○ If this condition is true, update the `href` attribute for the `theme` ID to
   `css/dark.css`.
7. Refresh `index.html` in your browser.
8. Click on any of the theme buttons in the upper-right corner. Check out that dynamic CSS!

### Bonus:

● Now that you have finished the basics of our theme switcher, why not create your own
stylesheet for a custom theme you create?</br>
● Make sure you add an HTML button and the jQuery code to make it work.</br>
● Have fun!
