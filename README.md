Email Validator

A Python project to validate email addresses based on a comprehensive set of rules to ensure they follow standard email formatting and restrictions.

Table of Contents

Overview

Features

Rules for Validation

Installation

Usage

Example

Contributing

License

Overview

This project provides a Python script that checks whether an email address is valid or invalid. It uses multiple validation checks to cover common email formatting rules, including restrictions on special characters, domain structure, and length.

Features

Ensures exactly one '@' symbol is present.

Validates local part and domain part separately.

Checks for illegal characters in both local and domain parts.

Prevents consecutive punctuation marks (e.g., !!).

Checks for the presence of at least one dot in the domain part.

Ensures local part length does not exceed 64 characters.

Prevents underscores (_) in the domain part.

Checks for valid top-level domain (TLD).

Ensures the total email length does not exceed 254 characters.

Prevents spaces in the email address.

Rules for Validation

The email is considered valid if it meets all the following criteria:

Contains exactly one '@' symbol.

Does not start with - or @.

The local part contains only alphanumeric characters or allowed special characters:
., _ - ! # $ % & ' * + / = ? ^ { } | ~ ,

No consecutive punctuation marks (e.g., !!).

The domain part:

Contains at least one .

Contains only alphanumeric characters and .

Does not contain _

Length rules:

Local part ≤ 64 characters

Entire email ≤ 254 characters

Email does not contain spaces.

The @ symbol is not more than 6 characters from the end.

Ends with a valid alphabetic TLD.
