<h1 style="text-align: center;"># My ToDo List Creation</h1>

Previously, we had an assignment to create a ToDo list with Javascript. 

Recently I had to do it again using Python. Here was my process:

First code:

```python
todos = [] 
```
## This is a empty list which will be filled with the inputs

```python
def show_the_todos():
    if not todos:
        print('Sorry there is no Todos.') 
    else:
        for i, todo in enumerate(todos, start = 1): 
            print(f'{i}. {todo}')
```
## This was used to show the user the different Todos that later on will be added.

``` python
while True: 
    show_the_todos() 
    user_input = input('Would you like to add (type: "add") or remove (type: "remove") a todo?: ') 
    if user_input == "add": 
        new_todo = input('What is your new todo?: ') 
        todos.append(new_todo) t
    elif user_input == "remove":
        if len(todos) == 0: 
            print('Sorry you have no todos already.') 
        else:
            remove_input = int(input("What would you like to remove? (give number of todo): " )) 
            if remove_input <= 0: 
                print("Sorry You must input a number on the list.") 
            else: 
                del todos[remove_input - 1] 
 ```
 ## This may look a little confusion but don't let all the code get to you.
---
<p style="text-align: center;">- This part of the code is basically saying the code will run for ever.</p>
<p style="text-align: center;">- This part of the code is basically saying the code will run for ever.</p>

