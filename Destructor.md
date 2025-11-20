
# Exp.No:5b  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```python
class Employee:
    def __init__ (self):
        print ( 'Employee created.' )
    def __del__(self):
        print("Destructor called, Employee deleted.")
obj = Employee ()
```

### OUTPUT
<img width="1184" height="216" alt="image" src="https://github.com/user-attachments/assets/a93dec65-a6d7-43d2-8ed1-dea7050808ec" />

### RESULT
Therefore, the output is the example to create a Python class `Student` with a destructor.
