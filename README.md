# ✅ Todo App (JavaScript)

A simple and responsive **Todo Application** built using **HTML, CSS, and JavaScript**.  
This project helps users manage daily tasks by adding, completing, and deleting todos with data saved in browser storage.

---

## 🚀 Features

- Add new tasks
- Mark tasks as completed
- Delete tasks
- Data stored in LocalStorage (persists after refresh)
- Simple and clean UI
- Fully responsive design
- Beginner-friendly JavaScript project

---

## 🛠️ Tech Stack

- HTML5
- CSS3
- JavaScript (Vanilla JS)
- LocalStorage API

---

## 📁 Project Structure

```

todo-app-js/
│── index.html
│── style.css
│── script.js
│── images/
│   ├── screenshot1.png
│   ├── screenshot2.png
│── README.md

````id="todostructure01"

---

## 🖼️ Screenshots

### Main Interface
![Todo App Home](images/screenshot1.png)

### Task Management View
![Todo App Tasks](images/screenshot2.png)

---

## ▶️ Live Project / GitHub

🔗 Repository: https://github.com/santosh312-dev/todo-app-js

---

## 💡 How It Works

- User adds a task in input field
- Task is stored in an array
- Data is saved in `localStorage`
- Tasks are rendered dynamically on the page
- Clicking delete removes task from storage

Example logic:

```javascript id="todolistlogic01"
let todos = JSON.parse(localStorage.getItem("todos")) || [];

function addTodo(task) {
    todos.push({ text: task, completed: false });
    localStorage.setItem("todos", JSON.stringify(todos));
    renderTodos();
}

function deleteTodo(index) {
    todos.splice(index, 1);
    localStorage.setItem("todos", JSON.stringify(todos));
    renderTodos();
}

function toggleTodo(index) {
    todos[index].completed = !todos[index].completed;
    localStorage.setItem("todos", JSON.stringify(todos));
    renderTodos();
}
```

---

## 🎯 Future Improvements

- Drag and drop task reordering
- Due dates and reminders
- Dark mode support
- Task categories/filters
- Cloud sync support

---

## 👨‍💻 Author

Built with ❤️ using HTML, CSS, and JavaScript.

GitHub: https://github.com/santosh312-dev

---

## 📜 License

This project is open-source and free to use.
