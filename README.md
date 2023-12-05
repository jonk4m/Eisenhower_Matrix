# Eisenhower_Matrix
Simple Program to Organize a Text-Based list of Tasks by How Important/Urgent They are via a Ranking System

<details>
<summary> What is an Eisenhower Matrix? </summary>

## What is an Eisenhower Matrix?
TODO:
- Provide links to articles 
- Provide brief description of why it's useful 

</details>
<details>
<summary> Functionality </summary>

## Functionality 

- Mention that this is not a note-taking resource. This is also not meant to replace the usefulness of a calendar. 

<details>
<summary> Entering Tasks </summary>

### Entering Tasks
The user needs to enter a list of tasks, either by selecting a text file filled with tasks (each on it's own line), or by manually typing them into the program one-by-one. 

</details>
<details>
<summary> Ranking Process </summary>

### Ranking Process
The user can select from the menu to rank the tasks by either importance or urgency. This will prompt a question-answer series where the program asks the user to select from two tasks which one is more important/urgent. Once the user has answered all the questions, the program will rank the tasks based on the responses. 

#### Example
Say the user enters the following tasks in the following order: 
Wash Car
Go on Walk
Laundry
Then the user asks to rank the tasks by importance. The program will then prompt:
Which is more important? 'Go on walk' or 'Laundry'?
If the user selects 'Laundry' then that task will receive a lower ranking than the other. 

### Completed List
The tasks can only be organized into an Eisenhower Matrix prioritized list once the user has ranked them in both importance and urgency. 

Once the user has ranked all tasks, the tasks are assigned a 2 dimensional ranking where the lowest ranking in both importance and urgency is (0,0). The next most important, but equally as urgent task, is ranked ().

This reveals a matrix with coordinates:

```
  Least │    (0,1)               (1,1)
        │ Most Important      Leas Important
        │ Less Urgent         Less Urgent
Urgency │
        │    (0,0)               (1,0)
        │ Most Important      Less Important
        │ Most Urgent         Less Urgent
   Most ▼
         ◄───────────────────────────────────
         Most         Importance        Least
```
The final list is next sorted starting from the (0,0) coordinate working linearly to the top right of the matrix. 

</details>
</details>
<details>
<summary> Install </summary>

# Install

TODO

</details>
<details>
<summary> Features </summary>

# Features

TODO 

<details>
<summary> Possible Future Features </summary>

  - Provide default sorting patterns for the user as a checkbox
    - Example: Sort list of tasks by:
      - Easiest
      - Most Important
      - Most Urgent
      - 2nd Easiest
      - 2nd Most Important
      - 2nd Most Urgent
      - etc.
  - Create a standard file type like .priority
    - Make it standard text readable in markdown format
      - use (0,0,0) before each task for (Importance, Urgency, Ease) sorting
      - use (C,0,0,0) before each complete task 
    - Make it have comments ignored with something like #ignore this comment, but probably not the '#' because that might mess with Markdown format
    - Possible improvement would be allowing for nested tasks (ideally in markdown format)
    - Include the time/date of the last ranking in the file somewhere 
  - Make it so you can send an executable to a customer, along with a .priority file, and they can run it to provide the developer with the resulting .priority file they can then use to determine the future of the project.
    - Providing a customer specific menu on startup (Are you ___ Customer?) and then proceeding based on that would be a nice way to handle this. 
  - Allow for reading in a .priority file, then dynamically adding tasks that are then sorted or not.
    - Maybe have an indicator next to unsorted tasks and a progress bar that always shows how many tasks in % are sorted or not. 
  - Biggest thorns to deal with where this program is currently lacking:
    - handling nested tasks
    - handling tasks that rely on other tasks being accomplished before they can be accomplished. Call it, sequential reliance on another task. This would theoretically change the order of importance.
      - For example, if Task B MUST be done before Task A (i.g. Task B is implement playing a file, while Task A is to add a play button) then the user selecting Task B to have a higher importance than task A should raise the importance of Task A since it has to be done first.
      - Another example: It would be confusing for the customer to rank the importance of "Buttons have tooltips" and "Buttons exist" when the latter clearly has to come first. 
  - OS independent: Is there a way to compile several executables that are wrapped in one executable which then picks the correct executable to use based on the OS calling it?
  - Runnable in a web browser. 
  - Runnable on mobile. 
  - Integration with Todoist, Google Tasks, or others possible. 
  - Making the ranking process "smarter" by mimicking techniques similar to active recall and spaced repetition. 
    - Example: User has 50 tasks. Ranking them all by importance should, at some point, loop back to the beginning of the list to heighten the likelyhood that Task 1 being ranked higher than Task 49 is true. Basically, even if all tasks are technically ranked in order, there should be some overlap of tasks the user is asked to rank to ensure a higher degree of certainty.
  - Make this a linux package that can be installed by most package managers
  - Thus far the thinking has been that each project would be it's own text file, but it would be cool to rank ALL tasks a user has, including tasks from multiple projects, into one big ranked list.
  - Giving every task a unique ID makes the most sense for sorting, organizing, uniquely identifying, etc.
    - I wonder if you could sort projects by having a known table of ID's for a given project, task's subtasks, or even filters. So theoretically you could create a filter for a person you've delegated tasks and then rank the tasks for that person specifically without separating the tasks into a different project.
  - Would be really cool to see if there's a "mode" you could apply to this program to gear it more towards learning a topic.
  - Add a "I'm feeling lucky" function that selects a random task for you to do
  - Option to export the list in such a way that you can easily print the tasks out on playing cards and they're numbered in order plus other info like who it's assigned to
  - Option to print most important+urgent task on thermal printer
  - Features that apply to a team aka shared document
    - Some way of syncing a document. Probably best if it uses github or something under the hood
    - Ideally there's a way for phone user's to use this. Ranking from your phone would be a fun pass-time.
    - Definitely need to add an option for assigning tasks to different people(s).
    - Would be cool to add a feature where if multiple people rank a task differently, it flags it as a point of contention to be hashed out.
    - 
  
</details>

</details>
<details>
<summary> Screenshots </summary>

# Screenshots 

TODO 

</details>
<details>
<summary> Acknowledgements </summary>

# Acknowledgements 

TODO:
- Add Asciiflow
- Add FTXUI
- Add 

</details>
