# Eisenhower_Matrix
Simple Program to Organize a Text-Based list of Tasks by How Important/Urgent They are via a Ranking System

## Functionality 

### Entering Tasks
The user needs to enter a list of tasks, either by selecting a text file filled with tasks (each on it's own line), or by manually typing them into the program one-by-one. 

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

'''
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
'''
