# interviewer_system

/interviewer_system
|
|-- backend/
|   |-- node_modules/           (Installed dependencies: express, cors, etc.)
|   |-- package.json            (Backend dependencies list)
|   |-- server.js               <-- EXPRESS: Defines API routes and role checks. (File 1)
|   |-- .env                    (Optional: Used for port, database connection string, etc.)
|
|-- frontend/
|   |-- node_modules/           (Installed dependencies: react, firebase, tailwind, etc.)
|   |-- public/
|   |   |-- index.html          (The HTML page that loads the React app)
|   |-- src/
|   |   |-- context/
|   |   |   |-- AuthContext.jsx <-- REACT CONTEXT: Handles Firebase auth and role (Admin/SuperAdmin) assignment. (File 3)
|   |   |-- pages/
|   |   |   |-- Dashboard.jsx   <-- REACT COMPONENT: The main UI, renders content based on the user's role. (File 4)
|   |   |-- index.css           (Tailwind import and base styles)
|   |   |-- main.jsx            <-- REACT ENTRY: Initializes the app and wraps it with <AuthProvider>. (File 5)
|   |   |-- App.jsx             <-- REACT ROUTER: The main component, acts as the gatekeeper based on `role`. (File 2)
|   |-- package.json            (Frontend dependencies list)
|   |-- tailwind.config.js      (Tailwind configuration file)
|   |-- postcss.config.js
|
|-- project_setup.md            (The project documentation/guide)
|-- README.md                   (Root documentation)
