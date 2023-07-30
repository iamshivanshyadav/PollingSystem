# PollingSystem API

Welcome to the PollingSystem API! This API allows you to manage polls, questions, and options for conducting polls and gathering responses from users.

Hosted link: [PollingSystem](https://pollingsystem-8vl1.onrender.com)

## File Structure

The API is organized with the following file structure:

```
PollingSystem
├── configs
│   └── db_connection.js
├── controllers
│   └── api
│       └── v1
│           ├── option_controller.js
│           └── question_controller.js
├── models
│   ├── option.js
│   └── question.js
├── routes
│   └── api
│       └── v1
│           ├── index.js
│           ├── options.js
│           └── questions.js
│       └── index.js
├── index.js
├── package-lock.json
├── package.json
└── vercel.json
```

### Description of directories and files:

- `configs`: Contains configuration files.
  - `db_connection.js`: Configuration file for database connection.
  
- `controllers/api/v1`: Contains API controllers.
  - `option_controller.js`: Controller for handling option-related API endpoints.
  - `question_controller.js`: Controller for handling question-related API endpoints.
  
- `models`: Contains data models for the API.
  - `option.js`: Model representing an option for a poll question.
  - `question.js`: Model representing a poll question.

- `routes`: Contains API routes.
  - `api/v1`: Version 1 of the API routes.
    - `index.js`: Main API entry point for version 1.
    - `options.js`: API routes related to options.
    - `questions.js`: API routes related to questions.

- `index.js`: Main entry point of the PollingSystem API.
- `package-lock.json`: Auto-generated file for package version locking.
- `package.json`: Contains metadata and dependencies for the project.
- `vercel.json`: Configuration file for Vercel deployment (in case of deployment on Vercel platform).

## API Endpoints

The API provides the following endpoints:

### Question Endpoints

- **GET** `/api/v1/questions`: Get all poll questions.
- **POST** `/api/v1/questions/create`: Create a new poll question.
- **DELETE** `/api/v1/questions/:id/delete`: Delete a poll question by its ID.
- **GET** `/api/v1/questions/:id`: Get a specific poll question by its ID.

### Option Endpoints

- **POST** `/api/v1/questions/:id/options/create`: Create a new option for a question.
- **DELETE** `/api/v1/options/:id/delete`: Delete an option by its ID.
- **GET** `/api/v1/options/:id/add_vote`: Add a vote to the option.

Please note that this is just a brief overview of the API. For detailed information on how to use each endpoint, their request/response formats, and possible errors, refer to the API documentation.

## Getting Started

To run the PollingSystem API locally or deploy it to a server, follow these steps:

1. Clone the repository or obtain the source code.
2. Install the required dependencies using `npm install`.
3. Ensure you have a compatible database set up and provide the necessary configuration in `db_connection.js`.
4. Start the API server with `npm start`.

## Contribution

If you wish to contribute to the PollingSystem API, feel free to create pull requests. Please follow the existing code style and include relevant test cases for any new features or bug fixes.

## License

The PollingSystem API is open-source and distributed under the [MIT License](LICENSE). Feel free to use, modify, and distribute it as per the terms of the license.

## Contact

If you have any questions or need further assistance, please feel free to contact the maintainers of the project.

Happy polling! 🗳️
