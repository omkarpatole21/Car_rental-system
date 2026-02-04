# Car Rental Management System

A professional Django-based car rental management system featuring a sleek Glassmorphism UI. This application handles car registration, customer management, rentals, and returns using an in-memory data store.

## Features
- **Glassmorphism Design**: Modern UI with backdrop filters and semi-transparent elements.
- **In-Memory Logic**: Uses the provided custom Python classes to manage data in RAM.
- **Full CRUD-like Flow**:
    - Add/View Vehicles
    - Register Customers
    - Process Rental Transactions
    - Manage Returns
- **Responsive Layout**: Built with Bootstrap 5 and Font Awesome.

## Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

## Installation

1. Clone or download the project files.
2. Navigate to the project root directory.
3. Install the required dependencies:
    pip install -r requirements.txt

## Running the Application

1. Ensure you are in the directory containing `manage.py`.
2. Run the development server:
    python manage.py runserver

3. Open your browser and navigate to:
    http://127.0.0.1:8000/


## Project Structure
- `rental/logic.py`: Contains the core `Person`, `Car`, `Customer`, and `CarRentalSystem` classes.
- `rental/static/css/style.css`: The custom stylesheet for the Glassmorphism effect.
- `rental/views.py`: Bridges the logic instance with the Django templates.
- `car_rental_project/settings.py`: Configured to serve static files correctly in development.

## Note on Data Persistence
Because this application uses a global object in `logic.py` to store data:
- **Data is NOT saved to a database**.
- If you restart the server (`Ctrl+C` and run again), all added cars and customers will be cleared.
- Some sample data is pre-populated in `logic.py` for immediate testing.
