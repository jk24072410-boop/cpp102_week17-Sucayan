# cpp102_week17-Sucayan
Simulated Device Monitoring and Alert System
Student Name: John Kierby Sucayan Student Number: 2601304 Section: 1CpE-C

Project Description
This program monitors simulated device temperature readings. It stores the readings in a list, accepts new valid readings, and classifies each one as NORMAL, WARNING, or CRITICAL. It also prints a numerical summary and an overall monitoring status. It was written for CPP102 Week 17 using only Python 3 built-in features.

Features
View all stored temperature readings
Add a new reading (whole numbers from 0 to 100 only)
Classify every reading (below 30 is NORMAL, 30 to 35 is WARNING, above 35 is CRITICAL)
Generate a numerical summary: count, total, average, minimum, maximum, category counts and percentages, and overall status
Reject invalid menu choices and invalid readings without crashing
Requirements
Python 3 (no external packages)
How to Run
Open a terminal inside the Week17 folder.
Type: python device_monitor.py
Sample Output
MONITORING SUMMARY
------------------
Number of readings  : 6
Total of readings   : 193
Average temperature : 32.17 °C
Minimum temperature : 28 °C
Maximum temperature : 37 °C

NORMAL   : 2 (33.33%)
WARNING  : 3 (50.00%)
CRITICAL : 1 (16.67%)

Overall Status: ATTENTION REQUIRED
This output was produced after adding the valid reading 33 to the initial list.

Test Cases
I performed 13 tests (the 10 required tests plus 3 extra). 13 passed and 0 failed. Full details are in test_cases.md.

Known Limitations
Readings are not saved to a file, so all data is lost when the program closes.

Readings can only be added; editing and deleting existing readings are not supported.

The 0–100 range and the limits of 30 and 35 are intended only for this classroom simulation. They do not represent actual device-safety standards.

Reflection
In this project, I combined lists, loops, selection statements, and functions to create a complete program for the first time. Dividing the program into smaller functions, with main() controlling the menu loop, made the code easier to understand, organize, and test compared to my earlier single-purpose exercises.

The most challenging part was implementing the correct order of input validation, particularly when testing the boundary cases TC06 and TC07. By trying specific input values, I gradually understood how the validation process worked and why the order of the checks was important.

If I were to continue developing this project, I would add a file-saving feature so that readings could be stored and retrieved even after the program closes. This would make the program more practical and improve its overall functionality.


