# Python API Student Management

## Overview

This project is a Python-based student management console application created by Grupp 4: Furkan, Simon, Sahand, Shilan, Sayna, and Wadad.

The application fetches student data from an external API and provides a simple command-line interface for:
- logging in with a fixed username and password
- displaying a full class list with contact details
- searching for a student by first name

## Key features

- Retrieves user data from `https://dummyjson.com/users`
- Stores results in student objects
- Prints contact details and formatted address information
- Offers a menu with options for class list display, student search, and logout
- Handles API connection errors and JSON parsing failures gracefully

## Files

- `Main Program` - Main Python script containing all application logic

## Requirements

- Python 3.8 or newer
- `requests` library

Install dependencies with:

```bash
pip install requests
```

## Usage

Run the main program from the `python-api-student-management` folder:

```bash
python "Main Program"
```

When prompted, log in with the following credentials:

- Username: `Devops24`
- Password: `Grupp4`

After login, choose from the menu:

1. Klasslista - show the full list of students
2. Sök elev - search for a student by first name
3. Logga ut - exit the application

## Notes

- The application uses fixed login credentials and a public dummy user API.
- Student search matches only the first name and is case-insensitive.
- If the API request fails, the program will display an error and exit without showing the menu.
