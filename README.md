# Steps to run the application
Installing Node.js and npm
Download and Install Node.js: First, visit the official Node.js website to download the installer. Choose the LTS (Long Term Support) version for stability and extended support.
Install npm: Node.js installation includes npm (Node Package Manager), with essential for managing JavaScript packages.
Creating a New React App
Install Create React App: Open your terminal and run npm install -g create-react-app to install this utility globally.
Generate Your Project: Execute npx create-react-app my-app to create a new directory named ‘my-app’ with all the necessary setups.

Understanding the Project Structure
Explore Initial Setup: Navigate to your project directory and observe the default structure provided by Create React App. Key folders include ‘public’ for static assets, ‘src’ for source files, and ‘node_modules’ for dependencies.
Key Files: The ‘src’ folder contains ‘App.js’, the root component, and ‘index.js’, which renders the App component into the DOM.

Starting the Development Server
Launch the Server: In your project directory, run npm start to fire up the development server. This command compiles the app and opens it in your default web browser.
Automatic Refresh: Any changes you make in the source files will automatically refresh the app in the browser, thanks to the hot reloading feature

Creating the App Component File
Initialize the Component: Start by creating a new file in your project’s src/components directory. Name it App.js. This file will house your main App component, which serves as the entry point for your ToDo List application.
Define the App Component: Within App.js, define your App component as a functional component. Use the following basic structure to get started.

Importing Necessary Modules
React and ReactDOM: At the top of your App.js file, ensure you import React. This import is crucial as it allows you to use JSX and other React features.
Additional Components: If your application will use other custom components or third-party libraries, import them at the beginning of the file. For instance, if you are using Material-UI components, you might add.
CSS Files: To style your component, import the necessary CSS files at the top of your component file.

Rendering the First Component
Create Root Element: In your project’s src/index.js, set up the root for your React application by importing ReactDOM and pointing it to the appropriate DOM element:
Display the App Component: The ReactDOM.createRoot() method links your React application to an existing DOM element (typically a div with the id of ‘root’ in your public/index.html file). The root.render() method then renders your App component within this root element, displaying your initial UI on the page.

To manage the list of tasks within your TodoList component, utilize the useState hook from React. Start by initializing the state with an empty array or a default set of tasks.

This state will hold all the tasks you add, each represented by an object with properties such as id, text, and completed status.

For adding new tasks, handle user input with a controlled component approach.

Include an input field in your component’s return statement and bind it to the text state with onChange to capture user input dynamically.
To add tasks to your list, create an addTask function that constructs a new task object and updates the state.

Bind this function to a button’s onClick event within your component to trigger task addition.

Use the map function to iterate over the tasks array and display each task.

Each task is rendered as a list item within an unordered list, with buttons to mark it as complete or to delete it. Implement toggleCompleted and deleteTask functions to handle these actions, updating the tasks array accordingly.

By following these steps, you’ll have a functional TodoList component that allows users to add, display, complete, and delete tasks dynamically.

Props Overview: TodoItem receives task, deleteTask, and toggleCompleted as props. These functions are crucial for manipulating the task’s state from the parent component.
Functionality:
task: Contains details of a specific task.
deleteTask: Function to remove a task from the list.
toggleCompleted: Function to toggle the completion status of a task.
