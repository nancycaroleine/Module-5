# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

---

### ALGORITHM

1. Define the `Student` class.
2. Inside the `Student` class, define the `__init__` method (constructor). The `__init__` method accepts two parameters: `name` and `student_id`.
    - Inside the `__init__` method: Assign the value of `name` to `self.name` and `student_id` to `self.student_id`.
3. Define the `get_student_info` method inside the `Student` class:
    - This method should return a string formatted with `self.name` and `self.student_id`.
4. Define the `Attendance` class, which inherits from the `Student` class.
5. Inside the `Attendance` class, define the `__init__` method (constructor).
    - The `__init__` method accepts three parameters: `name`, `student_id`, and `attendance`.
    - Inside the `__init__` method: Call the parent class constructor `super().__init__(name, student_id)` to initialize `name` and `student_id`. Assign the value of `attendance` to `self.attendance`.
6. Define the `check_eligibility` method inside the `Attendance` class:
    - If `self.attendance` is greater than 80, return a formatted string indicating the student is eligible for the module exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the module exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM
212223060181

NANCY
```
class stu:
    def __init__(self, name):
        self.name=name
class att:
    def __init__(self, id):
        self.id=id
class placement(stu, att):
    def __init__(self, name, id, grade):
        stu.__init__(self, name)
        att.__init__(self, id)
        self.grade=grade
        
    def display(self):
        print(self.name)
        print(self.id)
        if self.grade > 90:
            print("Eligible for Placement")
        else:
            print("Not Eligible for Placement")
name=input()
id=int(input())
grade=int(input())
obj=placement(name, id, grade)
obj.display()

```

### OUTPUT
<img width="875" height="364" alt="image" src="https://github.com/user-attachments/assets/a3fdf249-0b5d-4e47-8480-3e1377012ab1" />


### RESULT
Thus, program displays the student’s details and indicates whether they are eligible for placement based on attendance is verified successfully.
