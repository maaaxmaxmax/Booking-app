# Booking-app
A web-based application designed for managing bookings and task assignments. The app provides an intuitive interface to book time slots and manage a to-do list with tasks that can be assigned to users.

# Features

# Booking System
* View a monthly calendar with existing bookings.
* Book time slots (e.g., "Morgon", "Eftermiddag", "Kväll") for specific dates.
* Display detailed information for each booking when clicked.
* Prevent overbooking: Maximum of 4 bookings per day.
* Manage bookings through a responsive calendar.

  
# To-Do List
* Create tasks with a title and description.
* Assign tasks to a specific person (one task can only be assigned to one user).
* View assigned/unassigned tasks dynamically.
* Delete tasks when completed.

  
# Technologies Used
# Frontend:

* React.js for building the user interface.
* React Big Calendar for calendar visualization.
* Axios for HTTP requests.
* React Modal for displaying booking details.
  
# Backend:
* Node.js with Express.js for API handling.
* MongoDB as the database for storing bookings and tasks.
* Mongoose for MongoDB schema and query handling.

  
# Hosting:
* MongoDB Atlas for cloud-based database hosting.
* Localhost (during development) for API and frontend testing.

# How It Works
# Booking System

1. Booking a Time Slot:

- Select a date from the calendar.
- Choose a time slot (Morgon, Eftermiddag, Kväll).
- Fill in the required details: Name, Email, Phone.
- If the maximum number of bookings (4) is reached, booking for that day will be denied.

  
2. View Bookings:

- Existing bookings are displayed on the calendar.
- Click on a booking to see detailed information (date, time, user details).


# To-Do List
1. Create Tasks:
- Add tasks with a title and description via the task creation form.

2. Assign Tasks:

- Assign tasks to yourself or others by clicking the "Assign" button.
- Prevents double assignments for tasks.

3. Manage Tasks:

- View all tasks, filtered by assigned/unassigned.
- Delete completed tasks to keep the list updated.


# Installation
* Prerequisites
- Node.js and npm installed.
- MongoDB Atlas account (or a local MongoDB instance).
![image](https://github.com/user-attachments/assets/e2634b05-66a2-4201-98b5-9fd84afba365)


# API Endpoints
# Bookings
* POST /api/book - Create a new booking.
* GET /api/bookings/:date - Fetch bookings for a specific date.
* GET /api/bookings/:year/:month - Fetch bookings for a specific month.

# Tasks
* GET /api/tasks - Fetch all tasks.
* POST /api/tasks - Create a new task.
* PUT /api/tasks/:id/assign - Assign a task to a user.
* DELETE /api/tasks/:id - Delete a specific task.

  
# Screenshots
![image](https://github.com/user-attachments/assets/6a97608a-e972-44ad-94a3-d269fc85f47d)
![image](https://github.com/user-attachments/assets/60c31621-3d4e-4bcf-8449-3680895f9640)
![image](https://github.com/user-attachments/assets/b255d4fe-3b01-409a-b4f5-24e29a9f5c9e)


* This project is not finnished
