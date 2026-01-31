# IT23323902
ITPM Assignment 1
Playwright Automation – Singlish to Sinhala Translator
Student Registration Number: IT23323902

Project Overview
This project contains automated end-to-end test cases developed using Playwright to test the SwiftTranslator web application. The purpose of this project is to evaluate the accuracy of converting Singlish input into Sinhala output and to validate basic UI behavior such as real-time output updates, as required for Assignment 1 of the IT3040 – ITPM module.

Application Under Test
https://www.swifttranslator.com/

Technologies Used
Node.js
Playwright Test Framework
JavaScript
xlsx library for Excel-based test data handling

Project Folder Structure

IT23323902
├── data
│ └── IT23323902.xlsx
├── scripts
│ └── readExcel.js
├── tests
│ └── translator.spec.js
├── playwright.config.js
├── package.json
└── README.txt / README.md

Prerequisites
Node.js must be installed on the system (version 18 or higher is recommended).
npm must be available to install dependencies.

Installation Steps

Open the project folder named IT23323902 in Visual Studio Code.

Open a terminal in the project root directory.

Install required dependencies by running:

npm install

Install Playwright browsers using:

npx playwright install

Excel Test Data Setup
All test cases are stored in an Excel file.
The Excel file must be placed inside the data folder with the exact name:

IT23323902.xlsx

The tests will not run if the file name or location is changed.

Running the Tests
To execute all Playwright tests:

npx playwright test

To run tests only in the Chromium browser:

npx playwright test --project=chromium

To run tests in headed mode (browser visible):

npx playwright test --headed

Test Execution Details
Test cases are generated dynamically by reading data from the Excel file.
Each row in the Excel sheet represents a test case.
If the Excel file cannot be read, Playwright will not generate tests and will display “No tests found”.

Common Errors and Solutions

Error: ENOENT – no such file or directory
This error occurs when the Excel file is missing, renamed, or placed outside the data folder. Ensure that data/IT23323902.xlsx exists.

Error: No tests found
This usually happens when the Excel file fails to load or contains no valid test case data.

Academic Information
Module: IT3040 – IT Project Management
Degree Programme: BSc (Hons) in Information Technology
Year: 3
Semester: 2
Assignment: Assignment 1
Student Registration Number: IT23323902
