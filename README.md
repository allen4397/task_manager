# task_manager

GitHub peer pressured me into adding a README... so, here it is.

This is a tutorial prework for Mod 2 at Turing.

Here is also the answers to the questions at the end:

1. Define CRUD

Create, Read, Update and Destroy. It is referring to elements in the database. All of this is done through the controller and the view contains what the user sees and reflects those changes.

2. Why do we use set method_override: true?

This makes it so you can call methods that can't be interpreted by html in the traditional way.

3. Explain the difference between value and name in this line: <input type='text' name='task[title]' value="<%= @task.title %>"/>.

The name is getting the value from the task hash that has the key "title", the value is running ruby code to access the title of an instance of a task using the #title method (included in the attr_reader).

4. What are params? Where do they come from?

Params are the values taken from the user in the input section of an html document.

5. Check out your routes. Why do we need two routes each for creating a new Task and editing an existing Task?

When a new Task is created, it needs to update the database and the view. The same is true for editing a document. From a user perspective, a user needs to click new or edit which leads to slightly different routes and then they need to submit which goes down two separate routes as well.
