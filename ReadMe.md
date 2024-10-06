# Portfolio
#### The is rehab patient tracking, 22/09/2024
#### **By EMMACULATE MWIKALI**

## Getting Started
*Download the Files: Download the entire website directory which      includes HTML, CSS, image, and js .
* Download a zip in the code button to the desired folder
* Extract the files
* Open the extracted folder with VSCode
* Go live or open the index.html file with chrome
* fill the form and test js
* And you are all done

## Description
### Rehab Patient Tracking System

## index.html file
This is a basic HTML page that serves as the starting point for a rehab patient tracking system.

### Features:

This is a basic HTML foundation for a rehab patient tracking system. It allows users to:

 *Submit new patient information, including name, guardian name, stage, progress,    guardian phone number, doctor email, and priority.
 *Search for patients by name using a search bar.
 *View a list of all patients (initially empty, populated as data is submitted).
## Important Files:

index.html (assumed): This is the main HTML file that defines the overall structure of the web page.
   *style.css (assumed): This file contains CSS styles that control the appearance of the web page (not included in the code snippet).
    *script.js (assumed): This JavaScript file contains code that handles user interactions and data manipulation (not included in the code snippet).
### HTML Structure:

Document Declaration (<!DOCTYPE html>): This line specifies the document type as HTML.
HTML Tag (<html lang="en">): This tag is the root element of the HTML document and defines the language used (English in this case).
Head (<head>): This section contains meta information about the document.
Meta Tags (<meta>):
charset="UTF-8": Specifies the character encoding of the document for displaying various languages.
viewport="width=device-width, initial-scale=1.0": Controls how the page scales on different devices.
keywords: Optional keywords for search engines.
author: Optional information about the author.
title: Defines the title of the web page, displayed in the browser tab.
Stylesheet Link (<link rel="stylesheet" href="style.css">): Links to the external CSS file that styles the page.

### code 
Body (<body>): This section contains the visible content of the web page.
Header (<h1>): Displays a large heading "Rehab Patient Tracking" centered on the page.
Search Container (<div class="search-container">): Contains the search functionality.
Image (<img>): Displays an image related to rehab (likely defined in CSS).
Search Input (<input>): A text field for entering patient names to search.
Search Button (<button>): A button to initiate the search.
Main Content (<main class="container">): Holds the main content of the page.
Patient Information Form (<form id="patientForm">): Allows users to enter new patient information. Each input field has a corresponding label.
Required fields are indicated with the required attribute.
Patient List (<div id="patientList" class="mt-4">): Initially empty, this section will display a list of patients (populated from JavaScript).
Footer (<footer>): Displays copyright information and contact details for the rehab tracking system.
Script Link (<script src="script.js"></script">): Links to the external JavaScript file that handles functionalities.

### unctionality (requires JavaScript):

Upon submitting the form, patient information is collected and likely stored in an array or database (handled by JavaScript).
The search input allows users to filter the displayed patients by name (implemented by JavaScript).


*Edit and delete functionalities for patients.
*Implementing sorting options for the patient list (e.g., by priority, stage).
*Storing patient data persistently (e.g., using local storage or a database).

## javascrip code
This JavaScript code provides the core functionality for a basic rehab patient tracking system. 

### It interacts with an HTML form to:

*Collect patient data: Name, guardian name, stage, progress, guardian phone number, doctor email, and priority.
*Validate input: Ensures all required fields are filled.
*Add new patients: Stores patient information in an in-memory array (patients).
*Edit existing patients: Allows updating details of a selected patient.
*Delete patients: Removes patients from the array based on their index.
*Search patients by name: Filters the displayed patient list based on the search term.
*Display patient list: Generates HTML elements representing each patient with their information and edit/delete buttons.

### Functionality:

### Event Listeners:

 #### 1.Form Submission:
                     Prevents default form submission behavior.
                     Extracts patient data from form fields.
                     Validates input (all required fields are filled).

 ####  2.If editing an existing patient:
                    Updates the corresponding object in the patients array.
                    clears the form and resets the editingPatientIndex flag.
                    Displays a success message and updates the patient list.

#### 3.If adding a new patient:
Pushes a new object with patient data to the patients array.
Clears the form.
Displays a success message and updates the patient list.

#### 4.Search Input Keyup:
Gets the search term entered in the search input field (converted to lowercase Calls the displayPatients function with the search term.
   
#### 5.Search Button Click (if implemented):
    Triggers the same functionality as the search input keyup event.

 #### 6.displayPatients Function:
 Clears the existing patient list content. Initializes a patientsFound flag set to false.Iterates through the patients array:If there's no search term or the patient's name (lowercase) includes the search term: Sets patientsFound to true.Creates a new HTML element (div) for the patient.Sets appropriate class names for the patient item and priority level.

 #### buttons
Constructs HTML content for the patient, including name, guardian details, stage, progress, phone, email, and edit/delete buttons. Appends the patient element to the patientList container in the HTML.
Attaches click event listeners to the edit and delete buttons:

#### 7.Edit Button:
Populates the form with the selected patient's data.Sets the editingPatientIndex flag to the patient's index in the array. Displays the updated patient list (without hiding the current item).
   
#### 8.Delete Button:
Removes the patient from the patients array based on the index.
    
#### 9.Updates the displayed patient list.
If no patients match the search term after iterating, displays a message indicating "No patient found by that name."


### Live server
* You can view the web live on h
https://github.com/EMMA-KAREN/wk2.code-challage
### Known Bugs
The application works perfectly well, hopefully no bugs.

### Technologies Used
HTML, CSS , js, GIT



### Support and contact details
Contact details (mumokaren@gmail.com, 079792951, )

### License

*LIcenced under the [MT-licence]https://github.com/EMMA-KAREN/my-model-pertfolio/blob/master/LICENCE.md)