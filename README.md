# Payroll System

This is a Django-based payroll system designed to manage employee records and payroll processing.

## Features

- Employee Management: Add, update, delete, and view employee details.
- Payroll Management: Create, update, delete, and view payroll records.
- Detailed Reporting: Generate detailed reports for payroll and employee information.

## Models

The system includes the following models:

- **Empleado**: Represents an employee with fields for identification, name, salary, department, and position.
- **Nomina**: Represents a payroll record with fields for the period, total income, total deductions, and net pay.
- **NominaDetalle**: Represents detailed payroll information for each employee within a payroll record, including salary, bonuses, deductions, and net pay.

## Setup Instructions

1. **Clone the Repository**:
   ```
   git clone <repository-url>
   cd payroll_system
   ```

2. **Create a Virtual Environment**:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**:
   ```
   pip install -r requirements.txt
   ```

4. **Apply Migrations**:
   ```
   python manage.py migrate
   ```

5. **Run the Development Server**:
   ```
   python manage.py runserver
   ```

6. **Access the Application**:
   Open your web browser and go to `http://127.0.0.1:8000/`.

## Testing

To run the tests for the payroll app, use the following command:
```
python manage.py test payroll
```

## License

This project is licensed under the MIT License. See the LICENSE file for more details.