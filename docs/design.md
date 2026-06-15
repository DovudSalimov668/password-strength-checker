# Password Strength Checker Design

## Project Goal

Evaluate password strength using common cybersecurity principles.

## Features

- Password length validation
- Uppercase detection
- Lowercase detection
- Number detection
- Special character detection
- Strength scoring
- Improvement suggestions

## Scoring

+1 point:
- Length >= 8
- Lowercase present
- Uppercase present
- Number present
- Special character present

Maximum Score = 5

## Strength Levels

0-2 points = Weak

3-4 points = Medium

5 points = Strong

## Program Flow

1. User enters password

2. Program checks:
   - Length
   - Uppercase letters
   - Lowercase letters
   - Numbers
   - Special characters

3. Program calculates score

4. Program determines strength

5. Program displays suggestions

6. Program displays final result

## Planned Functions

check_length()

check_lowercase()

check_uppercase()

check_numbers()

check_special_characters()

calculate_score()

generate_suggestions()

## Future Security Enhancements

- Common password detection
- Dictionary word detection
- Entropy calculation
- Password breach database checking