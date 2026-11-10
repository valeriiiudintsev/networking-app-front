# Networking App Frontend

A social-network frontend built with React, TypeScript, Redux, and Material UI. Supports registration and login, user profiles, a post feed, and creating posts with images. Friends and user-directory pages are currently placeholders.

## Run

Requires Node.js and npm, plus a running compatible backend (not included in this repository).

```sh
npm ci
```

Set `REACT_APP_API_URL` in `.env.local` to your backend's base URL, without a trailing slash. For example, if it runs on port 5000:

```dotenv
REACT_APP_API_URL=http://localhost:5000
```

The client uses this URL for `/api/auth`, `/api/posts`, `/api/user`, and uploaded images.

```sh
npm start
```

Open the URL printed by the development server. The configured `homepage` uses `/networking-app-front`, normally at `http://localhost:3000/networking-app-front`.

## Build

```sh
npm run build
```

Production assets are written to `build/`. Set `REACT_APP_API_URL` before building; it is embedded in the bundle. The current `homepage` targets hosting under `/networking-app-front`; update it if deploying at a different path.
