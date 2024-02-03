# learn_Django

# Setting Up a Django Project in Virtual Environment using virtualenv

This guide will walk you through the process of creating and setting up a Django project in a virtual environment using `virtualenv`.

## Prerequisites

- Python installed on your system
- `pip` package manager

# Step 1: Install virtualenv

If you haven't installed `virtualenv` yet, you can do so using the following command:

```bash
pip install virtualenv
```

# Step 2: Create a Virtual Environment

Navigate to the directory where you want to create your Django project and run the following commands to create a virtual environment. Replace `myenv` with your preferred virtual environment name.

## On Windows
```python
python -m venv myenv
```


## On macOS/Linux
```python
python3 -m venv myenv
```
This step creates a virtual environment named myenv in your chosen directory.

# Step 3: Activate the Virtual Environment

Activate the virtual environment to start using it:

## On Windows
```bash
myenv\Scripts\activate
```

## On macOS/Linux
```bash
source myenv/bin/activate
```

# Step 4: Install Django

Once the virtual environment is active, you can install Django using `pip`. Run the following command:

```bash
pip install django
```

This installs the latest version of Django within your virtual environment.

## Step 5: Create a Django Project

Now that Django is installed, create a new Django project using the following command:

```bash
django-admin startproject myproject
```

Replace `myproject` with your preferred project name.

## Step 6: Navigate to the Project Directory

Move into the project directory:

```bash
cd myproject
```

This step ensures that you are inside the project directory before proceeding with further setup.

## Step 7: Run Migrations

Run the initial migrations to set up the database:

```bash
python manage.py migrate
```

This applies the initial database schema to your project.

## Step 8: Create a Superuser (Optional)

If you want to create an admin superuser, use the following command and follow the prompts:

```bash
python manage.py createsuperuser
```

This step allows you to create an administrative user for your Django project.

## Step 9: Run the Development Server

Start the development server:

```bash
python manage.py runserver
```

This command runs the development server, and you can view your Django project by opening [http://localhost:8000/](http://localhost:8000/) in your web browser.

And to access the admin panel [http://localhost:8000/admin](http://localhost:8000/admin)

## Conclusion

You've successfully set up a Django project in a virtual environment! Remember to activate your virtual environment every time you work on your project and deactivate it when you're done.

To deactivate the virtual environment, simply run:

```bash
deactivate
```

Happy coding!

