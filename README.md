# Note Taker
![alt text](./public/assets/images/Screenshot%202024-03-22%20at%205.27.59 PM.png)
![alt text](./public/assets/images/Screenshot%202024-03-22%20at%205.28.36 PM.png)
## Description

The Note Taker application is designed to allow users to write and save notes. It provides a simple interface for users to organize their thoughts and keep track of tasks they need to complete. The application utilizes an Express.js back end to handle data storage and retrieval, saving and retrieving note data from a JSON file.

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
  - `index.js`: Defines API routes for handling note data.
  - `notes.js`: Defines HTML routes for serving HTML files.
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

- [James House]


