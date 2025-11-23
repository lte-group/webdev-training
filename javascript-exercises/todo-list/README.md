# To-Do List

## Exercise Overview

Build a simple to-do list where users can add, remove, and mark tasks as complete using DOM manipulation.

## Objectives

- Learn DOM manipulation techniques
- Handle user input and events
- Dynamically create and remove HTML elements
- Work with event listeners
- Manage application state

## Key Concepts

- DOM selection (`querySelector`, `getElementById`)
- Creating elements (`createElement`)
- Event listeners (`addEventListener`)
- Event handling (click events, input events)
- CSS classes for styling states
- Array methods for managing tasks

## Features to Implement

1. **Add Tasks**: Input field and button to add new tasks
2. **Display Tasks**: Show all tasks in a list
3. **Mark Complete**: Click on tasks to toggle completion status
4. **Remove Tasks**: Delete button for each task
5. **Visual Feedback**: Different styling for completed tasks

## Suggested HTML Structure

```html
<div class="todo-container">
    <input type="text" id="taskInput" placeholder="Enter a new task">
    <button id="addButton">Add Task</button>
    <ul id="taskList"></ul>
</div>
```

## Tasks

1. Create the HTML structure with input field, button, and empty list
2. Add an event listener to the "Add" button
3. Create a function that adds a new task to the list
4. Add functionality to mark tasks as complete (click to toggle)
5. Add a delete button for each task
6. Style completed tasks differently (e.g., strikethrough, different color)

## Tips

- Use `document.createElement()` to create new list items
- Use `element.appendChild()` to add elements to the DOM
- Use `classList.toggle()` to add/remove CSS classes
- Use `element.remove()` to delete elements
- Consider using data attributes to track task information
- Add keyboard support (press Enter to add task)
- Clear the input field after adding a task

## CSS Styling Ideas

- Strikethrough text for completed tasks
- Different background colors for completed vs. active tasks
- Hover effects on tasks and buttons
- Smooth transitions for adding/removing tasks

## Extension Challenges

- Add local storage to persist tasks between sessions
- Add task editing functionality
- Add filter buttons (All, Active, Completed)
- Add a "Clear Completed" button
- Add task priority levels or categories
- Add due dates to tasks
- Add drag-and-drop reordering
