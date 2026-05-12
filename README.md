# Ex03 To-Do List using JavaScript

## Date: 11-05-2026 ##

## NAME: SHIV SUJAN S R ##

## DEPT: B.E(CSE) ##

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM

## HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To-Do List</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h2>To-Do List ✅</h2>
        <input type="text" id="taskInput" placeholder="Enter a task...">
        <button onclick="addTask()">Add</button>
        <div id="taskList"></div>
    </div>
    <footer>
        <p>&copy; 2026 SHIVSUJAN S R 212223040194| All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
```

## STYLE.CSS
```
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: linear-gradient(to right, #372c8b, #686ca0);
    font-family: Arial, sans-serif;
}
.container {
    background: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    width: 300px;
    text-align: center;
}
input {
    width: 70%;
    padding: 8px;
    margin-right: 5px;
}
button {
    background: #ff4d4d;
    color: white;
    border: none;
    padding: 8px 12px;
    cursor: pointer;
    border-radius: 5px;
}
.task {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #f8d7da;
    padding: 8px;
    margin-top: 5px;
    border-radius: 5px;
}
footer {
    position: absolute;
    bottom: 10px;
    width: 100%;
    text-align: center;
    color: white;
    font-size: 14px;
}
```

## JAVASCRIPT
```
function addTask() {
    let taskInput = document.getElementById('taskInput');
    let taskText = taskInput.value.trim();
    if (taskText === '') return;
    
    let taskDiv = document.createElement('div');
    taskDiv.classList.add('task');
    taskDiv.innerHTML = `<span>${taskText}</span> <button onclick="this.parentElement.remove()">Delete</button>`;
    
    document.getElementById('taskList').appendChild(taskDiv);
    taskInput.value = '';
}
```

## OUTPUT

<img width="1920" height="1080" alt="Screenshot 2026-05-12 154745" src="https://github.com/user-attachments/assets/afae93fb-7bcd-46fe-beef-4a1e83d51141" />
<img width="1920" height="1080" alt="Screenshot 2026-05-12 155006" src="https://github.com/user-attachments/assets/ecc6ed63-a6ff-4de3-ba51-9e76c2c51f64" />
<img width="1920" height="1080" alt="Screenshot 2026-05-12 155218" src="https://github.com/user-attachments/assets/c5cc5bda-3cd9-4348-8037-62b2ecee6fec" />

## RESULT
The program for creating To-do list using JavaScript is executed successfully.
