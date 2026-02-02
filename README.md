# ALU Regex Data Extraction & Secure Validation

## Overview

This project is a Python-based program designed to **extract structured data from raw text** and **validate it securely**. It demonstrates realistic data handling, robust regex extraction, and awareness of unsafe or malicious input.  

It is part of a coding assignment to showcase **accuracy, robustness, and security awareness** in data processing.

---

## Features

The program can:

- Extract and validate **emails**, **URLs**, **phone numbers**, and **credit card numbers**.
- Handle **realistic variations** of data formats, e.g., different phone number styles, URL formats, and credit card separators.
- Reject or ignore **malformed or malicious input**, e.g., emails with double `@@`, URLs starting with `javascript:`, and invalid credit card numbers.
- Mask sensitive information (credit card numbers) to prevent unnecessary exposure.
- Output results in a **readable JSON format**.

---

## Requirements

- Python 3.6+
- No external libraries required (uses built-in `re` and `json` modules)

---

## Sample Input

```text
Hello Team,

Please contact us at info@example.com or support@company.co.uk for inquiries.
Our website URLs are https://www.example.com and http://subdomain.example.org/page.

You can also call us at (123) 456-7890, 123-456-7890, or 123.456.7890.
For credit card payments, use 1234-5678-9012-3456 or 4321 8765 2109 6543.
Beware of fake emails like hacker@@evil.com or badcard 1111-2222-333.

Thanks,
Admin
