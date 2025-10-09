# ToDo — Simple React To‑Do App

This is a small single-page To‑Do application built with React and Materialize CSS. It was created with Create React App and stores tasks in the browser's Local Storage.

## Features

- Add tasks by typing a name and pressing Enter.
- Toggle tasks as completed using the checkbox.
- Remove tasks using the X button.
- Tasks persist between sessions via Local Storage.

## Tech stack

- React (v18)
- Create React App (react-scripts)
- Materialize CSS for basic styling
- uuid for unique task ids
- gh-pages for optional deployment to GitHub Pages

## Project structure

- `public/` — static files (HTML, manifest, icons)
- `src/` — React source code
  - `Main.jsx` — main app component, handles adding tasks and date display
  - `index.js` — app entry point
  - `index.css` — base and Materialize imports/styles
  - `components/Item.jsx` — single todo item component (toggle/remove)
  - `components/List.jsx` — renders list of tasks

## Installation

Make sure you have Node.js (>=16) and npm installed.

1. Install dependencies:

```powershell
npm install
```

2. Start the development server:

```powershell
npm start
```

The app will open at http://localhost:3000 by default.

## Available scripts

- `npm start` — Start the development server.
- `npm test` — Run tests (Create React App test runner).
- `npm run build` — Build the app for production into `build/`.
- `npm run deploy` — Run the `gh-pages` deploy (the project has `predeploy` configured to build first). Update the `homepage` field in `package.json` before using.
- `npm run eject` — Eject the Create React App configuration (irreversible).

## Notes and suggestions

- The app uses Local Storage for persistence. If you need multi-device sync, integrate a backend or a cloud storage solution.
- `Item.jsx` and `Main.jsx` directly access Local Storage; consider lifting state updates to a central place (Main) and pass callbacks to children for clearer data flow.
- Input currently adds tasks only on Enter key. You may add a dedicated Add button for accessibility.

## Contributing

Small improvements, bug fixes and docs are welcome. To contribute:

1. Fork the repository and create a new branch.
2. Make changes and add tests if appropriate.
3. Open a pull request with a clear description of your changes.

## License

This repository does not include a license file. Add a license (for example MIT) if you plan to publish it publicly.

## Contact

Linkedin - https://www.linkedin.com/in/pavlo-kucheriavykh-1b8053329
