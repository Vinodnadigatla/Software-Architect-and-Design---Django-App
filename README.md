# Hello World Django App

This is a simple Django web application that returns a JSON object with the message **"Hello World!"**.

## Getting Started

Follow the steps below to set up and run the application locally.

### Prerequisites

- Ensure you have Python installed.
- Install Django if it's not already installed:

   ```bash
   pip install django
   ```

### Installation

1. **Clone the repository** to your local machine:

   ```bash
   git clone <repository_url>
   ```

2. **Navigate** to the project directory:

   ```bash
   cd helloworld_project
   ```

### Running the Application

3. **Start the Django development server**:

   ```bash
   python manage.py runserver
   ```

4. **Access the application** in your browser:

   Open `http://127.0.0.1:8000/` to get the "Hello World" JSON response.

---

## Optional: Render "Hello World" in HTML

To display the "Hello World" message as an HTML page, follow these additional steps:

1. **Create an HTML template** named `hello_world.html` inside `helloworld_app/templates/`.

2. **Modify the view** in `helloworld_app/views.py` to render the template:

   ```python
   from django.shortcuts import render

   def hello_world(request):
       return render(request, 'hello_world.html')
   ```

3. **Restart the server** if needed and visit `http://127.0.0.1:8000/hello` to see the HTML version of the message.

---

## Project Structure

- `helloworld_project/`: Django project folder.
- `helloworld_app/`: Django app folder containing views and templates.
- `README.md`: Documentation.
