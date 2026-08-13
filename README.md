# EduLearn — Educational Learning Platform (Demo)

This repository contains demo code for *EduLearn*, a simple educational learning platform. It includes:

- A minimal Node.js + Express server with a Tailwind-styled login flow (server demo).
- A standalone front-end login page (`frontend/index.html`) for quick educational experiments.
- A small React single-file SPA demo using CDN builds (in `frontend/react-spa/`).

These demos are intentionally lightweight and self-contained for learning UI and UX patterns — they are not production-ready.

## Contents

- `index.js` — Express server (login stub, sessions, simple dashboard)
- `package.json` — server dependencies and start script
- `views/` — EJS templates for server demo (`login.ejs`, `dashboard.ejs`)
- `frontend/index.html` — single-file Tailwind front-end login demo (no build)
- `frontend/react-spa/index.html` — React SPA demo (CDN + Babel, multiple pages)
- `frontend/*/README.md` — quick notes for each frontend demo

## Features (demo)

- Login form (server-side demo) with session-based auth stub
- Client-side login page with Tailwind and JS validation
- React SPA demo with pages: Home, Courses, Login, Dashboard, Profile, About
- Demo credentials for testing convenience

## Quick Start — Server demo

1. Open a terminal in the repository root (Windows example):

```powershell
cd /d d:/Projects/workshop
npm install
npm start
```

2. Open http://localhost:3000 in your browser.

Server demo credentials (hard-coded):
- username: customer
- password: pets123

Notes:
- The server demo uses Tailwind from the CDN inside the EJS views for convenience.
- Authentication is a stub and stores sessions in memory — do not use in production.

## Quick Start — Front-end demos

- Open the simple front-end demo directly in your browser:

```powershell
start "" "d:/Projects/workshop/frontend/index.html"
```

- Open the React SPA demo (CDN builds) in your browser:

```powershell
start "" "d:/Projects/workshop/frontend/react-spa/index.html"
```

React SPA demo credentials:
- email: student@example.com
- password: learn123

## Development Notes

- To convert the React demo to a full project, scaffold with Vite or Create React App and install Tailwind via PostCSS.
- For production authentication, add a secure backend, hashed passwords, and a persistent database (SQLite, PostgreSQL, MongoDB, etc.).

## Suggested Next Steps

- [ ] Convert the React demo to a Vite app and add proper routing/build.
- [ ] Wire the React SPA to the Express server for real authentication and APIs.
- [ ] Add a small database (SQLite) and user management for enrollments and progress.

## Contributing

This is a learning project — contributions are welcome. Open an issue or send a pull request describing your change.

## License

MIT
