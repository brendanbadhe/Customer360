# Customer360

Customer360 is a Django-based web application for managing customer communication records in a centralized location. It allows organizations to consolidate customer interactions across multiple channels, providing a professional customer management experience.

## Features

- Capture customer communication records (Channel, Direction, Summary)
- Add and manage customer details
- Record interactions for each customer
- View interactions from the last 30 days
- Professional, responsive UI with Bootstrap and custom CSS
- Extensible: add new fields (e.g., social media) and channels

## Setup Instructions

1. **Install Python and Django**

   - Ensure Python 3.11+ is installed.
   - Install Django:

     ```
     python -m pip install Django
     ```

2. **Run Migrations**

   ```
   python manage.py makemigrations customer360
   python manage.py migrate
   ```

3. **Start the Development Server**

   ```
   python manage.py runserver
   ```

4. **Access the Application**
   - Open your browser and go to `http://127.0.0.1:8000/`

## Usage

- **Add a Customer:** Click "New Customer" and fill out the form.
- **List Customers:** View all customers on the home page.
- **Record Interaction:** Select a customer and click "Interact" to log a communication.
- **View Summary:** Click "Summary" to see interactions from the last 30 days.

## Customization

- To add new fields (e.g., `social_media`) to the customer model, update `models.py`, templates, and views accordingly.
- To add new interaction channels, update the `CHANNEL_CHOICES` in the `Interaction` model.
