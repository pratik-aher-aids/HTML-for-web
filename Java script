function addTask() {
    let taskInput = document.getElementById("taskInput");
    let taskText = taskInput.value.trim();
    
    if (taskText === "") return;

    let li = document.createElement("li");
    li.innerHTML = `${taskText} <button class="delete" onclick="deleteTask(this)">X</button>`;
    li.onclick = function() {
        this.classList.toggle("completed");
    };

    document.getElementById("taskList").appendChild(li);
    taskInput.value = "";
}

function deleteTask(button) {
    button.parentElement.remove();
}
