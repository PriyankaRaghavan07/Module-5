
# Exp.No:5d  
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

```python
class Person:
    def getname(self,name):
        self.name=name
class Age(Person):
    def getage(self,age):
        self.age=age
class Location(Age):
    def getlocation(self,l):
        self.l=l
    def display(self):
        print(f"{self.name} {self.age} {self.l}")
n=input()
a=int(input())
l=input()
g=Location()
g.getname(n)
g.getage(a)
g.getlocation(l)
g.display()
```

### OUTPUT
<img width="1182" height="242" alt="image" src="https://github.com/user-attachments/assets/011e30c6-c664-4fdc-980e-f3e47c696ab3" />

### RESULT
Therefore, the output is the example to write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.
