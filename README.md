# Django-Restaurant-Application

This is a Django project that demonstrates a simple web application for booking and displaying a menu. It includes views to showcase basic usage of Django's functionality, such as rendering templates, processing forms, and interacting with models.

## Project Structure

The project consists of the following main components:

- `app_name/` directory: This is the Django app directory that contains the code for the project.
  - `views.py`: Contains the view functions responsible for rendering different pages.
  - `models.py`: Contains the data models used in the project.
  - `forms.py`: Contains the form definition used for the booking form.
  - `templates/` directory: Contains HTML templates for different pages.
  - `static/` directory: Contains static assets like CSS, JavaScript, and images.

## Functionalities

### Home Page

The home page is accessible through the URL path `/`. It renders the `index.html` template.

### About Page

The about page can be accessed through the URL path `/about/`. It renders the `about.html` template.

### Booking Form

The booking form is accessible via the URL path `/book/`. Users can submit their booking information using this form. Upon submission, the data is saved to the database using the `Booking` model.

### Menu Display

The menu page can be accessed through the URL path `/menu/`. It displays a list of menu items retrieved from the `Menu` model in the database.

### Individual Menu Item Display

Individual menu items can be viewed by clicking on their respective links on the menu page. The URL path follows the format `/menu/<item_id>/`, where `item_id` corresponds to the primary key of the menu item. This view is rendered using the `menu_item.html` template.

## Getting Started

1. Clone this repository to your local machine.
2. Install the required dependencies using the command: `pip install -r requirements.txt`.
3. Run the Django development server: `python manage.py runserver`.
4. Access the project in your web browser at `http://localhost:8000/`.
