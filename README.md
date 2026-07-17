# Password Generator and Strength Checker

A Python-based authentication security utility that analyzes user passwords for strength, policy compliance, and personal data exposure. 

This project demonstrates two methodologies for password validation: a custom regex-based policy ruleset and a pattern-recognition/entropy-based evaluation utilizing Dropbox's `zxcvbn` library.

## Features

- **Personal Data Protection**: Rejects passwords that contain parts of the user's email address or mobile number.
- **Entropy & Pattern Matching**: Analyzes passwords against dictionary words, common names, keyboard patterns, and sequences.
- **Custom Rule Compliance**: Validates length, casing, numbers, and special characters.
- **Actionable Feedback**: Provides clear suggestions to users on how to fix weak passwords.

## Installation

This project requires Python 3.x and the `zxcvbn` library.

 ```bash
 pip install zxcvbn
```
## Uses of zxcvbn:
Because zxcvbn() function instantly checks the password against built-in lists of:

-**Common passwords** (like password, 123456, qwerty).
-**Keyboard spatial patterns** (like asdfgh or zaq12wsx).
-**Repeating sequences** (like aaaaa) or dates (like 1995).

## Future Roadmaps for Production
To turn this utility into a production-grade authentication engine, the following components should be added:

-**Password Generate**: Create password using mobile numbers and emails.
-**Password Hashing**: Implement bcrypt or Argon2 before database storage.
-**HaveIBeenPwned API**: Check if passwords have been exposed in historical public breaches.
-**Rate Limiting**: Add brute-force protection to lock accounts after multiple failed attempts.
-**Multi-Factor Authentication (MFA)**: Generate Time-based One-Time Passwords (TOTP).
