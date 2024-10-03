# ToDo_List\

1. HTML Structure:
Bootstrap Navbar:

The navigation bar is styled using Bootstrap, providing links for Home, About, and a dropdown for items.
There is also a search form included in the navbar.
Form for Adding Tasks:

There are two input fields:
A title input (#title).
A description text area (#description).
A button to add items to the list and a button to clear the entire list.
Table for Displaying Tasks:

The to-do items are displayed in a table, with columns for item number, title, description, and a "Delete" button for each task.
2. JavaScript Functionality:
Adding Items:

The getAndUpdate() function is triggered when the user clicks the "Add to list" button. It retrieves the title and description entered by the user, adds them to the localStorage, and then calls the update() function to refresh the list on the page.
Updating the Table:

The update() function retrieves the stored items from localStorage, parses them, and populates the table by looping through each item.
Deleting Items:

The deleted(itemIndex) function deletes a specific item from the list. It removes the item from localStorage by its index and updates the table.
Clearing the List:

The clearStorage() function clears all stored items from localStorage after confirming with the user and refreshes the list.
3. Bootstrap & jQuery:
The page uses Bootstrap 4 for styling (buttons, forms, and table) and jQuery for some JavaScript functionality, such as handling events.
4. LocalStorage:
The items in the to-do list are stored in localStorage as a JSON array, allowing persistence even after refreshing or closing the browser.
Main Features:
Add tasks with a title and description.
View tasks in a table format.
Delete individual tasks.
Clear the entire list.
