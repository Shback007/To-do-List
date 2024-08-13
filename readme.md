# To-Do List App

A simple and intuitive To-Do List application that allows users to manage their tasks efficiently. Users can add, edit, check off, and delete tasks, with data persistence via local storage.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Add Tasks:** Users can add new tasks using the input field.
- **Edit Tasks:** Users can edit existing tasks by clicking the edit button next to the task.
- **Mark as Complete:** Users can mark tasks as complete by clicking on the task. Completed tasks are visually distinguished.
- **Delete Tasks:** Users can delete tasks by clicking the delete button next to the task.
- **Data Persistence:** The app saves tasks in local storage, so they persist even after refreshing the page.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/todo-list-app.git
2. **Navigate to the project directory:**
    cd todo-list-app
3. **Open `index.html`**

## Usage

1. **Add a Task:**
   - Enter your task in the input box and click the `Add` button.
   - The task will be added to the list below with options to edit or delete the task.

2. **Edit a Task:**
   - Click the green edit button (✎) next to the task you want to edit.
   - A prompt will appear where you can modify the task.
   - After updating, click "OK" to save your changes.

3. **Mark as Complete:**
   - Click on a task to mark it as complete. The task will have a strikethrough effect, indicating it's completed.
   - Clicking the task again will toggle the completion status.

4. **Delete a Task:**
   - Click the delete button (×) next to the task you want to remove.
   - The task will be permanently removed from the list.

5. **Data Persistence:**
   - The app automatically saves the current state of the task list in the browser's local storage.
   - When the page is reloaded, the saved tasks will be retrieved and displayed.

## Code Overview

- **HTML Structure:**
  - The app is structured using basic HTML elements:
    - An input field for entering tasks.
    - A button to add the task.
    - An unordered list (`<ul>`) to display the tasks.
    - Each task is a list item (`<li>`) that contains:
      - The task name.
      - A delete button (×) to remove the task.
      - An edit button (✎) to modify the task.

- **CSS Styling:**
  - The app uses CSS for styling:
    - A gradient background for the app container.
    - Flexbox is used for layout alignment.
    - Task items have custom styles for normal, checked, and hovered states.
    - The edit and delete buttons have specific styles to distinguish them.

- **JavaScript Functionality:**
  - **`addTask()`**: 
    - This function creates a new list item when the user adds a task.
    - It includes adding edit and delete buttons to each task.
    - After adding a task, the data is saved to local storage.

  - **`editTask(taskElement)`**: 
    - Allows the user to edit a task by updating the task’s text.
    - Prompts the user with the current task text, allowing it to be modified.
    - Saves the updated task back to local storage.

  - **`saveData()`**: 
    - Stores the current list of tasks in the browser's local storage.
    - This ensures tasks persist even after the page is refreshed.

  - **`showTask()`**: 
    - Loads the task list from local storage when the page is loaded.
    - Displays the stored tasks, retaining their checked and unchecked statuses.

  - **`disableButtons(bool)`**: 
    - Temporarily disables the edit buttons, if needed.

  - **Event Listeners**:
    - **`button.addEventListener('click', addTask)`**: 
      - Attaches the `addTask()` function to the Add button.
    - **`listContainer.addEventListener('click', (e) => {...})`**: 
      - Handles clicks on tasks for checking/unchecking, editing, or deleting.
  
## Technologies Used

- **HTML5**: 
  - Used for structuring the content of the To-Do List App.
  - Elements like `<input>`, `<button>`, and `<ul>` are utilized to build the user interface.

- **CSS3**: 
  - Used to style the application, making it visually appealing and responsive.
  - Includes custom styling for buttons, task list items, and overall layout.

- **JavaScript (ES6)**: 
  - The core logic of the app is written in JavaScript.
  - Functions are used to manage tasks, handle user interactions, and store data in local storage.

- **Local Storage**: 
  - Web API used to store task data in the user's browser.
  - Ensures tasks persist across page reloads without needing a backend server.

  ## Contributing

Contributions are welcome! If you'd like to contribute to the project, please follow these steps:

1. **Fork the repository:**
   - Click on the "Fork" button at the top right of this repository's page.

2. **Clone your forked repository:**
   ```bash
   git clone https://github.com/Shback007/To-do-List.git
