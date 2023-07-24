# 0x15-api

This directory contains a Python script that interacts with a REST API to retrieve and display information about an employee's TODO list progress.

## Getting Started

To use the script, you need Python and the `requests` module installed on your system.

### Prerequisites

- Python 3.x
- `requests` module (install using `pip install requests`)

### Usage

Run the Python script with the employee ID as a parameter to retrieve the TODO list progress for the specified employee.

Example:

```bash
python3 0-gather_data_from_an_API.py 2
The script will then display the employee's TODO list progress in the specified format.
Files

    0-gather_data_from_an_API.py: Python script that interacts with the REST API to retrieve and display employee TODO list progress.

API Endpoint

The Python script uses the following REST API endpoint to gather the required data:

arduino

https://jsonplaceholder.typicode.com/todos?userId=<employee_id>
Replace <employee_id> with the integer value of the employee you want to retrieve the TODO list progress for.
Format of Output

The script will display the employee TODO list progress in the following format:

csharp

Employee EMPLOYEE_NAME is done with tasks(NUMBER_OF_DONE_TASKS/TOTAL_NUMBER_OF_TASKS):
    TASK_TITLE
    TASK_TITLE
    ...

Where:

    EMPLOYEE_NAME: Name of the employee
    NUMBER_OF_DONE_TASKS: Number of completed tasks
    TOTAL_NUMBER_OF_TASKS: Total number of tasks (completed + non-completed)
    TASK_TITLE: Title of each completed task
