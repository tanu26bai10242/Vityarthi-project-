# Python Alarm System

A simple terminal-based Python project for adding, viewing, deleting, and checking alarms.

## Features

- Add an alarm with a time and label
- View saved alarms
- Delete alarms
- Check alarms against the current time
- Validate `HH:MM` time format
- Prevent duplicate alarms
- Store alarm data locally in a text file

## How to Run

Make sure Python 3 is installed.

From the project directory, run:

```bash
python main.py
```

The program will open in the terminal and provide a menu for managing alarms.

## Project Structure

```text
python_alarm_system/
│
├── data/
│   └── alarms.txt
│
├── main.py
├── alarm.py
├── database.py
├── README.md
├── statement.md
├── TESTING.md
├── requirements.txt
└── .gitignore
```

## File Description

| File / Folder | Purpose |
|---|---|
| `main.py` | Main program and terminal menu |
| `alarm.py` | Alarm-related logic and validation |
| `database.py` | Local text-file storage operations |
| `data/alarms.txt` | Stores saved alarms |
| `statement.md` | Project/problem statement |
| `TESTING.md` | Testing documentation |
| `requirements.txt` | Lists project dependencies |
| `.gitignore` | Specifies files/folders ignored by Git |

## Alarm Format

Alarms use the 24-hour `HH:MM` format.

Examples:

```text
07:30
12:45
18:00
23:15
```

Each alarm contains:

- Time
- Label

For example:

```text
07:30 | Morning Exercise
18:00 | Study
```

## Important Notes

- Alarm times must follow the `HH:MM` format.
- Duplicate alarms are prevented.
- Alarm information is stored locally in `data/alarms.txt`.
- The current version checks alarms only when the user selects **Check Alarms**.
- It does **not** continuously run in the background.
- It does **not** send operating-system notifications.

## Requirements

This project is designed to use standard Python functionality and local text-file storage.

If `requirements.txt` contains no external packages, no additional installation is required.

## Example Workflow

```text
1. Add Alarm
2. View Alarms
3. Delete Alarm
4. Check Alarms
5. Exit
```

A typical workflow is:

1. Add an alarm with a valid time and label.
2. View the saved alarms.
3. Check alarms against the current time.
4. Delete an alarm when it is no longer required.

## Future Improvements

Possible improvements include:

- Continuous background alarm checking
- Desktop/system notifications
- Sound alerts
- Recurring alarms
- Snooze functionality
- Editing existing alarms
- A graphical user interface

## Author

Python Alarm System — Academic Python Project
