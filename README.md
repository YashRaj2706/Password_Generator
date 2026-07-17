# Secure Password Strength Checker

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
