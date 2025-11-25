# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM
212223060181

NANCY
```
class person:
    def __init__(self):
        self.name=""
    def get_name(self):
        self.name=input()
class age(person):
    def __init__(self):
        super().__init__()
        self.age=0
    def get_age(self):
        self.age=int(input())
class city(age):
    def __init__(self):
        super().__init__()
        self.city=""
    def get_city(self):
        self.city=input()
    def display(self):
        print(self.name, self.age, self.city)

obj=city()
obj.get_name()
obj.get_age()
obj.get_city()
obj.display()


```

### OUTPUT
<img width="830" height="265" alt="image" src="https://github.com/user-attachments/assets/33e752fa-a7c1-44b5-83cc-5cd692a43021" />

### RESULT
Thus,a Python program to get the name, age, and location of a person and display them using multilevel inheritance are verified.
