# Online Transport Service

An initial Final Year Project (FYP) for a web-based transport service connecting passengers with local drivers in Bhakkar, Pakistan. The current version provides a simple project introduction screen and a starter backend; booking and account features are planned for later development.

## Current Project Stage

- React frontend initialized with a centered project title and description.
- Express backend initialized with a health-check endpoint.
- Frontend production build and lint checks pass.
- User accounts, ride booking, and database integration are not implemented yet.
- GitHub push and proof-of-work screenshots/recording still need to be completed.

## Technology Stack

| Area | Technology |
| --- | --- |
| Frontend | React, JavaScript, CSS, Vite |
| Backend | Node.js, Express |
| Planned database | MongoDB (Mongoose dependency is present; database connection is not configured yet) |
| Development tools | Visual Studio Code, Git, npm |

Bootstrap is not currently installed or used. See [the implementation plan](docs/implementation-plan.md) for the proposed project architecture and future scope.

## Project Structure

```text
online-transport-service/
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── package.json
│   └── server.js
├── docs/
│   └── implementation-plan.md
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── App.css
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
└── README.md
```

## Prerequisites

- Node.js and npm
- Git
- A code editor such as Visual Studio Code

MongoDB will be needed when database integration is implemented. The current starter backend does not require a database connection to run.

## Setup and Run Locally

Install dependencies in each application directory:

```bash
cd frontend
npm install
cd ../backend
npm install
```

Start the frontend and backend in separate terminals from the project root:

```bash
cd frontend
npm run dev
```

```bash
cd backend
npm run dev
```

Open the local URL printed by Vite in the frontend terminal. The backend listens on port `5000` by default; set the `PORT` environment variable to use a different port.

Check that the backend is running by opening:

```text
http://localhost:5000/api/health
```

The endpoint returns a JSON message confirming that the starter backend is running. The frontend and backend are not connected yet.

## Frontend Checks

Run these commands from the `frontend/` directory:

```bash
npm run build
npm run lint
```

## Planned Work

- Connect the backend to MongoDB.
- Implement passenger and driver accounts and profiles.
- Add ride requests, booking status, and booking history.
- Develop administration and driver availability features.
- Add testing and deployment after core functionality is complete.
- Capture screenshots or a short recording of the local project and Git workflow for assignment evidence.

## Developer

Muhammad Hasnian Tahir
