# SECTION A 

# Student Grade Management System

This is a Python program that allows a user to enter students' names and grades. It calculates the total of all the grades and the average grade for the class. It also checks that the grades entered are valid before accepting them.

At the beginning of the programme, the user will be asked to enter the number of students which needs to be recorded. The number entered will determine how many times the programme will ask for the student's name and grade. 

Two empty lists that store the names and grades will be created by the program before collecting the student's information.  It also sets the total to zero so that it can add each student's grade as the program runs.

The program then uses a `for` loop to collect each student's name and grade. The student's grade is converted into a number so that it can be used in calculations.

To make sure that the grades entered are correct, the program uses a `while` loop to check whether a grade is below zero or above 100. If an invalid grade is entered, the program displays an error message and asks the user to enter the grade again. This continues until a valid grade is provided.

Once a valid grade has been entered, it is added to the class total. The student's name and grade are also stored in their respective lists so that they can be displayed later.

After collecting all the students' information, the program checks whether the number of students entered is greater than zero. If there are students, it calculates the class average by dividing the total of all the grades by the number of students.

The program then displays the class total and average. It uses another `for` loop to display each student's name and grade, together with the overall class average.

If the user enters zero as the number of students, the program displays a message saying that no students were entered instead of attempting to calculate an average.

The program uses variables to store information, lists to keep track of students' names and grades, and loops to repeat certain tasks. It also uses `if` statements to make decisions, input validation to prevent invalid grades from being accepted, and basic mathematical operations to calculate the class total and average.

This program provides a simple way to record students' grades and calculate the overall class average. It brings together basic Python concepts to show how a program can collect information, check the data entered, perform calculations, and display results to the user.

#SECTION B 

This program is designed to record students' names and their grades in Biology, English, and Chemistry. It calculates each student's average grade, identifies the highest and lowest grades in each subject, and displays the results in a summary table

The program begins by storing the three subjects in a list called subjects. It then asks the user how many students they want to enter and stores the number in number_of_students. An empty list called students is created to keep track of all the students and their grades.

The program uses a for loop to collect information for each student. It asks for the student's name and creates another empty list, student_grades, to store their marks. It then goes through each subject and asks the user to enter the corresponding grade.

To make sure the grades are valid, a while loop checks that each grade falls between 0 and 100. If the user enters a grade outside this range, the program displays an error message and asks them to try again. Once a valid grade is entered, it is added to the student_grades list using append().

After collecting the three grades, the program stores the student's name and grades together in the students list. This process repeats until all the students have been entered.

Once the information has been collected, the program checks whether any students were entered. If there are students, it calculates each student's average by adding their grades using sum() and dividing the result by the number of grades using len(). The round() function is used to display the average to two decimal places.

The program also compares students' performance in each subject. It collects the grades for one subject at a time and uses max() to find the highest grade and min() to find the lowest. This process repeats for Biology, English, and Chemistry.

Finally, the program displays a summary table showing each student's name, their grades in all three subjects, and their average. The table uses f-strings to keep the information neatly arranged in columns. If the user enters zero as the number of students, the program displays a message stating that no students were entered.

The subjects list stores the names of the three subjects, while number_of_students keeps track of how many students the user wants to enter. The students list stores the information collected for all students, and name holds the name of the student currently being entered or processed.

The student_grades list stores the grades entered for one student, while grade holds each individual grade as it is entered. The variable i controls how many times the student information loop repeats.

When the program processes the collected information, grades refers to a student's stored grades, and average_grade holds the average calculated from those grades. The variable position helps the program identify which subject it is processing, while subjects_grades temporarily stores all students' grades for that subject so that the highest and lowest can be found.

#SECTION C

This program manages students' grades in Biology, English, and Chemistry. It allows the user to enter student details, keep track of their grades, and perform different operations on the records through a menu.

At the beginning, the program stores the three subjects in a tuple called subjects and asks the user how many students they want to enter. The students are stored in a dictionary, where each student's name is linked to another dictionary containing their grades for each subject. I used lists to store the grades because a student may have more than one grade for a subject.

The program uses a for loop to collect each student's name and grades. It also checks that every grade is between 0 and 100. If the user enters a mark outside this range, a while loop keeps asking for a valid grade until the correct value is entered. Once the student's information has been collected, it is added to the main dictionary.

After the initial records have been entered, the program displays a menu with six options. The user can add a student, update a grade, delete a student, view grades for a particular subject, search for a student, or exit the program. A while loop keeps the menu running until the user selects option 6, while if and elif statements determine which operation should be performed.

When adding a student, the program first checks whether the name already exists in the dictionary. If it does, the user is informed that the student is already registered. Otherwise, the program collects the student's grades and adds the new record. When updating a grade, the program checks whether the student and subject exist before accepting the new mark. The append() method adds the new grade to the existing list, meaning that the previous grade is retained.

The delete option uses the del statement to remove a student's record from the dictionary. The view option allows the user to select a subject and see the grades recorded for that subject for all students. It uses a for loop and the items() method to go through the dictionary and display the information.

The search option allows the user to find a particular student's grades. If the student exists, the program displays their grades for all three subjects and calculates their average. The sum() function adds the grades together, while len() counts the number of grades recorded. The total is divided by the count to calculate the average, and round() limits the displayed result to two decimal places. If the student cannot be found, the program displays an appropriate message.

The program also handles invalid menu selections by displaying an error message and allowing the user to try again. It continues running until the user chooses to exit.

Overall, this program applies Python concepts such as dictionaries, lists, tuples, loops, conditional statements, and built-in functions to manage student information. It also demonstrates how these concepts can be combined to create a menu-driven program that allows users to store, access, and update data.


