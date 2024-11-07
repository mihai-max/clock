# Simple Web Clock with Alerts

This is a web-based clock that displays the current time in Berlin time and updates in real-time. It also displays the date in the `DD/MM/YYYY` format. The clock changes color under specific conditions:
- **Red**: During certain times on weekdays (Monday-Friday).
- **Green**: At 13:10 on Fridays before a Bavarian school vacation.

## Features

- Displays the current time with hours, minutes, and seconds.
- Shows the date in `DD/MM/YYYY` format.
- Alerts:
  - Turns **red**:
    - Monday-Friday: 9:30 - 9:50 and 11:20 - 11:40.
    - Tuesday and Wednesday: 12:25 - 13:10.
  - Turns **green**:
    - On Fridays at 13:10, if it's the last day before a Bavarian school vacation.
- Timezone set to Berlin (Europe/Berlin).

## Prerequisites

To run this project, you need:
- A web browser (no other dependencies are required).

## Usage

1. Clone or download the repository.
2. Open the `index.html` file in a web browser.
3. The clock will automatically start displaying the current Berlin time and date.

## Code Overview

The project uses simple HTML, CSS, and JavaScript:
- **HTML**: Structures the clock and date display.
- **CSS**: Styles the clock and date with dynamic colors for alerts.
- **JavaScript**: 
  - Fetches the current time and date in Berlin timezone.
  - Checks conditions to change color for specific alert times and dates.
  - Includes a function to identify Bavarian school vacation dates and determine the last school day before each vacation period.

## Customization

- **Alert Times**: You can modify the JavaScript code to change the alert times by editing the `isRedAlert` and `isGreenAlert` conditions.
- **Vacation Dates**: Modify the `bavarianVacations` array in JavaScript to update the vacation periods.

