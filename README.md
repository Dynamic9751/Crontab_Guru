# Vohala_Crontab_Guru


Vohala Crontab Guru is a simple web-based tool designed to help users create, visualize, and understand crontab expressions. It provides a user-friendly interface to input crontab fields and returns a human-readable description of the crontab schedule, along with the next execution time.
Features

    Crontab Field Input: Allows users to input values for the five key crontab fields (minute, hour, day of the month, month, day of the week).
    Crontab Description: Generates a human-readable description of the cron job schedule based on the input.
    Next Execution Time: Calculates and displays the next time the cron job will be executed.
    Real-Time Validation: Checks the validity of the crontab field inputs and displays an error message if any value is out of range.
    Crontab Expression: Displays the generated crontab expression based on user input.

Crontab Fields

    Minute: 0-59 or * (every minute).
    Hour: 0-23 or * (every hour).
    Day of Month: 1-31 or * (every day of the month).
    Month: 1-12 or * (every month).
    Day of Week: 0-7 (Sunday is both 0 and 7) or * (every day of the week).

Special Characters

The tool supports standard and non-standard special characters used in crontab expressions:

    * : any value (e.g., every minute or every hour).
    , : separates multiple values (e.g., 1,2,3).
    - : specifies a range of values (e.g., 1-5).
    / : specifies step values (e.g., */5 for every 5 minutes).
    Non-standard shortcuts:
        @yearly : Run once a year.
        @annually : Same as @yearly.
        @monthly : Run once a month.
        @weekly : Run once a week.
        @daily : Run once a day.
        @hourly : Run once an hour.
        @reboot : Run at system startup.

Usage

    Clone or download the repository.
    Open the index.html file in any modern web browser.
    Input the values for minute, hour, day of the month, month, and day of the week.
    The tool will automatically display:
        The crontab description.
        The next execution time.
        The crontab expression.

Example

For example, entering:

    Minute: 0
    Hour: 12
    Day of Month: 1
    Month: 1
    Day of Week: *

Will generate the following description and output:

    Description: "At 0 minute(s) past 12 hour(s), on 1 day(s) of the month, in 1 month(s), on every day(s) of the week."
    Next Execution Time: (Calculated based on the current date and time).
    Crontab Expression: 0 12 1 1 *

Code Explanation

    HTML: The structure includes input fields for crontab fields (minute, hour, day of the month, month, and day of the week).
    CSS: Provides a modern and clean design for the form and output sections.
    JavaScript: The logic handles validation of crontab fields, generation of the human-readable description, calculation of the next execution time, and construction of the crontab expression.

Key Functions

    describeCron(): Generates a human-readable description of the crontab expression.
    getNextExecutionTime(): Calculates the next execution time based on the current date and the provided crontab fields.
    isValidCrontabField(): Ensures that the input values are valid for each crontab field.

Contributing

Feel free to fork this repository, make improvements, and submit pull requests.
