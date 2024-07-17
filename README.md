# InteractiveShoppingList
# Shopping List Application
This application allows you to maintain a shopping list with basic functionalities such as adding items, marking them as purchased, and clearing the list.

Features:
Add Items: Type the name of the item in the input field and click Add Item to add it to the list.
Mark as Purchased: Click on an item in the list to mark it as purchased. Click again to unmark it.
Clear List: Click the Clear List button to remove all items from the list.
How to Use:
Adding Items:

Type the name of the item you want to add in the input field labeled New Item.
Click the Add Item button or press Enter to add the item to the shopping list.
Marking Items as Purchased:

Click on an item in the shopping list to toggle its status between purchased and unpurchased.
Purchased items are visually indicated by a strike-through effect.
Clearing the List:

To remove all items from the list, click the Clear List button labeled Clear Shopping List.
This action cannot be undone, and it will also clear any saved items stored in your browser's local storage.
Local Storage:
The application uses local storage to save the items you've added, so your list persists even if you refresh the page or close the browser.
If you clear your browser's local storage or use the application in a different browser or device, your saved items will not be accessible.
Technologies Used:
HTML: Provides the structure of the shopping list interface.
CSS: Basic styling to enhance the visual presentation of the application.
JavaScript: Implements the interactive features and manages data storage using local storage.
Implementation Details:
The application listens for DOM content to be fully loaded before initializing.
It checks if there are previously saved items in local storage and populates the list accordingly.
Each item in the list can be clicked to toggle its purchased status, which is reflected visually.
The list can be cleared completely using a dedicated button.
Development and Contributions:
This application is a basic implementation intended for learning purposes.
Contributions and enhancements are welcome via pull requests on the GitHub repository or by forking the project.
License:
This project is licensed under the MIT License - see the LICENSE file for details.
Code Explanation:
The JavaScript code initializes event listeners for adding items, marking them as purchased, and clearing the list. It utilizes local storage to persist the shopping list data between sessions. Here’s a breakdown of key components:

DOMContentLoaded Event: Ensures the DOM is fully loaded before executing JavaScript to manipulate elements.
Event Listeners:
addItemBtn: Adds a new item to the list when clicked.
newItem: Toggles the 'purchased' class on click to mark items as purchased or unpurchased.
clearListBtn: Clears all items from the list and removes them from local storage.
Local Storage: Stores and retrieves items using JSON serialization to maintain data between page refreshes.
This README provides an overview of the shopping list application, its features, and how to use it effectively. Adjustments and improvements can be made based on specific project requirements or user feedback.

# CSS Style for Purchased Items
In the shopping list application, purchased items are visually differentiated by applying a text decoration of line-through. This CSS rule enhances user experience by clearly indicating which items have been marked as purchased.

Implementation Details:
CSS Selector: .purchased

This selector targets elements that have the class purchased.
When an item in the shopping list is marked as purchased (by clicking on it), the JavaScript code dynamically adds or removes the purchased class to toggle the visual style.
Text Decoration:

text-decoration: line-through;
This CSS property applies a line through the text content of elements with the purchased class.
It provides a clear visual indication that the item has been marked as purchased.
How It Works:
When a user clicks on an item in the shopping list, the JavaScript code toggles the purchased class on the clicked element.
The presence of the purchased class triggers the CSS rule, applying the line-through text decoration to the item's text content.
Clicking the item again removes the purchased class, restoring the normal text appearance.
Benefits:
Visual Clarity: Users can easily distinguish between purchased and unpurchased items in the shopping list.
User Interaction: The dynamic application of CSS styles based on user actions (clicking items) enhances interactivity and user engagement.
Accessibility: Provides a clear visual cue that is beneficial for users with various browsing preferences and needs.
Considerations:
Compatibility: Ensure compatibility with different browsers and devices to maintain consistent visual styling.
Customization: The line-through decoration can be customized or replaced with alternative styles to suit specific design preferences or accessibility requirements.
Usage and Customization:
To integrate or modify the purchased CSS style in your project:

Integration:

Ensure that your HTML structure correctly integrates with the JavaScript functionality that toggles the purchased class on items.
Link your CSS file containing the .purchased style to your HTML document.
Customization:

Modify the .purchased CSS rule to adjust the visual appearance (e.g., color, font-size) of purchased items according to your project's design guidelines.
Testing:

Test the application across different browsers and devices to verify consistent display of the purchased styling.
Ensure accessibility standards are met to accommodate diverse user needs.
License:
This CSS style for indicating purchased items in a shopping list application is provided under the MIT License. See the LICENSE file for details.



