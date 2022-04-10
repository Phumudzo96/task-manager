# Capstone-II
In this task, you will be creating a program for a small business that can
help it to manage tasks assigned to each member of the team. Copy the
template program provided, Task19template.py, and rename it
task_manager.py in this folder. This template has been provided to make
this Task a little easier for you. Your job is to open and then modify the
template to achieve the rest of the compulsory Task set out below.
Remember to save your work as you go along.

●This program will work with two text ﬁles, user.txt and tasks.txt. Open
each of the ﬁles that accompany this project and take note of the
following:

tasks.txt stores a list of all the tasks that the team is working on.
Open the tasks.txt ﬁle that accompanies this project. Note that
this text ﬁle already contains data about two tasks. The data for
each task is stored on a separate line in the text ﬁle. Each line
includes the following data about a task in this order:

■ The username of the person to whom the task is assigned.

■ The title of the task.

■ A description of the task.

■ The date that the task was assigned to the user.

■ The due date for the task.

■ Either a ‘Yes’ or ‘No’ value that speciﬁes if the task has been completed yet.

user.txt stores the username and password for each user that has
permission to use your program (task_manager.py). Open the
user.txt ﬁle that accompanies this project. Note that this text ﬁle
already contains one default user that has the username, ‘admin’and the password, ‘adm1n’. The username and password for each
user must be written to this ﬁle in the following format:
■ First, the username followed by a comma, a space and then the password.
■ One username and corresponding password per line.

● Your program should allow your users to do the following:

Login. The user should be prompted to enter a username and
password. A list of valid usernames and passwords are stored in a
text ﬁle called user.txt. Display an appropriate error message if the
user enters a username that is not listed in user.txt or enters a valid
username but not a valid password. The user should repeatedly be
asked to enter a valid username and password until they provide
appropriate credentials.
The following menu should be displayed once the user has
successfully logged in:

If the user chooses ‘ r’ to register a user, the user should be
prompted for a new username and password. The user should also
be asked to conﬁrm the password. If the value entered to conﬁrm
the password matches the value of the password, the username
and password should be written to user.txt in the appropriate
format.

If the user chooses ‘a’ to add a task, the user should be prompted to
enter the username of the person the task is assigned to, the title of
the task, a description of the task and the due date of the task. The
data about the new task should be written to tasks.txt. The date on
which the task is assigned should be the current date. Also assume
that whenever you add a new task, the value that indicates whether
the task has been completed or not is ‘No’.

If the user chooses ‘ va’ to view all tasks, display the information for
each task on the screen in an easy to read format.

If the user chooses ‘ vm’ to view the tasks that are assigned to them,
only display all the tasks that have been assigned to the user that is
currently logged-in in a user-f riendly,  easy to read manner

o reg_user — that is called when the user selects ‘r’ to register a user.

o add_task — that is called when a user selects ‘a’ to add a new task.

o view_all — that is called when users type ‘ va’ to view all the tasks
listed in ‘tasks.txt’.

o view_mine — that is called when users type ‘ vm’ to view all the
tasks that have been assigned to them.

● Modify the function called reg_user to make sure that you don’t duplicate
usernames when you add a new user to user.txt. If a user tries to add a
username that already exists in user.txt, provide a relevant error message
and allow them to try to add a user with a different username.

● Add the following functionality when the user selects ‘ vm’ to view all the
tasks assigned to them:

o Display all tasks in a manner that is easy to read. Make sure that
each task is displayed with a corresponding number which can be
used to identify the task.

o Allow the user to select either a speciﬁc task by entering a number
or input ‘-1’ to return to the main menu.

o If the user selects a speciﬁc task, they should be able to choose to
either mark the task as complete or edit the task. If the user
chooses to mark a task as complete, the ‘Yes’/ ’No’ value that
describes whether the task has been completed or not should be
changed to ‘Yes’. When the user chooses to edit a task, the
username of the person to whom the task is assigned or the due
date of the task can be edited. The task can only be edited if it has
not yet been completed.

● Add an option to generate reports to the main menu of the application.
The menu for the admin user should now look something like this:

● When the user chooses to generate reports, two text ﬁles, called
task_overview.txt and user_overview.txt, should be generated. Both
these text ﬁles should output data in a user-f riendly, easy to read manner.

o task_overview.txt should contain:

▪ The total number of tasks that have been generated and
tracked using the task_manager.py.

▪ The total number of completed tasks.

▪ The total number of uncompleted tasks.

▪ The total number of tasks that haven’t been completed and
that are overdue.

▪ The percentage of tasks that are incomplete.

▪ The percentage of tasks that are overdue.

o user_overview.txt should contain:

▪ The total number of users registered with task_manager.py.

▪ The total number of tasks that have been generated and
tracked using the task_manager.py.

▪ For each user also describe:

▪ The total number of tasks assigned to that user.

▪ What percentage of the total number of tasks have
been assigned to that user?

▪ What percentage of the tasks assigned to that user
have been completed?

▪ What percentage of the tasks assigned to that user
must still be completed?

▪ What percentage of the tasks assigned to that user
have not yet been completed and are overdue?

● Modify the menu option that allows the admin to display statistics so that
the reports generated are read f rom task_overview.txt and
user_overview.txt and displayed on the screen in a user-f riendly manner.
If these text ﬁles don’t exist (because the user hasn’t selected to generate
them yet), ﬁrst call the code to generate the text ﬁles.
