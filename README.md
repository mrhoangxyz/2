# 2
Ứng dụng "To-Do List" (JavaScript)
const todoList = document.getElementById("todo-list");
const todoInput = document.getElementById("todo-input");
const addButton = document.getElementById("add-button");

addButton.addEventListener("click", () => {
    const todoText = todoInput.value;
    if (todoText) {
        const todoItem = document.createElement("li");
        todoItem.textContent = todoText;
        todoList.appendChild(todoItem);
        todoInput.value = "";
    }
});
