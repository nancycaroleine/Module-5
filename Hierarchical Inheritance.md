# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
212223060181

NANCY
```
class Details:
    def __init__(self):
        self.id=0
        self.name=''
        self.gender=''
    def get_details(self):
        self.id=int(input())
        self.name=input()
        self.gender=input()
        
class employee(Details): #Inheritance
    def __init__(self):
        super().__init__()
        self.com=''
        self.dept=''
    def get_emp(self):
        self.get_details()
        self.com=input()
        self.dept=input()
    def display_employee(self):
        print("Employee Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Company: ", self.com)
        print("Department: ", self.dept)

class doc(Details): #Inheritance
    def __init__(self):
        super().__init__()
        self.hospital=''
        self.department=''
    def get_doc(self):
        self.get_details()
        self.hospital=input()
        self.department=input()
    def display(self):
        print("\nDoctor Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)


emp=employee()
emp.get_emp()
emp.display_employee()
d=doc()
d.get_doc()
d.display()


```

### OUTPUT  

<img width="1093" height="553" alt="image" src="https://github.com/user-attachments/assets/9b86da0e-f98f-4684-98eb-d2bae34ddfb8" />
 
### RESULT
Thus , a Python program to get the employee and doctor details and display them using hierarchical inheritance are verified.
