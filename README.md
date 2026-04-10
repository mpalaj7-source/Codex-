# AI-Powered Coding App

## Overview
This project is designed to help users with coding by providing smart suggestions and snippets.

## Features
- **Code suggestions**: Offers real-time code suggestions based on input.
- **Multi-language support**: Compatible with popular programming languages like Python, JavaScript, and C++.
- **Context-aware**: Understands the context of your code to provide relevant snippets.
- **Collaborative editing**: Enables multiple users to work on the same project simultaneously.

## Prerequisites
- Node.js (version 14 or higher)
- npm (Node Package Manager)
- MongoDB (version 4.0 or higher)

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/mpalaj7-source/Codex-
   cd Codex-
   ```
2. Install the dependencies:
   ```bash
   npm install
   ```
3. Set up the database:
   - Ensure that MongoDB is running and accessible.
   - Create a database named `codex_db`.
4. Configure environment variables in a `.env` file:
   ```
   DB_URI=mongodb://localhost:27017/codex_db
   PORT=3000
   ```
5. Start the application:
   ```bash
   npm start
   ```

## Project Structure
```
Codex-
│
├── src
│   ├── controllers  # Handles API requests
│   ├── models       # Database models
│   ├── routes       # API routes
│   └── utils        # Utility functions
├── .env             # Environment variables
├── package.json     # npm package configuration
└── README.md        # Project documentation
```

## API Routes
- **GET** `/api/suggestions` - Fetches code suggestions based on the current input.
- **POST** `/api/code` - Submits code for analysis and feedback.
- **GET** `/api/languages` - Returns a list of supported programming languages.
- **POST** `/api/collab` - Starts a collaborative session.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
