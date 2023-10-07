# Google Sheets Auto-Invoice Script

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Challenges and Solutions](#challenges-and-solutions)
4. [Technologies and Methods Used](#technologies-and-methods-used)
5. [Demo](#demo)
6. [Google Sheet Template](#google-sheet-template)
7. [License](#license)

## Overview

This project is a Google Sheets script designed to automate the process of generating invoices for gigs. The script is part of a larger system that manages gig data, including client information, job details, and payment rates. The script triggers automatically upon specific user actions in the Google Sheet and performs various tasks such as data validation, invoice generation, and email draft creation.

## Features

- **Auto-Trigger for Invoice Generation**: The script automatically prompts the user to generate an invoice when a gig status is set to 'Done'.
- **Data Validation**: Ensures that all necessary fields are filled out before proceeding with invoice generation.
- **Dynamic Invoice Creation**: Generates a new invoice by pulling data from multiple sheets and populating an invoice template.
- **Client Information Retrieval**: Automatically fetches client information like address and contact details from a separate 'Clients' sheet.
- **Email Draft Creation**: Automatically creates an email draft with the invoice details, ready to be reviewed and sent.

## Challenges and Solutions

- **Auto-Triggering**: One of the challenges was to auto-trigger the invoice generation process when a gig status changes. This was solved using Google Sheets' `onEdit` trigger.
  
- **Data Retrieval**: The script had to pull data from multiple sheets to generate an invoice. This was achieved using Google Apps Script's `getRange` and `getValues` methods.

- **Dynamic Invoice Numbering**: Generating unique invoice numbers for each client was a challenge. This was solved by maintaining a separate 'config' sheet that keeps track of the last invoice number for each client.

## Technologies and Methods Used

- **Google Apps Script**: The backbone of the project, used for automating Google Sheets.
- **Google Sheets API**: Used for reading and writing data to Google Sheets.
- **JavaScript**: The script is written in JavaScript, which is the language supported by Google Apps Script.

## Demo

Here's how the script works in action:

![Auto-Invoice Demo](./demo.gif)

## Google Sheet Template

You can view and make a copy of the Google Sheet template [here](your-google-sheet-link).

## License

This project is licensed under the MIT License. See the [LICENSE.md](LICENSE.md) file for details.

---

Feel free to customize this README to better fit your project's specific needs.
