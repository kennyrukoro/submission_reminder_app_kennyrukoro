markdown
Copy
# Submission Reminder App

This is a simple shell script application that reminds students about upcoming assignment deadlines. The application checks a list of students and their submission statuses, then sends reminders to those who haven't submitted their assignments yet.

## Directory Structure

The application follows this directory structure:
submission_reminder_{yourName}/
├── app/
│ └── reminder.sh
├── modules/
│ └── functions.sh
├── assets/
│ └── submissions.txt
├── config/
│ └── config.env
└── startup.sh

Copy

## Files

- **`app/reminder.sh`**: The main script that checks student submissions and sends reminders.
- **`modules/functions.sh`**: Contains helper functions used by `reminder.sh`.
- **`assets/submissions.txt`**: A CSV file containing student names, assignments, and submission statuses.
- **`config/config.env`**: Configuration file for the application (e.g., assignment name and days remaining).
- **`startup.sh`**: A script to start the reminder application.

## How to Run the Application

### Prerequisites

- Ensure you have `bash` installed on your system.
- The script is designed to run on Linux or macOS.

### Steps to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourUsername/submission_reminder_app_githusername.git
Navigate to the Project Directory:

bash
Copy
cd submission_reminder_app_githusername
Run the create_environment.sh Script:
This script will set up the directory structure and populate the files.

bash
Copy
./create_environment.sh
When prompted, enter your name. This will create a directory named submission_reminder_{yourName}.

Navigate to the Created Directory:

bash
Copy
cd submission_reminder_{yourName}
Run the Application:
Use the startup.sh script to start the reminder application:

bash
Copy
./startup.sh
This will display a list of students who haven't submitted their assignments yet.

Example Output
When you run the application, you should see output similar to this:

Copy
Assignment: Shell Navigation
Days remaining to submit: 2 days
--------------------------------------------
Checking submissions in ../assets/submissions.txt
Reminder: Chinemerem has not submitted the Shell Navigation assignment!
Reminder: Divine has not submitted the Shell Navigation assignment!
Reminder: John has not submitted the Shell Navigation assignment!
Reminder: Alice has not submitted the Shell Navigation assignment!
Reminder: Charlie has not submitted the Shell Navigation assignment!
Reminder: Eve has not submitted the Shell Navigation assignment!
Reminder: Grace has not submitted the Shell Navigation assignment!
Reminder: Ivy has not submitted the Shell Navigation assignment!
Reminder: Karen has not submitted the Shell Navigation assignment!
Reminder: Mona has not submitted the Shell Navigation assignment!
Adding More Students
To add more students, edit the assets/submissions.txt file. Follow the format:

Copy
student, assignment, submission status
StudentName, AssignmentName, submitted/not submitted
Customizing the Assignment
You can change the assignment name and days remaining by editing the config/config.env file:

Copy
ASSIGNMENT="Your Assignment Name"
DAYS_REMAINING=5
