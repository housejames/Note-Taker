# Note Taker

## Description

The Note Taker application is designed to allow users to write and save notes. It provides a simple interface for users to organize their thoughts and keep track of tasks they need to complete. The application utilizes an Express.js back end to handle data storage and retrieval, saving and retrieving note data from a JSON file.

## User Story

As a small business owner, I want to be able to write and save notes so that I can organize my thoughts and keep track of tasks I need to complete.

## Acceptance Criteria

- When the Note Taker is opened, users are presented with a landing page containing a link to a notes page.
- Clicking on the link to the notes page displays existing notes in the left-hand column and empty fields to enter a new note title and text in the right-hand column.
- Upon entering a new note title and text, "Save Note" and "Clear Form" buttons appear in the navigation at the top of the page.
- Clicking the "Save Note" button saves the new note and displays it in the left-hand column with other existing notes, while hiding the navigation buttons.
- Clicking on an existing note in the list displays that note in the right-hand column and reveals a "New Note" button in the navigation.
- Clicking the "New Note" button presents users with empty fields to enter a new note title and text, while hiding the button.

## Getting Started

### Installation

1. Clone the repository.
2. Install dependencies using `npm install`.

### Usage

1. Ensure you have Node.js installed on your machine.
2. Navigate to the project directory in your terminal.
3. Run `npm start` to start the server.
4. Open your web browser and navigate to `http://localhost:3000` to access the application.

## File Structure

- `db.json`: JSON file used to store and retrieve notes.
- `public/`
  - `assets/`: Contains CSS and JavaScript files.
  - `index.html`: Landing page HTML.
  - `notes.html`: Notes page HTML.
- `routes/`
  - `apiRoutes.js`: Defines API routes for handling note data.
  - `htmlRoutes.js`: Defines HTML routes for serving HTML files.
- `server.js`: Main entry point for the application.

## Routes

### HTML Routes

- `GET /notes`: Returns the notes.html file.
- `GET *`: Returns the index.html file.

### API Routes

- `GET /api/notes`: Reads the db.json file and returns all saved notes as JSON.
- `POST /api/notes`: Receives a new note to save on the request body, adds it to the db.json file, and returns the new note to the client.

## Technologies Used

- Node.js
- Express.js

## Contributors

- [Your Name]

## License

This project is licensed under the [MIT License](LICENSE).
