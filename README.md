# React ToDo App

## Overview

The React ToDo App is a user-friendly task management application designed to help users stay organized and productive. It provides a soothing and visually appealing user interface, along with a range of features to enhance the task management experience. The ToDo App was developed using React and TypeScript, focusing on advanced state management, API integration, and user interaction enhancements. The app enables users to efficiently manage their tasks, supporting features like adding, deleting, updating, and toggling task status. The project involved converting pre-made HTML and CSS markups into a fully functional, interactive application, integrating complex UI behaviors with robust API handling.

## [Check the live demo here](https://alina-kabanets.github.io/react-js_todo-app-with-api/)


![preview img](/description/todoapp.gif)

![preview img](/description/edittodo.gif)


## Technologies:

  - React functional components;
  - useEffect, useState, useContext, useDispatch, useRef, custom hooks;
  - useReducer for a better understanding of what is under the hood of Redux;
  - Local storage, refactored to using fetch from API;
  - GET, DELETE, PATCH, POST methods for working with the API;
  - Promises, refactored to async/await syntax;
  - TypeScript types and enums;
  - React Transition Groups;


## Key Contributions:

### React Development:
Utilized React functional components, incorporating hooks such as useEffect, useState, useContext, useReducer, and custom hooks to manage component state and side effects.

### TypeScript Integration:
Implemented TypeScript for enhanced type safety, using types, interfaces, and enums to define component props and application state, ensuring robust code quality and reducing runtime errors.

### API Interaction: 
Handled data persistence with API server using GET, POST, PATCH, and DELETE methods. Applied async/await syntax for cleaner, more readable asynchronous code, and managed API calls with error handling and user feedback.

### State Management: 
Explored useReducer to deepen understanding of Redux-like state management patterns and used useDispatch for controlled state updates.

### UI/UX Enhancements:
Implemented smooth UI transitions using React Transition Groups, improving user experience by providing visual feedback on task operations.

### Local Storage: 
Initially integrated local storage for task persistence, later refactoring to sync data directly with the API server, ensuring data consistency across user sessions.

### Error Handling & Notifications:
Developed user-friendly error handling mechanisms, displaying appropriate notifications for scenarios like empty task titles, API failures, and task update errors.




## Features Implemented:


### Adding a Todo: 
Enabled users to add tasks with validation, API integration for task creation, and real-time UI updates using temporary task states with loaders.

### Deleting Todos:
Implemented task deletion with immediate UI feedback and error handling, including batch deletion for completed tasks.

### Toggling Todo Status:
Allowed users to toggle task completion status with overlay loaders and synchronized status updates with the backend.

# Renaming Todos: 
Provided in-place task renaming functionality with support for keyboard events, API integration, and rollback on errors.

### Bulk Operations: 
Developed bulk operations like toggling all task statuses and clearing completed tasks with synchronized API requests and error handling.



## 🤝 **Contributing**

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or submit feedback.


## 📧 **Contact**

If you have any questions or suggestions, feel free to reach out:

LinkedIn: [Alina Kabanets](https://www.linkedin.com/in/alina-kabanets/)

GitHub: [alina-kabanets](https://github.com/alina-kabanets)



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
