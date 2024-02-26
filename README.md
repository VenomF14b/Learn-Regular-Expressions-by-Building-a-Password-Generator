# Learn-Regular-Expressions-by-Building-a-Password-Generator
This Python script generates strong passwords based on specified criteria such as length, inclusion of numbers, special characters, uppercase, and lowercase letters.

Password Generator
Description
This Python script generates strong and secure passwords based on specified criteria such as length, inclusion of numbers, special characters, uppercase, and lowercase letters. It utilizes the secrets module for secure random password generation and validates generated passwords to ensure they meet specified constraints using regular expressions.

Features
Customizable password length and character composition.
Generates passwords with a mix of uppercase letters, lowercase letters, numbers, and special characters.
Ensures password strength by validating against specified constraints.
Secure random password generation using the secrets module.

Installation
Clone the repository to your local machine:

bash
git clone https://github.com/yourusername/password-generator.git


python
from password_generator import generate_password

# Generate a default password (16 characters, with at least one of each: number, special character, uppercase, lowercase)
new_password = generate_password()
print('Generated password:', new_password)

# Generate a password with custom length and constraints
custom_password = generate_password(length=20, nums=2, special_chars=2, uppercase=2, lowercase=2)
print('Custom password:', custom_password)

Parameters
length: Length of the generated password (default is 16).
nums: Minimum number of digits in the password (default is 1).
special_chars: Minimum number of special characters in the password (default is 1).
uppercase: Minimum number of uppercase letters in the password (default is 1).
lowercase: Minimum number of lowercase letters in the password (default is 1).

Examples
Generate a Default Password
python
new_password = generate_password()
print('Generated password:', new_password)

Generate a Custom Password
python
custom_password = generate_password(length=20, nums=2, special_chars=2, uppercase=2, lowercase=2)
print('Custom password:', custom_password)

Contributing
Contributions are welcome! If you have any suggestions, improvements, or feature requests, please feel free to open an issue or submit a pull request.
