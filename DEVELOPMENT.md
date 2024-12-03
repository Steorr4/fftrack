### Developer's Guide for the FFTrack Project

#### 1. Introduction
This project aims to identify songs from audio input using audio fingerprinting technology. This document guides developers through the setup, development process, and standards for contributing to the project.

#### 2. Getting Started

**Prerequisites**: Ensure you have Python (version 3.7 or newer) and SVN installed on your machine. If not, download and install them from the official websites.

**Environment Setup**:
- **Development Environment**: We recommend using Visual Studio Code or PyCharm as your IDE. Set up a virtual environment for the project by running `python -m venv venv` in the project root, then activate it with `source venv/bin/activate` (Linux/Mac) or `venv\Scripts\activate` (Windows).
- **Dependency Management**: Install required dependencies by running `pip install -r requirements.txt`.

#### 3. Project Structure

The project is organized as follows:
- `fftrack/`: Main package containing all source code.
  - `main.py`: Entry point for the application.
  - `database/`: Contains database models and management scripts.
  - `audio/`: Audio processing components.
  - `matching/`: Song matching algorithms.
  - `ui/`: User interface components. (CLI, GUI, etc.)
- `scripts/`: Utility scripts for database initialization and other tasks.
- `tests/`:
  - `database_tests/`: Tests for database models and management scripts.
  - `audio_tests/`: Tests for audio processing components.
  - `matching_tests/`: Tests for song matching algorithms.
  - `ui_tests/`: Tests for the user interface.

- `requirements.txt`: Project dependencies.

#### 4. Development Workflow

**Version Control Practices**: Make a new branch for new features or bug fixes. Name branches meaningfully, e.g., `/audio-enhancement`. Commit messages should be concise, and meaningful, for example 
- `Fix bug in database model creation`
- `Add audio processing module for FFT`
- `Update UI to display song matches in a list`


**Issue Tracking and Task Management**: Tasks are managed using NOTION. Create a new task for each feature or bug fix, and link it to the relevant branch in SVN. Update the task status as you progress. Finally, close the task and add it to the Forge.

#### 5. Coding Standards and Practices

**Coding Conventions**: Follow PEP 8 guidelines for Python code. Ensure your code is clean, well-commented, and easy to understand.

**Code Documentation**: Document your code with comments and docstrings. Use Google style for docstrings.
Example:
```python
def add(x, y):
    """Add two numbers together.

    Args:
        x (int): First number.
        y (int): Second number.

    Returns:
        int: Sum of x and y.
    """
    return x + y
```

**Testing Practices**: Write unit tests for your code using `pytest`. Aim for a test coverage of at least 70%. Run tests locally with `coverage run -m pytest` and view the report with `coverage report`.

**Code Reviews**: You code will be reviewed by other team members before merging to ensure quality and consistency.

#### 6. Quality Assurance

**Testing Strategies**: Our testing strategy includes unit tests for individual components and integration tests for testing components together. Use `pytest` for writing tests.

**Linting**: Run `flake8` on your code to ensure it meets our coding standards. Install `flake8` via pip and run `flake8 path/to/your/code` to check for issues.
You can also install the `flake8` extension in your IDE to get real-time feedback. (Recommended)