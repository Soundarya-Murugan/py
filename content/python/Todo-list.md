---
title: Todo-List
date: 2024-11-29
author: Your Name
cell_count: 7
score: 5
---

```python
# Simple To-Do List Manager

def display_menu():
    print("\n=== To-Do List Manager ===")
    print("1. View To-Do List")
    print("2. Add a Task")
    print("3. Mark Task as Completed")
    print("4. Delete a Task")
    print("5. Exit")



```


```python
def view_tasks(tasks):
    if not tasks:
        print("\nYour to-do list is empty!")
    else:
        print("\nTo-Do List:")
        for i, task in enumerate(tasks, 1):
            status = "✓" if task['completed'] else "✗"
            print(f"{i}. {task['title']} [{status}]")


```


```python
def add_task(tasks):
    title = input("\nEnter the task title: ")
    tasks.append({"title": title, "completed": False})
    print("Task added successfully.")


```


```python
def mark_task_completed(tasks):
    view_tasks(tasks)
    if tasks:
        task_num = int(input("\nEnter the task number to mark as completed: ")) - 1
        if 0 <= task_num < len(tasks):
            tasks[task_num]["completed"] = True
            print("Task marked as completed.")
        else:
            print("Invalid task number.")


```


```python
def delete_task(tasks):
    view_tasks(tasks)
    if tasks:
        task_num = int(input("\nEnter the task number to delete: ")) - 1
        if 0 <= task_num < len(tasks):
            removed_task = tasks.pop(task_num)
            print(f"Task '{removed_task['title']}' deleted.")
        else:
            print("Invalid task number.")


```


```python
def main():
    tasks = []
    while True:
        display_menu()
        choice = input("\nEnter your choice (1-5): ")

        if choice == '1':
            view_tasks(tasks)
        elif choice == '2':
            add_task(tasks)
        elif choice == '3':
            mark_task_completed(tasks)
        elif choice == '4':
            delete_task(tasks)
        elif choice == '5':
            print("Goodbye!")
            break
        else:
            print("Invalid choice, please try again.")

# Run the main function to start the program
main()
```

    
    === To-Do List Manager ===
    1. View To-Do List
    2. Add a Task
    3. Mark Task as Completed
    4. Delete a Task
    5. Exit


    
    Enter your choice (1-5):  1


    
    Your to-do list is empty!
    
    === To-Do List Manager ===
    1. View To-Do List
    2. Add a Task
    3. Mark Task as Completed
    4. Delete a Task
    5. Exit


    
    Enter your choice (1-5):  2
    
    Enter the task title:  Check Task


    Task added successfully.
    
    === To-Do List Manager ===
    1. View To-Do List
    2. Add a Task
    3. Mark Task as Completed
    4. Delete a Task
    5. Exit


    
    Enter your choice (1-5):  3


    
    To-Do List:
    1. Check Task [✗]


    
    Enter the task number to mark as completed:  3


    Invalid task number.
    
    === To-Do List Manager ===
    1. View To-Do List
    2. Add a Task
    3. Mark Task as Completed
    4. Delete a Task
    5. Exit



```python

```


---
**Score: 5**
