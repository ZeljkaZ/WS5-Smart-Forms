# Smart Form Project

## Overview

This project is part of the **Dynamic Web Applications with JavaScript** course. The goal of this assignment was to build a **dynamic, interactive form** that demonstrates key JavaScript concepts, including validation, autosave, error handling, accessibility, and UX improvements.

---

## Features

### 1. Form Validation

- Real-time validation (as the user types) and on submission.
- Errors are shown below each input and summarized in a red box at the top.
- Fields use `aria-invalid` for accessibility.
- Focus moves automatically to the first invalid field on submit.

### 2. Phone Number Normalisation

- Formats phone numbers on blur.
- Converts local numbers starting with `0` to Finland international format `+358`.
- Preserves numbers starting with `+`.
- Improves consistency without forcing input masks.

### 3. Company Section Toggle

- Selecting “Register as a company” reveals the company name field.
- Required validation only applies if the company checkbox is checked.
- Hidden fields do not trigger validation.

### 4. Autosave

- Input data is saved automatically to `localStorage`.
- Refreshing the page restores previously entered data.
- Passwords are saved for demo purposes only and should **not** be stored in production.

### 5. Clear Button

- Resets the form and deletes saved draft data.
- Clears error messages and hides optional sections.

### 6. Accessibility

- Visible labels linked with `for` and `id`.
- Error messages and summaries use ARIA attributes and alert regions.
- Fully navigable via keyboard (`Tab` key).
- Colors are not the sole conveyer of meaning.

### 7. Debugging

- `console.log` statements show autosave, restoration, and phone normalisation.
- Tested with browser developer tools to ensure no errors and proper functionality.

---

## Learning Goals

This assignment helped achieve the following learning goals:

- Adopt a **clear JavaScript style** with proper naming, small functions, and comments.
- Set up **ESLint and Prettier** for automated code quality and formatting.
- Design **accessible forms** with labels, hints, ARIA attributes, and keyboard support.
- Use **HTML5 input types and attributes** for improved validation and mobile UX.
- Apply the **Constraint Validation API** with custom error messages.
- Validate fields on blur and submit with **debounced checks** for performance.
- Submit data safely, preventing XSS and handling server responses.
- Implement **autosave** with `localStorage` and data restoration.
- **Normalise phone numbers** and use a **honeypot** field for bot detection.
- Ensure **progressive enhancement**, allowing the form to work even without JavaScript.

---

## Workshop Content

The project covers the following workshop topics:

- Naming conventions, comments, folder layout, and module patterns.
- Configuring **ESLint** and **Prettier** in VS Code.
- Building a smart form with email, password, confirm password, and select fields.
- Validation using `required`, `pattern`, `minlength`, `maxlength`, and `customValidity`.
- UX improvements: inline messages, ARIA live feedback, show/hide rules, error summary.
- Progressive enhancement with normal POST and optional `fetch` submission.
- Autosave using `localStorage` with debounce.
- Phone normalisation and honeypot for security.
- GitHub submission with clear file structure.

---

## Repository Content

- **index.html** – The HTML structure of the smart form.
- **styles.css** – Styling for the form.
- **app.js** – JavaScript logic for validation, autosave, phone normalisation, dynamic company field, and form submission.
- **screenshots/** – Folder containing relevant screenshots.
- **README.md** – This file with assignment description, objectives, and screenshots.

## How to Run

1. Open the project folder in **VS Code**.
2. Install the **Live Server** extension if not already installed.
3. Open `index.html` and click **Go Live** in the bottom-right corner.
4. The form will open in your browser (e.g., `http://127.0.0.1:5500/index.html`).
5. Test the features: typing, phone normalisation, toggling company fields, autosave, clearing, and submission.

