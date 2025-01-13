# Booking-app
A web-based application designed for managing bookings and task assignments. The app provides an intuitive interface to book time slots and manage a to-do list with tasks that can be assigned to users.

Features
Booking System
View a monthly calendar with existing bookings.
Book time slots (e.g., "Morgon", "Eftermiddag", "Kväll") for specific dates.
Display detailed information for each booking when clicked.
Prevent overbooking: Maximum of 4 bookings per day.
Manage bookings through a responsive calendar.
To-Do List
Create tasks with a title and description.
Assign tasks to a specific person (one task can only be assigned to one user).
View assigned/unassigned tasks dynamically.
Delete tasks when completed.
Technologies Used
Frontend:

React.js for building the user interface.
React Big Calendar for calendar visualization.
Axios for HTTP requests.
React Modal for displaying booking details.
Backend:

Node.js with Express.js for API handling.
MongoDB as the database for storing bookings and tasks.
Mongoose for MongoDB schema and query handling.
Hosting:

MongoDB Atlas for cloud-based database hosting.
Localhost (during development) for API and frontend testing.
How It Works
Booking System
Booking a Time Slot:

Select a date from the calendar.
Choose a time slot (Morgon, Eftermiddag, Kväll).
Fill in the required details: Name, Email, Phone.
If the maximum number of bookings (4) is reached, booking for that day will be denied.
View Bookings:

Existing bookings are displayed on the calendar.
Click on a booking to see detailed information (date, time, user details).
To-Do List
Create Tasks:

Add tasks with a title and description via the task creation form.
Assign Tasks:

Assign tasks to yourself or others by clicking the "Assign" button.
Prevents double assignments for tasks.
Manage Tasks:

View all tasks, filtered by assigned/unassigned.
Delete completed tasks to keep the list updated.
Installation
Prerequisites
Node.js and npm installed.
MongoDB Atlas account (or a local MongoDB instance).
Steps
Clone the repository:

bash
Kopiera kod
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install dependencies:

bash
Kopiera kod
npm install
Create a .env file in the root directory:

plaintext
Kopiera kod
MONGO_URI=your-mongodb-uri
PORT=5000
Start the backend server:

bash
Kopiera kod
npm run server
Start the frontend:

bash
Kopiera kod
npm run client
Open the app in your browser:

plaintext
Kopiera kod
http://localhost:3000
API Endpoints
Bookings
POST /api/book - Create a new booking.
GET /api/bookings/:date - Fetch bookings for a specific date.
GET /api/bookings/:year/:month - Fetch bookings for a specific month.
Tasks
GET /api/tasks - Fetch all tasks.
POST /api/tasks - Create a new task.
PUT /api/tasks/:id/assign - Assign a task to a user.
DELETE /api/tasks/:id - Delete a specific task.
Screenshots
Booking System

To-Do List

Future Improvements
User authentication to track individual bookings and tasks.
Task filtering and sorting by priority.
Integration with external APIs for advanced scheduling.
