
# Project Automator

## Overview

The Project Automator is a Python script designed to automate the creation and initial configuration of Laravel and Django projects. This script helps developers quickly set up their development environment, allowing them to focus more on coding and less on the repetitive setup tasks.

## Features

- **Laravel Project Setup**: Creates a new Laravel project with an optional Jetstream setup using Inertia.js.
- **Django Project Setup**: Creates a new Django project along with an initial application, and configures URLs and models.
- **User-Friendly Interface**: Simple command-line interface to select the type of project and specify the project name.

## Requirements

- Python 3.x
- Composer (for Laravel)
- Laravel installer
- Django
- Jetstream (optional for Laravel)

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/project-automator.git
    cd project-automator
    ```

2. **Install necessary dependencies**:
    - For Laravel:
      ```bash
      composer global require laravel/installer
      ```
    - For Django:
      ```bash
      pip install django
      ```

## Usage

1. **Run the script**:
    ```bash
    python project_automator.py
    ```

2. **Follow the on-screen instructions**:
    - Select the type of project you want to create.
    - Enter the project name.
    - For Django projects, enter the name of the initial application.

## Example

### Creating a Laravel Project

```bash
python project_automator.py
```
- Select option `1` for a standard Laravel project or `2` for a Laravel project with Jetstream (Inertia.js).
- Enter the project name when prompted.

### Creating a Django Project

```bash
python project_automator.py
```
- Select option `3` for a Django project.
- Enter the project name and the name of the initial application when prompted.

## Script Details

### Functions

- `run_command(command)`: Executes a shell command and handles output.
- `create_laravel_project(project_name, with_jetstream=False)`: Creates a Laravel project and optionally configures Jetstream with Inertia.js.
- `create_django_project(project_name)`: Creates a Django project, sets up an initial application, and configures URLs and models.
- `main()`: Main function to handle user input and project creation.

### Project Structure

```
project-automator/
│
├── project_automator.py   # Main script
└── README.md              # This file
```

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
