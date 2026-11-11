# Architecture

How the main parts connect. Read this before adding a module or changing how
parts talk to each other. Describe the shape, not every file.

## Parts

- **Frontend** (src/): Vue 3 single-page application with TypeScript, styled with Tailwind CSS. The app is currently static, focused on the login screen and the first UI flow.
- **Static assets** (public/): icons, images, and other files that do not need a build step.
- **No backend yet**: the project is intentionally frontend-only for the first phase; authentication and task storage are not implemented yet.

## How they connect

- The app runs as a client-side Vue interface in the browser.
- The user interacts with forms, validation states, and screen transitions directly in the frontend.
- A future backend, if added later, will sit behind the frontend and connect through a dedicated API boundary.

## Data

- For now, user and task information live only in the browser state or are mocked during UI development.
- No database or server-side persistence is required for the login page milestone.
- The frontend keeps the logic local and isolated so the UI can be tested visually before backend work begins.

## What does not belong here

How to start the project (docs/dev-environment.md) and why a choice was made
(docs/decisions.md).
