## Week 8 Final Exam

### Part A Vaccination Tracker

We are in the middle of a global pandemic. The dean of a university has asked you to write a program (using the C programming language) to track how many of the students and staff are vaccinated and with which vaccine. A person’s record includes their name, date of birth, student or staff ID, a list of any underlying health conditions, the vaccine vendors and the dates for each vaccine. Two examples of formatted records could look like this:

1.
+ Name: John Smith
+ Vaccine vendor: Pfizer
+ Vaccination date: 02/08/2021
+ Date of birth: 06/01/1990
+ Underlying condition: None
+ Student/Staff ID: 556679

2.
+ Name: Mary Jones
+ Vaccine vendor: None
+ Vaccination date: None
+ Date of birth: 09/10/1988
+ Underlying condition: Asthma
+ Student/Staff ID: 556677

Students can assume that privacy law does not apply in this case.

Making use of techniques covered in the course material: functions, file handling, dynamic memory allocation, data structures and sorting algorithms, produce a system with the following functions (named exactly as provided below).

Function 1: load_data 

This function is automatically called when the program is started. It loads a list of records from a file called “records.txt” (the user is not required to input the file name).  If the file does not exist, notify the user, create a new file and display the main menu. Once the file is open, data is read into an array of structs by dynamically creating sufficient memory for each entry read from the file.

Function 2: display_menu

After the application has started, use this function to print a series of options to the user using a numbered list (see below). When the user selects an option, the system performs the required action, and then returns to the menu, waiting for the user to select another option. Include an option to exit the system.

Your main menu system might resemble the following:
1.	Add a new person
2.	View vaccination status for all students and staff
3.	Modify existing record
4.	Sort vaccinated people by name
5.	Sort unvaccinated people by name
6.	Sort vaccinated people by date
7.	Display percentage of unvaccinated people 
8.	Display a list of people with an underlying condition older than 65 
9.	Exit

Function 3: add_new_record

When the user selects the “1. Add a new person” menu item, prompt them for the data for the new record. Append the new record to the array of current records and notify the user that the new record has been added successfully. 

Function 4: view_all_records

When the user selects the “2. View vaccination status for all students and staff” option, this function prints a list of all employees and their information on record. Make sure that the information is formatted neatly with headers and appropriate tabs or spacing, not simply a list of raw information. 

Function 5: modify_record

When the user selects the “3. Modify existing record” option, they are prompted for an ID. This function then finds the relevant record and prompts the user for the updated details, which should replace the existing record details.

Function 6: sort_vaccinated_by_name

When the user selects the “4. Sort vaccinated people by name” option, this function prints a list of the names of people who have been vaccinated with two doses. This list should be sorted by the last name.

Function 7: sort_unvaccinated_by_name

When the user selects the “5. Sort unvaccinated people by name” option, this function prints a list of the names of people who have not had any doses of vaccine. This list should be sorted by the last name.

Function 8: sort_vaccinated_by_date

When the user selects the “6. Sort vaccinated people by date” option, this function prints a list of the names of people who have been vaccinated. This list should include the date of the most recent vaccine dose presented in the following format “yyyy/mm/dd” and be ordered from most recent to least recent.

Function 9: display_percent_unvaccinated

When the user selects the “7. Display percentage of unvaccinated people” option, this function shows the percentage of unvaccinated people formatted to 2 decimal places, along with an appropriate message.

Function 10: display_seniors_with_condition

When the user selects the “8. Display a list of people with an underlying condition older than 65” option, this function prints a list of the names of people over the age of 65 with any underlying health condition. This list should include the date of birth of the person, their underlying condition and be ordered from oldest to youngest.

Function 11: save_data

This function is called when the user chooses to exit the system. Open the data file and write out the information currently contained in the array. 


Part B - Modification 								

Improve your program by allowing for storage of up to two vaccination vendors and dates to represent the standard two doses that each adult would be expected to receive. Dates should be stored as integer values representing the number of days that have passed since the 1st of January 2000. E.g. 03/12/21 would be 8007 days since 01/01/00. Your modified program should accept the date as a string in the format “dd/mm/yy” and parse the string to create an int representing the number of days. When the stored dates are required to be displayed on screen they should be converted back to a format that allows them to be displayed as “dd/mm/yy”.

Now that booster doses of vaccines are being administered, further modify the system to include details of the booster vendor and booster date in the records.

Add new menu items to the main menu to allow the user to access these new record details. 

Note: Produce a separate code file to Part A. It should contain all the functionality of Part A, but with appropriate changes relating to the vaccine and booster details. 


