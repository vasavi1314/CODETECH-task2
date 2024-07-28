# CODETECH-Task2
<h1><b>Intern</b></h1><br>
<b>Name:</b>V.vasavi Gayathri<br>
<b>College:</b>NRI Institute of Technology<br>
<b>Roll No:</b>22KP1A44E5<br>
<B>Company:</B>CODETECH IT SOLUTIONS<br>
<B>ID:</B>CT4PP3667<br>
<B>Domain:</B>PYTHON PROGRAMMING<br>
<B>Duration:</B>July to August 2024<br>
<B>Mentor:</B>Srvavani Gouni<br>
<h1>Project Overview</h1><br>
<h2>Sample code:</h2>
def calculate_letter_grade(average):
    if average >= 90:
        return 'A', 4.0
    elif average >= 80:
        return 'B', 3.0
    elif average >= 70:
        return 'C', 2.0
    elif average >= 60:
        return 'D', 1.0
    else:
        return 'F', 0.0
def get_grades():
    grades = []
    while True:
        try:
            grade = float(input("Enter a grade (or type 'done' to finish): "))
            if 0 <= grade <= 100:
                grades.append(grade)
            else:
                print("Please enter a grade between 0 and 100.")
        except ValueError:
            break
    return grades

def calculate_average(grades):
    if grades:
        return sum(grades) / len(grades)
    else:
        return 0

def main():
    print("Student Grade Tracker")
    print("---------------------")

    grades = get_grades()
    if not grades:
        print("No grades entered.")
        return

    average = calculate_average(grades)
    letter_grade, gpa = calculate_letter_grade(average)

    print("\nGrade Summary")
    print("-------------")
    print(f"Grades Entered: {grades}")
    print(f"Average Grade: {average:.2f}")
    print(f"Letter Grade: {letter_grade}")
    print(f"GPA: {gpa:.2f}")

if __name__ == "__main__":
    main()

<h1>Output</h1><br>

![image](https://github.com/user-attachments/assets/3ffe4d15-0df4-4bd5-b1c8-1cccd677dbcf)

<h1><b>Objective:</b></h1><br>
The objective of developing a Python program to track and manage student grades is to provide a simple yet effective tool for students and educators to:

Input and Store Grades: Allow users to input grades for different subjects or assignments.
Calculate Average Grade: Compute the average grade across all subjects or assignments.
Determine Overall Grade: Display the overall grade, including letter grade and GPA.
Provide Insights: Offer additional information such as letter grades and GPA to help students understand their academic performance.
<h1>Explanation:</b></h1>


StudentGrades Class:

__init__: Initializes an empty dictionary to store grades.<br>
add_grade: Adds a grade for a specific subject.<br>
calculate_average: Computes the average of the grades.<br>
determine_letter_grade: Determines the letter grade based on the average.<br>
determine_gpa: Determines the GPA based on the letter grade.<br>
display_overall_grade: Displays the average grade, letter grade, and GPA.<br>
display_grades: Displays all the grades entered.<br>
<b><h1>main Function:<b><h1>
Provides a menu-driven interface for users to add grades, display grades, and display overall grades.<br>
Users can add grades for different subjects, view all entered grades, or calculate and display the overall grade with corresponding letter grade and GPA.<br>
This program allows users to efficiently manage and track student grades, providing clear insights into academic performance.<br>
<h1><b>Conclusion</b></h1>
Developing a Python program to track and manage student grades offers a practical solution for students and educators seeking to streamline the process of grade management. The program provides a user-friendly interface for inputting grades, calculating averages, and determining overall performance through letter grades and GPA. This tool not only ensures accuracy and consistency in grade calculations but also enhances transparency and provides valuable insights into academic achievements.






