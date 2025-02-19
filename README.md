# Submission Reminder System

## Project Overview
The **Submission Reminder System** is a shell script-based application that helps students keep track of their assignment deadlines. It automatically generates a directory structure and necessary files, allowing users to receive personalized reminders about their pending submissions.

## Features
- Automatically creates a structured directory for the reminder system.
- Allows users to input their name during setup, generating a personalized directory.
- Displays a personalized reminder for the user when the system starts.
- Shows a list of all students and their submission statuses.
- Ensures users whose names are not in the records receive an appropriate message.
- Provides an easy-to-run startup script to check assignment reminders.

## Directory Structure
```
submission_reminder_{username}/
│-- app/
│   │-- reminder.sh
│-- modules/
│   │-- functions.sh
│-- assets/
│   │-- submissions.txt
│-- config/
│   │-- config.env
│-- startup.sh
```

## Installation and Setup
1. Clone the repository or download the script files.
2. Open a terminal and navigate to the project directory.
3. Run the environment setup script:
   ```bash
   bash create_environment.sh
   ```
   - The script will prompt for your name and create a personalized directory.
4. Navigate to the generated directory:
   ```bash
   cd submission_reminder_{yourName}
   ```
5. Run the startup script to check assignment reminders:
   ```bash
   ./startup.sh
   ```

## Usage
- Upon running `startup.sh`, the script will:
  - Display your personalized reminder if your name exists in the submission records.
  - Show a list of all students and their submission statuses.
  - Notify users if their name is not found in the records.

## Sample Submission Record (submissions.txt)
name submission reminder
```

## Customization
You can modify `config.env` to change the assignment name and deadline:
```bash
ASSIGNMENT="New Assignment"
DAYS_REMAINING=5
```

## Requirements
- A Linux/macOS terminal (or WSL on Windows)
- Bash shell

## Contributing
If you'd like to improve this project, feel free to fork the repository and submit a pull request!

## License
This project is open-source and available under the MIT License.

 
