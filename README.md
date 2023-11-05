# Pwned Password Checker

A simple Python script to check if a password has been exposed in a data breach using the "Have I Been Pwned" API.

## Features

- Checks the password against a database of known compromised passwords.
- Provides the number of times the password has been found in breaches.

## Prerequisites

- Python 3.x
- Required Python packages: requests

Install the required package using pip:

```bash
pip install requests

Usage
1.Clone the repository or download the script.
2.Run the script in your terminal:

python pwned_password_checker.py

3.Enter the password you want to check.
4.The script will query the "Have I Been Pwned" API and display the results.

type "break" to exit
password: mysecretpassword
mysecretpassword was found 12345 times

How It Works
The script computes the SHA-1 hash of the password and sends the first five characters to the "Have I Been Pwned" API. It then checks if the remaining characters of the hash exist in the response, which contains a list of known breached passwords.

License
This project is licensed under the MIT License. See the LICENSE file for details
