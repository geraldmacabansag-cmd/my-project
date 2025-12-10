Name: Gerald Macabansag
Section: [BSIT-3A]

Project Title: Smart Interactive Dashboard (A Note Taking Dashboard0
Language Used: Python (PyQt5)

What is PyQt5?
PyQt5 is a Python library that lets you create desktop applications with windows, buttons, tables, and other visual tools. It reacts to user actions using signals and slots. It is easy to use and works on different operating systems like Windows, Mac, and Linux.

Features of the Dashboard (Simple English)
1. Debounced Search Bar
The search bar waits for 500ms after the user stops typing before it runs the search. This prevents too many searches while typing. It updates a label with the text you typed and filters the table rows. This makes searching smooth and fast.

2. Throttled Scroll Event
When you scroll the table, the dashboard shows the scroll position as a percentage. The table header changes color while scrolling. After 500ms of no movement, the header returns to normal. This prevents too many scroll updates and keeps the UI fast.

3. Buttons and Basic UI Events
Buttons like Add Notes, Open, Delete, Change Theme, Reset Dashboard, and Exit all perform their own actions. Each button is connected to a function that runs when clicked. This shows how events work in PyQt5. It also includes warnings when actions are not allowed, like deleting without selecting a row.

4. Data-Driven Panel
The task table gets its data from a SQLite database. When you add, edit, or delete a task, the table updates right away. This makes sure the information is always correct. It shows how the UI and database work together.

5. Custom Events + Notification Area
The dashboard has custom signals such as taskAdded, taskUpdated, taskDeleted, and themeChanged. When these events happen, a message appears in the notification area with a timestamp. This lets users see all actions clearly and understand what changed.

6. Error Handling
If the user tries to do something invalid, like opening a note without selecting one, the app shows a warning message. This prevents mistakes and keeps the app from crashing. It guides the user to make correct actions.

7. Timer / Clock Feature
A digital clock at the top shows the current time and date. It updates every second using a timer. This displays live system time inside the dashboard.

8. Reset Dashboard Button
The Reset button returns the dashboard to its default state. It clears the search bar, scrolls the table back to the top, and also clears the notification area. This gives the user a clean and fresh view of the dashboard. It is helpful when the user wants to remove old logs and reset the view quickly.
