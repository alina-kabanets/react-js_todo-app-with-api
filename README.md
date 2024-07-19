# React ToDo App

## [Check the live demo here](https://alina-kabanets.github.io/react-js_todo-app-with-api/)

![preview img](/description/todoapp.gif)
![preview img](/description/edittodo.gif)

## Overview

The React ToDo App is a user-friendly task management application designed to help users stay organized and productive. It provides a soothing and visually appealing user interface, along with a range of features to enhance the task management experience.

## Technologies:

  - React functional components;
  - useEffect, useState, useContext, useDispatch, useRef, custom hooks;
  - useReducer for a better understanding of what is under the hood of Redux;
  - Local storage, refactored to API;
  - GET, DELETE, PATCH, POST methods for working with the API;
  - Promises, refactored to async/await syntax;
  - TypeScript types and enums;
  - React Transition Groups;


## Features:

The project was implemented using pre-made HTML and CSS markups; my task was to develop the React.js with TypeScript part.

### - Adding a todo

  Add a todo with the entered title on form submit:

  - the text field is focused by default;
  - if the title is empty - a "Title should not be empty" notification is shown at the bottom;
  - the title is trimmed when checked or saved;
  - sends a POST request to the API;
  - the input is disabled until receiving a response from the API;
  - immediately after sending a request, a todo with id: 0 is created and saved to the tempTodo variable in the state;
  - the temporary TodoItem has a loader;
  - in case of success, the todo created by the API is added to the array;
  - in case of an API error an "Unable to add a todo" notification is shown at the bottom;
  - the text field is focused after receiving a response;
  - in case of success the text is cleared;
  - keeps the text in case of an error;

### - Deleting todos

  Removes a todo on the TodoDeleteButton click:

    - the todo is covered with a loader while waiting for the API response;
    - removes the todo from the list on success;
    - in case of API error shows an "Unable to delete a todo" notification at the bottom (the todo stays in the list);

  Removes all the completed todos after the ClearCompleted button click:

    - the button is enabled only if there is at least one completed todo;
    - the deletion works as several individual deletions running at the same time;
    - in case of any error shows an error message but processes success deletions;

### - Inline editing for the TodoItem:

  - double-clicking on the todo title shows a text field instead of the title and deleteButton;
  - form submission saves changes (press Enter to save);
  - the saved text is trimmed;
  - the todo is deleted if the title is empty;
  - changes are saved onBlur;
  - pressing Escape cancels editing;

### - Toggling a todo status:

Toggles the completed status on TodoStatus change:

  - the todo is covered with a loader overlay while waiting for the API response;
  - the status changes on success;
  - shows an "Unable to update a todo" notification in case of API error;

Allows toggling the completed status of all the todos with the toggleAll checkbox:

  - the toggleAll button has active class only if all the todos are completed;
  - clicking toggleAll changes its status to the opposite one and sets this new status for all the todos;
  - it works the same as several individual updates of the todos which statuses were actually changed;
  - sends requests for the todos that were not changed;


### - Renaming a todo:

  Allows editing a todo title on double-click:

  - shows the edit form instead of the title and remove button;
  - saves changes on the form submit (press Enter);
  - saves changes when the field loses focus (onBlur);
  - if the new title is the same as the old one it cancels editing;
  - cancels editing on Esс key keyup event;
  - if the new title is empty it deletes the todo the same way the remove button does it;
  - if the title was changed, shows the loader while waiting for the API response;
  - updates the todo title on success;
  - shows "Unable to update a todo" in case of an API error or a deletion error message if attempting to delete the todo;

### Quick start guide

Instructions to start this project:

 - Clone repository: 

   ```
   git clone [repository]
   ```

 - Install NPM packages and dependencies:

   ```
   npm install
   ```

 - Run project on local server:

   ```
   npm start
   ```
