### TODO List Application
This is a simple todo list application implemented using JavaScript. The application allows users to add tasks, mark them as completed, and remove them. The tasks are saved in the browser's local storage, so they persist across page reloads.

## Features
- Add new tasks by typing in the input box and pressing Enter.
- Mark tasks as completed by clicking on them.
- Remove tasks by clicking the "×" button next to each task.
- Tasks are saved in local storage and are reloaded when the page is refreshed.

## Explanation

# Variables
- inputBox: References the input element where users type their tasks.
- listContainer: References the container where the task list is displayed.

# Functions
- AddTask(): Adds a new task to the list. If the input box is empty, it shows an alert. Otherwise, it creates a new list item (li) with the task text and a "×" button to remove the task. The task is then saved to local storage.
- SaveData(): Saves the current task list to local storage.
- ShowList(): Loads the task list from local storage and displays it.

# Event Listeners
- inputBox.addEventListener("keypress", ...): Adds a task when the Enter key is pressed.
- listContainer.addEventListener("click", ...): Toggles the completion status of a task when it is clicked, and removes the task when the "×" button is clicked.

## How to Use
- Open the HTML file containing the input box and list container elements.
- Type a task in the input box and press Enter to add it to the list.
- Click on a task to mark it as completed.
- Click the "×" button next to a task to remove it.

The tasks will be saved automatically and reloaded when the page is refreshed.

## Local Storage
The application uses the browser's local storage to save the task list. The SaveData function stores the inner HTML of the listContainer in local storage, and the ShowList function retrieves it when the page loads. This ensures that the task list persists across page reloads.
