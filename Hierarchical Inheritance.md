# Exp.No:5c  
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
```python
class Details:
    def get_details(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

class Employee(Details):
    def get_employee_details(self, company, department):
        self.company = company
        self.department = department

    def display(self):
        print("Employee Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Company: ", self.company)
        print("Department: ", self.department)

class Doctor(Details):
    def get_doctor_details(self, hospital, department):
        self.hospital = hospital
        self.department = department

    def display(self):
        print("\nDoctor Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

emp_id = int(input())
emp_name = input()
emp_gender = input()
emp_company = input()
emp_dept = input()

doc_id = int(input())
doc_name = input()
doc_gender = input()
doc_hospital = input()
doc_dept = input()

emp = Employee()
doc = Doctor()

emp.get_details(emp_id, emp_name, emp_gender)
emp.get_employee_details(emp_company, emp_dept)
doc.get_details(doc_id, doc_name, doc_gender)
doc.get_doctor_details(doc_hospital, doc_dept)
emp.display()
doc.display()
```

### OUTPUT  
<img width="1183" height="486" alt="image" src="https://github.com/user-attachments/assets/528e3adf-f0fe-4a05-8683-457a82837203" />

### RESULT
Therefore, the output is the example to write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.
