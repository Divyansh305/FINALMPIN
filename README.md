#MPIN Strength Checker

This project is a Python-based solution for a MPIN (Mobile Banking Personal Identification Number) strength analysis task. It evaluates the security of 4 and 6-digit MPINs by checking them against common patterns and personal demographic data.

The entire solution is contained within a single Jupyter Notebook (mpin_notebook.ipynb) for easy portability and execution in environments like Google Colab.
Features

    Strength Analysis: Classifies an MPIN as either STRONG or WEAK.

    Common PIN Detection: Checks against a comprehensive list of commonly used and easily guessable PINs (e.g., "1234", "1111", "1998").

    Demographic Analysis: Detects if a PIN is derived from personal user data, including:

        User's Date of Birth

        Spouse's Date of Birth

        Wedding Anniversary

    Detailed Reasoning: If a PIN is weak, it provides specific reasons (e.g., COMMONLY_USED, DEMOGRAPHIC_DOB_SELF).

    4 & 6-Digit Support: All checks are compatible with both 4-digit and 6-digit PINs.

    Interactive & Test Modes: The notebook can be run in two modes:

        Interactive Mode: Prompts the user to enter a custom PIN and dates for analysis.

        Test Mode: Runs a full suite of 23 unit tests to verify the correctness of the logic.

How to Use

This project is designed to be run in Google Colab or any standard Jupyter Notebook environment.

    Download the Notebook: Download the mpin_notebook.ipynb file from this repository.

    Upload to Google Colab:

        Go to colab.research.google.com.

        Click on File > Upload notebook... and select the mpin_notebook.ipynb file.

    Run the Cells:

        The notebook is divided into logical cells with Markdown explanations.

        Run the cells sequentially from top to bottom by clicking the "Play" button (▶️) or pressing Shift + Enter.

        The final cells allow you to either run the full test suite or start the interactive checker.

Project Structure (mpin_notebook.ipynb)

The notebook is organized into the following cells for clarity and presentation:

    Introduction: A Markdown cell explaining the project.

    Imports and Constants: A code cell that imports necessary libraries and defines the sets of weak 4 and 6-digit PINs.

    Core Logic Functions: A code cell containing the check_mpin_strength function and its helpers. This is the heart of the program.

    Unit Test Class: A code cell defining the TestMpinChecker class, which contains 23 test cases to validate the logic against the assignment requirements.

    Runner Functions: A code cell with two helper functions: run_all_tests() and run_interactive_checker().

    Execution Cells: Two final code cells that call the runner functions, allowing the user to easily execute the tests or start the interactive mode.

Technologies Used

    Language: Python 3

    Standard Libraries:

        datetime: For handling date objects.

        unittest: For creating and running the test suite.

        typing: For type hints.
