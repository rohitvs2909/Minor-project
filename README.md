# Password Strength Checker

## Overview
The **Password Strength Checker** is a cybersecurity tool designed to evaluate and improve password security. It provides both a **GUI and CLI interface** to help users check the strength of passwords and generate secure ones.

## Team Members
- **Member 1:** A R Shakeel Irfan
- **Member 2:** V S Rohit
- **Member 3:** S Tharun

## Features
- **Dual Interface**: Supports both GUI (Tkinter) and CLI modes.
- **Password Strength Analysis**: Uses `zxcvbn` for realistic strength evaluation.
- **Password Generation**: Creates strong, random passwords of customizable length.
- **Security Checks**:
  - Minimum length requirements
  - Character complexity (uppercase, lowercase, numbers, special characters)
  - Detection of common and banned passwords
- **Improvement Suggestions**: Provides tips to strengthen weak passwords.
- **Logging**: Tracks password checks for security auditing.

## Installation

### Prerequisites
- **Python 3.x** must be installed on your system.
- Required Python packages: `tkinter`, `zxcvbn`.

> **macOS users:** The GUI depends on the system's Tcl/Tk
> libraries. Some older versions of macOS (Darwin&nbsp;16 / macOS
> 10.12 and earlier) ship with a Tk build that aborts when a window
> is created. The script detects this situation and automatically
> falls back to the CLI interface rather than crashing.

### Install Dependencies
```bash
pip install pyzxcvbn
```

## Usage

### GUI Mode
Run the following command to start the graphical interface:
```bash
python password_strength_checker.py
```

### CLI Mode
1. **Check a password’s strength**:
```bash
python password_strength_checker.py --check "your_password_here"
```

2. **Generate a strong password**:
```bash
python password_strength_checker.py --generate --length 20
```

### Command Line Arguments
- `--cli` : Launches interactive CLI mode.
- `--check PASSWORD` : Checks the strength of a given password.
- `--generate` : Generates a strong password.
- `--length N` : Specifies password length (default: 16 characters).

## Logging
All password checks are logged in `password_checker.log`, recording:
- Timestamp
- Action performed
- Password strength rating

## Security Notes
- No passwords are stored permanently.
- The tool works entirely offline.
- Secure random generation ensures strong passwords.

## License
This project is licensed under the **Apache 2.0 License**. See the [LICENSE](LICENSE) file for details.

## Contributing
Feel free to fork the repository, submit issues, or create pull requests for improvements.

## Contact
For any questions, contact:
- **Member 1:** A R Shakeel Irfan - shakeelirfan1997@gmail.com
- **Member 2:** V S Tharun - rohitvs250@gmail.com
- **Member 3:** S Tharun - tharun0610@gmail.com

