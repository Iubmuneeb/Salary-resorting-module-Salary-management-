Muneeb iqbal
BSEE1E02041

class Employee:
    def __init__(self, emp_id, name, salary):
        self.emp_id = emp_id
        self.name = name
        self.salary = salary

class SalaryManagement:
    def __init__(self):
        self.employees = []

    def add_employee(self, emp):
        self.employees.append(emp)

    def generate_salary_report(self):
        print("Salary Report:")
        print("Employee ID\tName\t\tSalary")
        print("----------------------------------")
        for emp in self.employees:
            print(f"{emp.emp_id}\t\t{emp.name}\t\t{emp.salary}")
        print("----------------------------------")

# Create an instance of SalaryManagement
salary_management = SalaryManagement()

# Example Usage:
employee1 = Employee(1, "Muneeb Iqbal", 50000)
employee2 = Employee(2, "Jane Smith", 60000)  # Updated name to Jane Smith
