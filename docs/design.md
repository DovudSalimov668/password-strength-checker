# Password Strength Checker Design

## Project Goal

Develop a Python-based password strength checker that evaluates passwords using common cybersecurity principles and provides actionable recommendations for improvement.

## Technologies

* Python 3.13
* Tkinter (GUI)
* Git
* GitHub
* Pytest (planned)

---

## Features

### Password Validation

The application will check:

* Password length
* Presence of lowercase letters
* Presence of uppercase letters
* Presence of numbers
* Presence of special characters

### Strength Evaluation

The application will:

* Calculate a password strength score
* Classify passwords as Weak, Medium, or Strong
* Display recommendations for improvement

### User Interface

The application will provide a graphical interface using Tkinter.

GUI components:

* Password input field
* Check Password button
* Clear button
* Strength label
* Strength progress bar
* Suggestions area

### Color Indicators

* Weak = Red
* Medium = Yellow
* Strong = Green

---

## Scoring System

A password receives one point for each criterion met:

* Length >= 8 characters
* Contains lowercase letters
* Contains uppercase letters
* Contains numbers
* Contains special characters

Maximum score: 5

---

## Strength Levels

### Weak

Score: 0-2

Characteristics:

* Easy to guess
* Missing multiple security requirements

### Medium

Score: 3-4

Characteristics:

* Meets most requirements
* Can be improved

### Strong

Score: 5

Characteristics:

* Meets all defined requirements
* Better resistance against common attacks

---

## Program Flow

1. User launches the application

2. GUI window opens

3. User enters a password

4. User clicks "Check Password"

5. The application checks:

   * Length
   * Lowercase letters
   * Uppercase letters
   * Numbers
   * Special characters

6. The application calculates a score

7. The application determines the strength level

8. The application generates recommendations

9. The GUI displays:

   * Strength level
   * Score
   * Recommendations

---

## Project Architecture

### main.py

Responsibilities:

* Start the application
* Launch the GUI

### gui.py

Responsibilities:

* Build the Tkinter interface
* Receive user input
* Display results
* Update visual elements

### checker.py

Responsibilities:

* Perform password analysis
* Calculate scores
* Generate recommendations
* Return results to the GUI

---

## Planned Functions

### checker.py

* check_length()
* check_lowercase()
* check_uppercase()
* check_numbers()
* check_special_characters()
* calculate_score()
* determine_strength()
* generate_suggestions()

### gui.py

* create_window()
* check_password()
* update_ui()
* clear_fields()

---

## Future Security Enhancements

Planned improvements:

* Password entropy calculation
* Common password detection
* Dictionary word detection
* Password breach database checking
* Password generation feature
* Password history analysis
* Export analysis results

---

## Known Limitations (Version 1)

The first version will not:

* Detect leaked passwords
* Calculate entropy
* Check password dictionaries
* Detect keyboard patterns
* Detect password reuse

These features may be implemented in future versions.
