# Employee Wellbeing Monitoring

This Python project tracks and visualizes the wellbeing status of employees over time. It defines a structured framework for managing employee data, applying wellbeing protocols, and visualizing wellbeing history using a heatmap.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Example Output](#example-output)

## Overview

The purpose of this project is to monitor the wellbeing status of employees, update their status based on predefined protocols, and visualize their wellbeing trends over time. It makes use of Python's `pandas`, `seaborn`, and `matplotlib` libraries for data handling and visualization.

## Features

- **Employee Class**: Stores individual employee details and their wellbeing history.
- **Wellbeing Protocol Class**: Defines wellbeing protocols that can be applied to employees.
- **Management Class**: Manages a list of employees and applies wellbeing protocols.
- **Data Visualization**: Visualizes wellbeing status over time in a heatmap.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/employee-wellbeing-monitoring.git
   ```
2. Navigate into the project directory:
   ```bash
   cd employee-wellbeing-monitoring
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the script to initialize a sample set of employees, generate random wellbeing statuses, and display a heatmap:

```bash
python wellbeing_monitoring.py
```

### Explanation

1. **Employee Class**: Stores basic employee details and a history of their wellbeing.
2. **WellbeingProtocol** and **SpecificWellbeingProtocol**: Define a structure for applying custom protocols to employees.
3. **Management Class**: Manages employees and applies wellbeing protocols to each.
4. **Data Visualization**: Creates a heatmap showing the wellbeing status of each employee over time.

### Sample Code Snippet
```python
employee_names = ["Alice", "Bob", "Charlie", "David", "Emma"]
management = Management()
for i, name in enumerate(employee_names, start=1):
    employee = Employee(name, i, "Good")
    management.add_employee(employee)
```

## Dependencies

- `pandas`
- `seaborn`
- `matplotlib`

You can install all dependencies with:
```bash
pip install pandas seaborn matplotlib
```

## Example Output

The script generates a heatmap that visualizes the wellbeing status of each employee across a series of days:

![Employee Wellbeing Heatmap](https://github.com/user-attachments/assets/3ecfbd4d-fdc4-4e28-b652-ebb6ab37311e)
