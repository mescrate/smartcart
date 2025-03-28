# Smartcart

## Prerequisites

Before you start, make sure you have the following installed on your system:

- Python 3.x
- pip (Python package installer)
- virtualenv (to create isolated Python environments)

### Steps to Set Up Your Project

### 1. **Install Python**

If Python is not installed on your machine, follow these steps:

- **Ubuntu/Debian:**
  ```bash
  sudo apt update
  sudo apt install python3 python3-pip python3-venv
  ```

- **Windows/macOS:**
  Download Python from the [official Python website](https://www.python.org/downloads/) and follow the installation instructions.

### 2. **Install pip (Python Package Installer)**

`pip` is the package manager for Python. If you installed Python 3.4+ from the official website, pip is installed by default. If you need to install it manually:

- **For Ubuntu/Debian:**
  ```bash
  sudo apt install python3-pip
  ```

- **For Windows/macOS:**
  Pip should already be included with Python. If not, you can follow the [pip installation guide](https://pip.pypa.io/en/stable/installation/).

### 3. **Create a Virtual Environment**

A virtual environment is an isolated Python environment that allows you to install dependencies without interfering with system-wide packages.

In your project directory, run the following command to create a virtual environment:

```bash
python3 -m venv env
```

### 4. **Activate the Virtual Environment**

To activate the virtual environment:

- **For Linux/macOS:**
  ```bash
  source env/bin/activate
  ```

- **For Windows:**
  ```bash
  .\env\Scripts\activate
  ```

You should see `(env)` in your terminal, indicating that the virtual environment is active.

### 5. **Install Project Requirements**

Ensure that your virtual environment is active, then install all required dependencies from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

This command will install all the packages listed in your `requirements.txt`.

### 6. **Run Migrations**

Django uses migrations to apply changes to the database schema. Run the following command to apply any pending migrations:

```bash
python manage.py migrate
python manage.py makemigrations
```

### 7. **Run the Development Server**

After applying migrations, you can start the development server using:

```bash
python manage.py runserver
```

This will start the Django development server. By default, it runs on `http://127.0.0.1:8000/`.

### 8. **Access the Application**

Once the server is running, open a web browser and visit the following URL to see the project in action:

```
http://127.0.0.1:8000/
```
